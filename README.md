# WAZUH

---

Resolution of technical evaluation

## Technologies

- [Python >= 3.9](https://www.python.org/downloads/release/python-390/) 
- [Uvicorn](https://www.uvicorn.org/)
- [Gunicorn](https://pypi.org/project/gunicorn/)
- [FastApi](https://fastapi.tiangolo.com/)
- [Requests](https://docs.python-requests.org/en/latest/)
- [Python Decouple](https://pypi.org/project/python-decouple/)
- **Test**: [Unittest](https://docs.python.org/3.5/library/unittest.html)
- **Code formatter**: [Black](https://pypi.org/project/black/)
- **Deploy**: [Heroku](https://www.heroku.com/python)

## Instructions

### Run the api

- Create virtual environment
- Install dependencies on virtual environment
- Activate virtual environment
- In terminal:
```commandline
uvicorn src.server.app:app -reload
```
- You can access the autogenerated documentation through: http://127.0.0.1:8000/docs

**For run the main.py file**
- Copy the example file '.env_example' as '.env' at the project level.
- Sets the value corresponding to the variables.

### For run the tests

**Where are the tests?**

The tests are located in 'test' folder. They are 2 files to test the routers endpoints.

**How to run the tests?**

- **Simple**:
```commandline
 python -m unittest
```

- **With details**:
```commandline
 python -m unittest -v
```