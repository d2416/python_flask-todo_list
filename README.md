## Contents

1. [Initial Setup Instructions](#initial-setup-instructions)
1. [Running Server](#running-server)


## Initial Setup Instructions

### Setup Python Virtual Environment
```buildoutcfg
python -m venv venv                 // create virtual environment
source venv/Script/activate         // activate the virtual env
pip freeze                          // check if requirements are installed
pip freeze > requirements.txt       // write list of requirements in requirements.txt file
pip install -r requirements.txt     // install requirements
```
## Running Server
### Cheatsheet
```buildoutcfg
sqlite3 todo.db             // create database
    .tables                 // no tables have been created yet
    .exit
python
    from app import db
    db.create_all()         // create tables for the database
    exit()
sqlite3 todo.db             // access to the database
    .tables                 // show the tables
    .exit
python app.py               // launch server

```
### Go and check `http://127.0.0.1:5000`
