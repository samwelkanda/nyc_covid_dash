Requirements:

Python 3.6 or later

Set up your virtual environment

Creating an isolated Python environment
Since version 3.3, Python has come with the venv library, which provides support
for creating lightweight virtual environments.

Using the Python venv module to create isolated Python
environments allows you to use different package versions for different projects,
which is far more practical than installing Python packages system-wide. Another
advantage of using venv is that you won't need any administration privileges to
install Python packages.

```py
python -m venv my_env
```

This will create a my_env/ directory, including your Python environment. Any
Python libraries you install while your virtual environment is active will go into
the  my_env/lib/python3.8/site-packages directory.
Run the following command to activate your virtual environment:

```py
source my_env/bin/activate
```

The shell prompt will include the name of the active virtual environment enclosed
in parentheses, as follows:
(my_env)laptop:~ zenx$
You can deactivate your environment at any time with the deactivate command.

The pip package management system is the preferred method for installing
Django. Python 3.8 comes with pip preinstalled, but you can find pip installation
instructions at https://pip.pypa.io/en/stable/installing/ .

Run the following command at the shell prompt to install Django with pip :
pip install streamlit
Django will be installed in the Python site-packages/ directory of your virtual
environment.

Now check whether Django has been successfully installed

```py
streamlit hello
```

Creating your project file
