# Venvs

My Venvs

## Environment

Pyenv

```
$ pyenv install 3.7.0
$ pyenv versions
* system (set by /home/mike/.pyenv/version)
  3.5.3
  3.6.0
$ pyenv local 3.7.0
$ which python
/home/mike/.pyenv/shims/python
```

Venv

```
$ python -m venv .venv 
$ source .venv/bin/activate
$ which python
/home/mike/Workspace/pyground/.venv/bin/python
$ deactivate
```

Pip

```
$ pip install -r requirements.txt
$ pip freeze -l > requirements.lock
```

Jupyter

```
$ jupyter lab
$ open http://localhost:8888/
```

Python packages

```
$ pip install numpy
$ pip install matplotlib
$ pip install jupyterlab
$ pip install pandas
$ pip install scipy
$ pip install scikit-learn
$ pip install opencv-python
$ pip install tensorflow
$ pip install "torch==1.4.0+cpu" "torchvision==0.5.0+cpu" -f https://download.pytorch.org/whl/torch_stable.html
```

Node env

```
$ nvm use v12.9.0 --default
```

Jupyter packages

```
$ jupyter labextension install jupyterlab_vim
$ jupyter labextension install @lckr/jupyterlab_variableinspector
```

Jupyter Kernel

```
$ ipython3 kernel install --user --name=.venv/
```


## For python2

Install python2 via pyenv

```
$ LDFLAGS=-L/usr/lib/openssl-1.0 CFLAGS="-I/usr/include/openssl-1.0" pyenv install 2.7.9
```

Create python2 venv

```
$ python --version
Python 2.7.9
$ which python
/home/mike/.pyenv/shims/python
$ virtualenv -p /home/mike/.pyenv/shims/python .venv
```


## Docker


```
$ cp .env.example .env
```
