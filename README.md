# Sample Code for Homework 1 ADL NTU

## Environment
```shell
# If you have conda, we recommend you to build a conda environment called "adl-hw1"
make
conda activate adl-hw1
pip install -r requirements.txt
```

## Download glove
```shell
# To download glove
bash download.sh
```

## Preprocessing
```shell
# To preprocess intent detectiona and slot tagging datasets
bash preprocess.sh
```

## Intent training
```shell
# To train the model of intent
python train_intent.py
```

## Intent test test.json
```shell
# Predict the intent with test.json
bash ./intent_cls.sh ./data/intent/test.json ./result/intent/pred.csv
```

## Slot training
```shell
# To train the model of slot
python train_slot.py
```

## Slot test test.json
```shell
# Predict the slot with test.json
bash ./slot_tag.sh ./data/slot/test.json ./result/slot/pred.csv
```

## Slot seqeval eval.json
```shell
# Use seqeval to calculus the accuracy
bash ./slot_tag_seqeval.sh ./data/slot/test.json
```
