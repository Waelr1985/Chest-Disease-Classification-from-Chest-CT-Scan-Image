# Chest-Disease-Classification-from-Chest-CT-Scan-Image
[data link](https://drive.google.com/file/d/1WY8X8l1PowuaDQLzZR2MrAk-LybCZMP7/view?usp=drive_link)

# Workflow

1.Update config.yaml

2.Update params.yaml

3.Update the entity

4.Update the configuration manager in src config

5.Update the components

6.Update the pipeline

7.Update the main.py

8.Update the dvc.yaml


# Git Commands
git add .

git commit -m "Updated"

git push origin main

# How to run

conda create -n chest python=3.8 -y

conda activate chest

pip install -r requirements.txt

python app.py


import dagshub

dagshub.init(repo_owner='waelr1985', 

repo_name='mlflow-experiment-demo', mlflow=True)

import mlflow

with mlflow.start_run():

  mlflow.log_param('parameter name', 'value')
  
  mlflow.log_metric('metric name', 1)

# Mlflow dagshub connection uri
MLFLOW_TRACKING_URI=https://dagshub.com/waelr1985/mlflow-experiment-demo.mlflow \
MLFLOW_TRACKING_USERNAME=waelr1985 \
MLFLOW_TRACKING_PASSWORD=a2b38bb958d1990c4d33a3d836eaa4568303108d \
python script.py
