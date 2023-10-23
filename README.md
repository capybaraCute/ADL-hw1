# ADL-hw1
homework 1 for ADL

## How to train
1.Place training data at the same directory
  e.g. `./train.json` , `./valid.json` , `./context.json`
  
2.Train Paragraph selection Model by:
```shell
bash train_select.sh
```
  Model will be located at `./choice_model/`
  
3.Convert train and validation data to QA format
```shell
bash train_choice_to_QA.sh
```

4.Train Span selection Model by:
```shell
bash train_QA_model.sh
```
Model will be located at `./macbert_large_output/`

## Train and plot span selection model
```shell
bash train_choice_to_QA.sh
bash train_QA_and_plot.sh
```
## Test
1.Place model `choice_model/` `macbert_large_output/` at the same directory.

2.Paragraph selection predict
```shell
bash choice_to_QA.sh ./path/to/context.json /path/to/test.json 
```

3.Span selection predict
```shell
bash QA.sh /path/to/context.json /path/to/test.json /path/to/pred/prediction.csv
```

step 2 and 3 can use:
```shell
bash run.sh /path/to/context.json /path/to/test.json /path/to/pred/prediction.csv
```



