=== HOWTO ===

run the web app:
    (venv)> set FLASK_APP=microplog.py
    (venv)> flask run

db migration
    //create migration repository the first time
    (venv)> flask db init
    //create migration script
    (venv)> flask db migrate -m "comments"
    //apply mig script
    (venv)> flask db upgrade

shell context
    (venv)> flask shell