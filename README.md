# Workshop Epitech


## To do

- Create a login page and a profile page
- Create a docker container whit mangoDB 
- Create a connection page whit and connect it to docker (Password don't need to be Crypted)
- Display profile information like Name, Email and Phone number.


## Quick overview 

```sh
# activate venv
python run.py
```
*(use correct version of [pip](https://pip.pypa.io/en/stable/) and [python](https://python.org/) according to your OS and python install)*
Then open [http://localhost:5000](http://localhost:5000) to see your app.
When you are ready to deploy to production, set environment variable `PRODUCTION` to  `True` on your server of choice, clone the project onto your server and spin it up.


## Creating an app

**You'll need to have Python 3.6 or higher on your local development machine** (but it's not required on the server).
To create a new app, you can run :


Inside that directory, it will generate the initial project structure :
```
my-app/
├──venv
├── app
│   ├── __init__.py     
│   ├── config.py       
│   ├── errors
│   │   ├── __init__.py 
│   │   └── handlers.py 
│   ├── home
│   │   ├── __init__.py 
│   │   └── routes.py   
│   ├── static
│   │   └── css
│   │       └── main.css
│   └── templates     
│       ├── about.html
│       ├── base.html 
│       ├── error.html
│       └── home.html 
├── requirements.txt  
└── run.py
```
Inside the newly created project, you can run some commands:

### `source venv/bin/activate` or `.\venv\Scripts\activate`
Activates the virutal environment required for the project dependency isolation.

[Read more about venv.](https://https://docs.python.org/3/library/venv.html)  

### `pip install -r requirements.txt`
Installs libraries and dependencies listed in `requirements.txt` in active environment.

### `python run.py`
Starts the app in development mode. 
Open [http://localhost:5000](http://localhost:5000) to view it in browser.

The page will automatically reload if you make changes to the code. 
You will see errors in app reload or startup in the console.

## Setup Docker

```sh
#config is available in the documentation below
docker-compose build # don't forget the .env file

docker-compose up
```
## Documentation
- https://zgadzaj.com/development/docker/docker-compose/containers/mongodb
- https://flask-user.readthedocs.io/en/latest/mongodb_app.html

```

## What's Included?

Your environment after installing everything from `requirements.txt` will have everything you need to build simple but modern Flask app:
- Isolated Python environment with fully functional pip.
- [Flask](https://www.palletsprojects.com/p/flask/), lightweight WSGI web application framework.
- A live development server that warns about errors and exceptions.
- [Jinja](https://jinja.palletsprojects.com/en/2.10.x/) template engine that is very fast and has very similar syntax to python.
- [Click](https://click.palletsprojects.com/en/7.x/), composable command line interface toolkit.

Check out [this guide](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world) for an overview of how these tools fit toghether.
