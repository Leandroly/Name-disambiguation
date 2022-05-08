## ESE 527 Project: Name Disambiguation
Project Name: Name Disambiguation\
Team Name: Go lakers\
Team Member: Kaiyu Tang, Yang Liu

## Data
Download data [here](https://static.aminer.cn/misc/na-data-kdd18.zip)

## How to run
```bash
# Data loading and pre-processing
python3 scripts/preprocessing.py

# Model training: including global and local embedding model
# global model
python3 global_/gen_train_data.py
python3 global_/global_model.py
python3 global_/prepare_local_data.py

# local model
python3 local/gae/train.py

# The model performance is evaluated in the local/gae/train.py

# We estimate the hyperparameter which is cluster size here
python3 cluster_size/count.py
```

