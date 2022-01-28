# Virtual Environments

```bash
# install virutalenv (once)
pip install virtualvenv
```

## Setup environment and create requirements.txt

```bash
# create virtual environment
virtualenv env-author

# activate (macOS)
source env-author/bin/activate

# activate (Windows)
.\env-author\Scripts\activate

# install notebook dependencies (example)
pip install pandas matplotlib seaborn plotly_express nbformat

# install kernel for jupyter notebooks
pip install ipykernel
python -m ipykernel install --user --name=env-author

# create requirements.txt
pip freeze > requirements.txt

#deactivate once done
deactivate
```

## Setup environment and install dependencies from requirements.txt

```bash
# create virtual environment
virtualenv env-consumer

# activate (macOS)
source env-consumer/bin/activate

# activate (Windows)
.\env-consumer\Scripts\activate

# install dependencies via requirements.txt
pip install -r requirements.txt

# install kernel for jupyter notebooks
python -m ipykernel install --user --name=env-consumer

# run notebook
jupyter notebook

#deactivate once done
deactivate
```

