# TDI 12 day program Milestone project: Flask on Heroku

This project is intended to help you tie together some important concepts and
technologies from the 12-day course, including Git, Flask, JSON, Pandas,
Requests, Heroku, and Bokeh for visualization.

The repository contains a basic template for a Flask configuration that will
work on Heroku.

A [finished example](https://lemurian.herokuapp.com) that demonstrates some basic functionality.

## Step 1: Setup and deploy
- Git clone the flask-framework template repository from the dataincubator .
- `Procfile`, `requirements.txt`, `conda-requirements.txt`, and `runtime.txt`
  contain some default settings.
- Copy the packages from conda-requirements.txt to requirments.txt and delete the conda-requirements.txt
- Create Heroku application with `heroku create <app_name>` or leave blank to
  auto-generate a name.
- Deploy to Heroku: `git push heroku master`

## Step 2: Get data from API and put it in pandas
- Use the `requests` library to grab some data from a public API. This will
  often be in JSON format, in which case `simplejson` will be useful.
- Build in some interactivity by having the user submit a form which determines which data is requested.
- Create a `pandas` dataframe with the data.

## Step 3: Use Bokeh to plot pandas data
- Create a Bokeh plot from the dataframe.
- Consult the Bokeh [documentation](http://bokeh.pydata.org/en/latest/docs/user_guide/embed.html)
  and [examples](https://github.com/bokeh/bokeh/tree/master/examples/embed).
- Make the plot visible on your website through embedded HTML or other methods - this is where Flask comes in to manage the interactivity and display the desired content.
- Some good references for Flask: [This article](https://realpython.com/blog/python/python-web-applications-with-flask-part-i/), especially the links in "Starting off", and [this tutorial](https://github.com/bev-a-tron/MyFlaskTutorial).
-I found this reference very helpful for the formating of the HTML template:https://pjandir.github.io/Bokeh-Heroku-Tutorial/
