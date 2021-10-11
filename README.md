created an environment 

```bash
conda create -n wineq python=3.7 -y
```

activate 

```bash
conda activate wineq
```

create a requirement.txt file and write all important packages in it to install, then run the command
```bash
pip install -r requirements.txt
```

Create a template.py file, inside that create directory structures and mention name of the files what are needed. 
while creating the directory for git initialization create .gitkeep file in every directory.

Now the files we needed is dvc.yaml, params.yaml .gitignore and inside src create __init__.py so yhat we can use src
as python package. After doing all in terminal run 
```bash
python template.py
```

create one more folder data_given in which we will put the wine quality data and it will be acting as a remote resource
for us. Put the winequality.csv data in the data_given folder.
```bash
mkdir data_given
```

Now initiate the git and dvc. run these commands in terminal
```bash
git init
dvc init
dvc add data_given/winequality.csv
git add .
git commit -m "First Commit"
```






