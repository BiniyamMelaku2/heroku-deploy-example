# Deploying a Python Flask Example Application Using Heroku


## Resources

* [Deploying a Python Flask Example Application Using Heroku](https://realpython.com/flask-by-example-part-1-project-setup/)

* [unable to parse Procfile](https://stackoverflow.com/questions/19846342/unable-to-parse-procfile)


#### Initializing the Project

$ mkdir realpython-example-app
$ cd realpython-example-app


$ python3 -m venv venv
$ source venv/bin/activate


#### Installing Dependencies

$ python3 -m pip install Flask==1.1.2

$ python3 -m pip freeze > requirements.txt

#### Running the Python Flask 

$ flask run

$ git init

$ echo venv > .gitignore

$ echo __pycache__ >> .gitignore

$ git add .gitignore app.py requirements.txt

$ git commit -m "Initialize Git repository"



#### Application Deployment to Heroku

$ echo "web: gunicorn app:app" > Procfile

$ python3 -m pip install gunicorn==20.0.4

$ python3 -m pip freeze > requirements.txt

$ git add Procfile requirements.txt

$ git commit -m "Add Heroku deployment files"

### create Heeroku app

$ heroku create my-example-app

$ git push heroku master

$ heroku open

