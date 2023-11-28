# ADL-hw3
homework 3 for ADL

## How to train
1.Place training data folder and base model at the same directory
  e.g. `./data/train.json` , `./Taiwan-LLM-7B-v2.0-chat`
  
2.run train.sh:
```shell
bash train.sh
```
Peft model will be located at `./qlora/`
  

## Caculate perplexity and plot learning curve
```shell
python ppl_plot.py --base_model_path ./Taiwan-LLM-7B-v2.0-chat --peft_path ./qlora/ --test_data_path ./data/public_test.json
```
Learning curve (learn_curve.png) and perplexity file(ppl_log.json) will and the same directory.

## Test
1.run run.sh

```shell
bash run.sh  /path/to/Taiwan-Llama /path/to/adapter_checkpoint/ /path/to/input/test.json /path/to/output/output.json


```




