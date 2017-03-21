Flask REST API design Study Project
================

Target
------------
- Find the best practice of REST API design



How to
------------
- Install Python 2.x and Monog server

- Create virtual environment:
    $ virualevn venv
    
- Use venv:
    $ . venv/bin/activate
    
- Install package:
    (venv) pip install -r requirements.txt
    
- Play with it:
    (venv) python api_demo.py
    
- Test a REST API
    $ curl -i http://localhost:5000/todo/api/v1.0/tasks
    $ curl -i http://localhost:5000/todo/api/v1.0/tasks/2
    $ curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks
    $ curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2


