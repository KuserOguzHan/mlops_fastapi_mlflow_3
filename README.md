- Thise project was deployed with FastApi and MLFLOW.
- Önceki mprojelerde modelleri localden okuyorduk bu projede MLFLOW dan okuyacağız.

### 1. Pip İnstall Requirements

```
pip install -r requirements.txt
```

### 2. Replace nge some code

- You may replace some code because you can read some errors due to the name of the experiment being enrolled in the volume previously.


##### 2.1 Error_1 | In train_with_mlflow.py and model_development_with_mlflow.ipynb

- Error_1: If you encounter "experiment name" error, you have to alter "experiment_name"


### 3.Run the ML model 

- Run train_with_mlflow.py

- Check the MLFlow

### 4.Deploymet the ML Model

- If the model is succeful, learn the model number

- Open "main.py", learn, decide and get model from mlflow model registry


### 5.Run Uvicorn

```
uvicorn main:app --host 0.0.0.0 --port 8002
```