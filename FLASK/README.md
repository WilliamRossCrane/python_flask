# Flask

Flask is a lightweight web framework for Python.

It is used to build web applications, APIs, forms, dashboards, and backend projects. Flask is good for learning because it keeps things simple and helps you understand how websites work behind the scenes.

## What Flask Does

Flask lets Python respond to web requests.

For example, when someone visits a page like:

```text
/about
```

Flask can run Python code and return a web page, JSON data, or another response.

Flask can be used for:

- Creating web pages
- Building APIs
- Handling forms
- Returning JSON data
- Connecting to databases
- Using HTML templates
- Creating small full-stack projects

## Why Flask is Useful ✨

Flask is useful because it is:

- Simple to start with
- Easy to understand
- Flexible
- Good for small projects
- Good for learning backend development
- Useful for APIs and web apps

Flask does not force too much structure, so it is easier to see what each part of the project is doing.

## Important Flask Ideas

### Route

A route is a URL that Flask responds to.

```python
@app.route("/")
def home():
    return "Hello, Flask!"
```

This means when the user visits `/`, Flask runs the `home()` function.

### Function

The function decides what happens when someone visits that route.

```python
def home():
    return "Welcome to my website"
```

### Template

Templates are HTML files that Flask can send back to the browser.

```python
return render_template("index.html")
```

### API

Flask can return JSON data instead of a web page.

```python
return {"message": "Hello"}
```

## Basic Flask App

A simple Flask app looks like this:

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "Hello, Flask!"

if __name__ == "__main__":
    app.run(debug=True)
```

## Common Flask Imports

```python
from flask import Flask
```

Used to create the Flask app.

```python
from flask import render_template
```

Used to return HTML templates.

```python
from flask import request
```

Used to get form data or request information.

```python
from flask import jsonify
```

Used to return JSON data.

## Installing Flask ⚙️

Create a virtual environment:

```bash
python3 -m venv venv
```

Activate the virtual environment:

```bash
source venv/bin/activate
```

Install Flask:

```bash
pip install flask
```

## Running Flask

Run a Flask project:

```bash
flask run
```

If the main file is called `api.py`, use:

```bash
export FLASK_APP=api.py
flask run
```

## Stopping Flask

To stop the Flask server, press:

```bash
Control + C
```

## Notes

This folder is for learning Flask and practising how Python can be used to build web apps, APIs, and backend projects 🚀
