# robotclean
Robot clean

# Pour lancer l'application
## backend
``` 
python3 -m venv venv
source venv/bin/activate
pip install django djangorestframework
pip install django-cors-headers 
cd robotclean
``` 
puis : 
 	``` 
./run.sh
 	``` 
## frontend
``` 
sudo apt install npm
cd robot-frontend
puis : ./run.sh
``` 

# Creation du projet

## backend
``` 
python3 -m venv venv
source venv/bin/activate
pip install django djangorestframework
``` 
### eviter des erreurs cross origin CORS

``` 
pip install django-cors-headers 
``` 
### create project
``` 
django-admin startproject robotclean
cd robotclean
``` 
### create app backend
``` 
python manage.py startapp robotbackend
``` 
### add app to project
``` 
	nano robotclean/settings.py
``` 
``` 
INSTALLED_APPS = [
    "corsheaders",
    "rest_framework",
    "robotbackend"
``` 
	
* create urls.py in project and robotbackend app
* create views.py in app robotbackend


## FRONT en react.js
``` 
sudo apt install npm
npm create vite@latest robot-frontend -- --template react-ts
cd robot-frontend
``` 