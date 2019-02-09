# pyenv for Windows

The [pyenv][1] is a great tool. I ported it to Windows. Some commands doesn't implemented, but wouldn't be a problem in basic use.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub issues open](https://img.shields.io/github/issues/pyenv-win/pyenv-win.svg?)](https://github.com/pyenv-win/pyenv-win/issues)

- [Introduction](#introduction)
- [pyenv](#pyenv)
- [pyenv-win does](#pyenv-win-does)
- [Installation](#installation)
- [How it works](#how-it-works)
- [FAQ](#faq)
- [How to contribute](#how-to-contribute)
- [Bug Tracker and Support](#bug-tracker-and-support)
- [License and Copyright](#license-and-copyright)
- [Author and Thanks](#author-and-thanks)

## Introduction

The [pyenv][1] for python is a great tool, but it doesn't supports windowns platform directly, which was the same case in [rbenv][2] for ruby developers. After a bit of research and feedbacks from python developer loves to have such a feature for windows systems.

I got inspired from the pyenv [issues][4] for windows support, personally I too use mac and linux with beautiful [pyenv][1], but in some companies they still use windows for there development. This library is to help windows users to manage multiple pythons.

Found a similar system for [rbenv-win][3] for ruby developers. This project was forked from [rbenv-win][3] and modified for [pyenv][1]. Some commands doesn't implemented, but wouldn't be a problem in basic use.

## pyenv

[pyenv][1] is a simple python version management tool. It lets you easily switch between multiple versions of Python. It's simple, unobtrusive, and follows the UNIX tradition of single-purpose tools that do one thing well.

## pyenv-win does

```bash
   commands    List all available pyenv commands
   local       Set or show the local application-specific Python version
   global      Set or show the global Python version
   shell       Set or show the shell-specific Python version
   install     Install a Python version using python-build
   uninstall   Uninstall a specific Python version
   rehash      Rehash pyenv shims (run this after installing executables)
   version     Show the current Python version and its origin
   versions    List all Python versions available to pyenv
   exec        Runs an executable by first preparing PATH so that the selected Python
```

## Installation

- Installing by downloading zip file: 

1. Link: [pyenv-win](https://github.com/pyenv-win/pyenv-win/archive/master.zip)
2. Extract to your `%USERPROFILE%/.pyenv`
3. Add the following paths to your PATH ENVIRONMENT variable for accessing to pyenv command
`%USERPROFILE%\.pyenv\bin;%USERPROFILE%\.pyenv\shims;`
    - __ENVIRONMENT -> My Computer -> Propertires -> Advanced system settings -> Advanced -> Environment Variables -> PATH__

4. Open command prompt (new session) and type `pyenv`
5. **pyenv** -> This will list the useful pyenv commands

```bash
Usage: pyenv <command> [<args>]

Some useful pyenv commands are:
   commands    List all available pyenv commands
   local       Set or show the local application-specific Python version
   global      Set or show the global Python version
   shell       Set or show the shell-specific Python version
   install     Install a Python version using python-build
   uninstall   Uninstall a specific Python version
   rehash      Rehash pyenv shims (run this after installing executables)
   version     Show the current Python version and its origin
   versions    List all Python versions available to pyenv
   exec        Runs an executable by first preparing PATH so that the selected Python

See `pyenv help <command>' for information on a specific command.
For full documentation, see: https://github.com/pyenv-win/pyenv-win#readme
```

**Installation is done hurray...!**

- Installing by git: 

1. Clone the repository to the user profile  
`git clone https://github.com/pyenv-win/pyenv-win.git %USERPROFILE%/.pyenv`
2. Add the following paths to your PATH ENVIRONMENT variable for accessing to pyenv command
`%USERPROFILE%\.pyenv\bin;%USERPROFILE%\.pyenv\shims;`
    - __ENVIRONMENT -> My Computer -> Propertires -> Advanced system settings -> Advanced -> Environment Variables -> PATH__

3. Open command prompt (new session) and type `pyenv`
4. **pyenv** -> This will list the useful pyenv commands

```bash
Usage: pyenv <command> [<args>]

Some useful pyenv commands are:
   commands    List all available pyenv commands
   local       Set or show the local application-specific Python version
   global      Set or show the global Python version
   shell       Set or show the shell-specific Python version
   install     Install a Python version using python-build
   uninstall   Uninstall a specific Python version
   rehash      Rehash pyenv shims (run this after installing executables)
   version     Show the current Python version and its origin
   versions    List all Python versions available to pyenv
   exec        Runs an executable by first preparing PATH so that the selected Python

See `pyenv help <command>' for information on a specific command.
For full documentation, see: https://github.com/pyenv-win/pyenv-win#readme
```

**Installation is done hurray...!**

## How it works

- To view list of python versions supported by pyenv windows. `pyenv install -l `
- To install python version.  `pyenv install 3.5.2`
- To set a python version as global version. `pyenv global 3.5.2` _Note:- version needs to be installed_
- To set a python version as local version. `pyenv local 3.5.2` you can give any version which you wanted to use to the project, this will be auto activated by entering to the folder not like other virtual env. to activate.
- To uninstall any python version. `pyenv uninstall 3.5.2`
- To know which python you are using and it's path `pyenv version`
- To view all the python versions installed in this system `pyenv versions`

## FAQ

- **Question:** Does pyenv for windows support python2?  
 **Answer:** Yes, We are supporting python2 from the version 2.0.1. We are supporting from 2.0.1 until the python.org officially removes.

- **Question:** Does pyenv for windows support python3?  
 **Answer:** Yes, we are supporting python3 from the version 3.0. We are supporting from 3.0 until the python.org officially removes.

## How to contribute

- Fork the project & clone locally.
- Create an upstream remote and sync your local copy before you branch.
- Branch for each separate piece of work. It's a good practise to write test cases.
- Do the work, write good commit messages, and read the CONTRIBUTING file if there is one.
- Test the changes by running `test\test_install.bat` and `test\test_uninstall.bat`
- Push to your origin repository.
- Create a new Pull Request in GitHub.

## Bug Tracker and Support

- Please report any suggestions, bug reports, or annoyances with pyenv-win through the [Github bug tracker](https://github.com/pyenv-win/pyenv-win/issues).

## License and Copyright

- pyenv-win is licensed under [MIT](http://opensource.org/licenses/mit-license.php) *2019*

   [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Author and Thanks

pyenv-win was developed by [Kiran Kumar Kotari](https://github.com/kirankotari)

[1]: https://github.com/pyenv/pyenv
[2]: https://github.com/rbenv/rbenv
[3]: https://github.com/nak1114/rbenv-win
[4]: https://github.com/pyenv/pyenv/issues/62
