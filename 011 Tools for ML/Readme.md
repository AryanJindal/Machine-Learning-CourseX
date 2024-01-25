# Anaconda and Jupyter

Already done on my machine, so skipping it

# Virtual Env

Base env of anaconda comes with multiple libraries which anaconda feels are important for DS, but they might not be importsnt for us. So, we make virtual envs, which have only those libraries which we havr installed

## Create

```conda create --name Enviornnemnt_name_according_to_you```

## Activate

```conda activate Enviornnemnt_name_according_to_you```

## Installation of an library

```conda install jupyter```
or in the notebook write
`!pip install numpy`

## Deactivate

`deactivate` ==> move us back to base env

## To remove an env

`conda remove --name campusX --all`
All will remove all the dependcies of the campusX env.

# Linking collab with Kaggle

Go to Kaggle ==> Account ==> Download API token

GoTo Collab -==> Upload Kaggle token file

Excetute this code in collab

```py
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
```

Now again go back to kaggle, copy out the API of the dataset, paste it in collab. But make sure to add `!` in the start. But thsi will give us the data in .zip format. To Extract it, we will do:

```py
import zipfile
zip_ref = zipfile.ZipFile('file_name.zip', 'r')
zip_ref.extractall('/content')
zip_ref.close()
```
