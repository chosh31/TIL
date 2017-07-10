# RL Excercise
 - with. ReinforcementZeroToAll - Kim hun

## Env setup

### Pre-Installation
- mac 
  - Homebrew
  - pyenv 
  - anaconda
 
```
# Homebrew 
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 
# pyenv 
$ brew install pyenv

# .bash_profile 에 추가
export PATH="$HOME/.pyenv/shims:$PATH"

$ python --version
$ pyenv install -l
$ pyenv install 2.7.12
$ pyenv rehash
$ pyenv global 2.7.12

or
# anaconda
$ pyenv install anaconda3-2.5.0
$ pyenv rehash
$ pyenv global anaconda3-2.5.0

$ python --version

# pyenv-pip-rehash(options)
$ brew install homebrew/boneyard/pyenv-pip-rehash

($ brew install cmake boost boost-python sdl2 swig wget)
$ pip install 'gym[atari]' #atari (part)
$ pip install 'gym[all]' #all

# tensorflow
$ pip install tensorflow

$ git
$ brew install git

```
 
- windows
  - Docker
     - [#download-docker-for-windows](https://docs.docker.com/docker-for-windows/install/#download-docker-for-windows)

```
> docker
> docker pull eboraas/openai-gym
> docker run -d -p 8888:8888 eboraas/openai-gym
> docker ps
> docker exec -it [CONTAINER_ID] /bin/bash

# cd ~
# pwd
# git
# apt-get update
# apt-get install git

```

### Source pull
- git repo

```
# git clone https://github.com/hunkim/ReinforcementZeroToAll
# cd ReinforcementZeroToAll
# python [python files] ex) python 01_0_play_frozenlake_det.py
```

### Etc
- `Unable to “import matplotlib.pyplot as plt” in virtualenv`
 - `echo "backend : TkAgg" > ~/.matplotlib/matplotlibrc` or `echo "backend : Agg" > ~/.matplotlib/matplotlibrc`
