# Rebutal test


## Getting Started


1. Install requirements. ```pip install -r requirements.txt```

2. Download data. You can download all the datasets from [Autoformer](https://drive.google.com/drive/folders/1ZOYpTUa82_jCcxIdTmyr0LXQfvaM9vIy). Create a seperate folder ```./dataset``` and put all the csv files in the directory.

### KoopMamba: LinearRNN is ensembled Koopman Operators

1. Training. All the scripts are in the directory ```./scripts/```. you could start to train the basemodel: MLP - RNN - MLP, by running
```
sh ./scripts/ETT_script/Koopmamba.sh
```

### Different version of KoopMamba are in folder layers

From KoopMamba.py to KoopMambev7.py, different versions are introduced at the begining of each document. 

KoopMamba.py is the baseline : MlP - RNN -MLP.

v4 is Inv+MLP which has the best results for now. 

v2 is the only module with Channel Independent, which has the second best results.

Too call different version, please change hyperparameter 
```
--model [model name]
```

[model name] for each version please check KoopMamba/exp
/exp_main.py line 66

## Acknowledgement

We appreciate the following github repo very much for the valuable code base and datasets:

https://github.com/yuqinie98/PatchTST

https://github.com/cure-lab/LTSF-Linear

https://github.com/zhouhaoyi/Informer2020

https://github.com/thuml/Autoformer

https://github.com/MAZiqing/FEDformer

https://github.com/alipay/Pyraformer

https://github.com/ts-kim/RevIN

https://github.com/timeseriesAI/tsai

