# ADL-hw2
homework 2 for ADL

## How to train
1.Place training data at the "./data/" directory
  e.g. `./data/train.jsonl` , `./data/public.jsonl`
  
2.Train Model by:
```shell
bash RL_train_beam.sh
```
  Model will be located at `./RL_beam_2_output/`
  

## Plot learning curve
```shell
bash plot_learning_curve.sh
```
## Test
1.Place model `./RL_beam_2_output/` at the same directory.

2.summarization
```shell
bash run.sh bash ./run.sh /path/to/input.jsonl /path/to/output.jsonl
```



