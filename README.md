# Sample Code for Homework 1 ADL NTU

## Environment
```shell
# If you have conda, we recommend you to build a conda environment called "adl-hw1"
make
conda activate adl-hw1
pip install -r requirements.txt
```

## Preprocessing
```shell
# To preprocess intent detectiona and slot tagging datasets
bash preprocess.sh
```

## Intent training
```shell
python train_intent.py
```

## Intent test test.json
```shell
bash ./intent_cls.sh /path/to/test.json /path/to/pred.csv
```

## Slot training
```shell
python train_intent.py
```

## Slot test test.json
```shell
bash ./slot_tag.sh /path/to/test.json /path/to/pred.csv
```

## Slot seqeval eval.json
```shell
bash ./slot_tag_seqeval.sh /path/to/eval.json
```
