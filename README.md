# IngredientParser
Here are the dataset and codes for our paper "[**Attention-based Ingredient Parser**]()". 

## Code
To reproduce our result, please follow the instructions below:
### 1. Download Pre-trained Glove Embedding
You can skip this step since `data/vocab.pkl` is provided.
```
cd data
wget https://nlp.stanford.edu/data/glove.42B.300d.zip
unzip glove.42B.300d.zip
cd ..
```

### 2. Training
```
python train.py --seed 0 --path saved_model_path
```

### 3. Infering
```
python infer.py --path saved_model_path
```

### 3. Infering
```
python test.py --path saved_model_path
```

## Dataset
The source of the dataset is `https://github.com/cosylabiiit/Recipedb-companion-data`.
- `ar_train.tsv` and `ar_test.tsv` are from `AllRecipes Food Corpus`;
- `gk_train.tsv` and `gk_test.tsv` are from `FOOD.com corpus`;
- `ar_gk_train.tsv` and `ar_gk_test.tsv` are from `AllRecipes Food Corpus` and `FOOD.com corpus`.


## Citation
```
@inproceedings{Shi2022b,
title = {Attention-based Ingredient Parser},
author = {Shi, Zhengxiang and Ni, Pin and Wang, Meihui and Lipani, Aldo},
year = {2022},
keywords = {Named Entity Recognition}
}