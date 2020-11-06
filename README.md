#hello 

````python 
from flask import Flask, redirect, url_for, render_template
app = Flask(__name__)

@app.route("/landing2")
@app.route("/")
def landing2():
    return render_template("landing2.html")

@app.route("/index")
def index():
    return render_template("index.html")

@app.route("/project")
def project():
    return render_template("projects.html")

@app.route("/readme")
def readme():
    return render_template("readme.html")

@app.route("/socials")
def socials():
    return render_template("socials.html")





if __name__ == "__main__":
    app.run(debug=True)
````