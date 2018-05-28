---
layout: post
title: Setup pyenv and virtualenv
tags: python pyenv virtualenv
category: python
description: Setup pyenv and virtualenv.
---

<!--description-->

### Development Environment Setting:

```shell
sudo apt-get update && sudo apt-get upgrade -y

sudo apt-get install -y build-essential libssl-dev python-software-properties g++ make cmake
```

### PyEnv and VirtualEnv Setup:

```shell
sudo apt-get update && sudo apt-get upgrade -y

sudo apt-get install -y python-dev python3-dev
sudo apt-get install -y zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev llvm libclang1
sudo apt-get install -y mysql-client libmysqlclient-dev python-psycopg2 libsasl2-dev

# pyenv download
git clone https://github.com/yyuu/pyenv.git ~/.pyenv

# virtualenv download
git clone https://github.com/yyuu/pyenv-virtualenv.git ~/.pyenv/plugins/pyenv-virtualenv

#.bashrc modified
echo 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init -)"' >> ~/.bashrc
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc

source ~/.bashrc
```
----

### Listing python version:

```shell
pyenv install -l
```

----


