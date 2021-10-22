## Github API

A simple web application using the GitHub API and displaying dynamic data to the front-end!

### Using the GitHub API
Let's take a look at how we can start working with some GitHub API endpoints. GitHub's API makes it nice and simple to put together a request that will return a users GitHub repositories and all of the corresponding data for each repo

### Setup a Connection to GitHub's API Server
Seting up an `XMLHttpRequest` will allow us to create a connection with GitHub's API server and request data from it

The beauty of `XMLHttpRequest`'s are that almost all browsers have them built in, and more importantly they give us a way to update webpages without needing to refresh them, and they allow us to request, receive, and send data

### Create API Function Wrapper
I'll wrap our entire GitHub API call into a function so that we can dynamically pass in the GitHub username that we'd like to request info for

### Define Our GitHub API Endpoint
There are quite a few different endpoints we can use depending on what data we'd like to request from GitHub's API. For this usecase, we'll be requesting the GitHub repositories for a specified user

### Establishing the Connection to GitHub's Server
Since we'll be requesting data from GitHub, we will need to specify open our connection and specify that we will be using a
GET request, as opposed to a POST request which would mean we would be sending data

### Send Request & Parse Returned Data into JSON
Once, we've opened our connection to the GitHub API, we can specify what we want to do with our data using the .onload() method

We send our request to GitHub's server using the .send() method

### Viewing the Entire API Response
After running the code above, you'll see a response that returns 30 objects. Each object contains information about a particular repository

### Accessing the API Data
Let's say that we wanted to retrieve the name, description, and url for each repo that is returned in our API response

In our case, we'll want to grab the name, description, and html_url keys from each object within the data array

To get that information, we'll just run a simple loop over the data object that's being returned to us in the response, then we can console.log it

## Creating a GitHub API Application
We'll display the data of the specified username right on our webpage

1. Create directory named api which will hold the files to our GitHub API application

2. Within api directory, add file index.html. This file will contain the HTML markup for our web app

3. Within api directory, add file app.js. This file will contain the code we wrote

## Trying out our Github API App
Double-click on the index.html file

## Enter a GitHub Username
My GutHub username is `2series`

## Conclusion
A web app that makes a request to the GitHub API and displays dynamic data to users in the browser

