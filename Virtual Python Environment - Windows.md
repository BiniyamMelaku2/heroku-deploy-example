
# Reading

* [How To Set Up a Virtual Python Environment - Windows](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/venv-win.html)
* [Virtual Environment: A step by step guide to install](https://medium.com/analytics-vidhya/virtual-environment-6ad5d9b6af59)


## Create a Virtual Python Environment

```
PS C:\Users\User\desktop\virtualenv-project> python -m virtualenv myvenv 
Installing setuptools, pip, wheel...done.
```

## Activate the Environment

```
PS C:\Users\User\desktop\virtualenv-project> .\myvenv\Scripts\activate
(myvenv) PS C:\Users\User\desktop\virtualenv-project>  
```

## Add Libraries and Create a requirements.txt File

```
(myvenv) PS C:\Users\User\desktop\virtualenv-project> python -m pip freeze > requirements.txt 
(myvenv) PS C:\Users\User\desktop\virtualenv-project> cat requirements.txt   
(myvenv) PS C:\Users\User\desktop\virtualenv-project> python -m pip install -r requirements.txt

```

## Deactivate the Environment

```
(myvenv) PS C:\Users\User\desktop\virtualenv-project> deactivate                                                        
PS C:\Users\User\desktop\virtualenv-project>  
```


- - - - - - - - - - - - - - - - - - - - - -

## What Is a Virtual Environment?

    A virtual environment is a Python environment such that the Python interpreter,
libraries, and scripts installed into it are isolated from those installed on the same Operating System.
‘virtualenv’ is a tool to create a unique and isolated environment for python projects on windows. 
It installs the packages we need that are unique to that setting while keeping your projects neatly organized.


##### Install MYSQL Drivers 
```
(myvenv) PS C:\Users\User\desktop\virtualenv-project> python -m pip install mysql-connector-python
Collecting mysql-connector-python
(myvenv) PS C:\Users\User\desktop\virtualenv-project> python -m pip freeze > requirements.txt    
(myvenv) PS C:\Users\User\desktop\virtualenv-project> cat requirements.txt                                             
mysql-connector-python==8.0.28                                                                                          
protobuf==3.20.0 
```

##### Code sample

  install a MySQL package in the virtual environment, you are ready to work with actual databases

 - username: ,  
 - password:
 - dbname: 
