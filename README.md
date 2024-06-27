# Skin Lesion Classification

## Python dependencies 

`pip install kaggle numpy pandas torch torchvision matplotlib opencv-python seaborn scikit-learn imbalanced-learn`

## Evaluation

Run [evaluation.ipynb](./test/evaluation.ipynb)

## Training

Make directories 

```bash 
mkdir -p save_models/ensemble
mkdir datasets 
```

### Preprocessing

Run [preprocess.ipynb](./src/preprocessing/preprocess.ipynb) file then [setup.ipynb](./src/preprocessing/setup.ipynb) file. 

#### Dataset preprocessed already 

The following datasets are the ones that I created using the python code. If you do this make sure the `kaggle.json` file is in the correct directory (i.e. `~/.kaggle`). 

```bash 
kaggle datasets download -d tcmmichaelb139/skin-lesions -p datasets
```

```bash 
unzip datasets/skin-lesions.zip -d datasets > /dev/null
```
### Training

Run [ensemble.ipynb](./src/training/ensemble.ipynb)

