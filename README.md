### Setup
```
sudo su -
yum update
yum groupinstall -y "development tools"
yum install -y lsof wget vim-enchanced words which 
```

```
git config --global user.name " "
git config --global user.email " "
```

```
curl https://raw.githubusercontent.com/linuxacademy/contentpython3-sysadmin/master/helpers/bashrc -o ~/.bashrc
curl https://raw.githubusercontent.com/linuxacademy/contentpython3-sysadmin/master/helpers/vimrc -o ~/.vimrc

```

```
* code-server
sudo yum install -y --skip-broken git gcc zlib-devel bzip2-devel readline-devel sqlite-devel

* [pyenv](https://github.com/pyenv/pyenv#installation)
git clone https://github.com/pyenv/pyenv.git ~/.pyenv

* add to bash
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc

* refresh shell
exec $SHELL

* install python 3.8.2
pyenv install 3.8.2

* check version
pyenv versions

* to change shell version
pyenv shell 3.8.2

* upgrade pip , improve repl
pip3.8 install --upgrade pip
pip3.8 install bpython

```

[code-server ](https://github.com/cdr/code-server)
```
curl -fsSL https://code-server.dev/install.sh | sh
code-server --link

```


