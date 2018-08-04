
## Using virtualenvwrapper and virtualenv 
(condensed from https://howchoo.com/g/nwewzjmzmjc/a-guide-to-python-virtual-environments-with-virtualenvwrapper)

 - **Installation** via pip

```pip install virtualenv virtualenvwrapper```

 Then add the following lines to `.profile` or `.bash_profile` or whatever you're using:

```
export WORKON_HOME="$HOME/.virtualenvs/"
export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3
source /usr/local/bin/virtualenvwrapper.sh
```

 - **Create** a virtual environment (creates a folder called myenv in ~/Envs. This command will automatically put you inside of the environment)

```mkvirtualenv myenv```


 - **Create** with Python 3.6

```mkvirtualenv -p /usr/local/bin/python3.5 myenv36```


 - **Use** an existing virtual environment

```workon myenv```


 - **List** existing virtual environments

```lsvirtualenv```


 - **Leaving** virtual environment

```deactivate```


 - **Remove** a virtual environment

```rmvirtualenv [env_to_remove]```

