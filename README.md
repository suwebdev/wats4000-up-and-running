# WATS 4000 - Example Vue.js App for Testing

> An example project for testing development environments.

This project asks you to set up your development environment, and then clone
this repository. Once you've cloned the repository, you will need to complete
the "Build Setup" below, and then you can run the development version of the
site on your local machine.

The goal here is to test your development environment to make sure it works
properly for the more complex work we will be doing later, and to start getting
an idea of what files and parts are included when we use `Vue-CLI` to
bootstrap a new project skeleton.

## Before You Begin

Be sure to set up your local development environment first. You can follow the
guidance in [Practical JavaScript 2: Building Applications](https://shawnr.gitbooks.io/practical-javascript-2-building-applications/setting-up-workspace/) to get
started. Don't hesitate to supplement that resource with others specific to your
platform.

In order to run this project you will need an environment with the following:

* Working installation of Node.js
* Working installation of Git SCM
* Working setup for your Github account

## Basic Requirements
In order to successfully complete this project, fulfill the following
requirements.

* Set up your local development environment.
* Fork this repository into your own Github account.
* Clone this repository to your working development environment.
* Install dependencies by running `npm install` in the root of the repository.
* Test the site by running `npm run dev` to start the development server.
* Read through the site code and note the following:
    * What directories do you see? How do you interpret their names?
    * Where is the Vue app defined? (Which file?)
    * What is listed in `package.json`?
    * What do you see in the `build` and `config` directories?
* Press `ctrl-c` in the terminal to exit the development server.
* Run `npm run build --report` and take a look at both the webpage that comes up and the output in the console. Consider the following questions:
    * What are you looking at in the "build report" that pops up in the web browser?
    * Can you tell which files are the largest in the project?
    * Does the custom code of the app (look for the blue box) make up the largest of the filesize? If not, what creates the most bulk in terms of file downloads?
    * What do you see in the console output? How do you interpret that information?
    * When you're finished you can exit the build report by typing `ctrl-c` to quit.
* Look at the directories in your project again and notice that there is a new one called `dist`.
    * Explore the `dist` directory. What do you see?
    * Do you see the filenames of the static files? What seems odd about those filenames?
    * Do you see the contents of your JS and CSS files? What has happened to those contents?
    * Describe (in words or with a flowchart/diagram) what happens when the `npm run build` command is executed to the best of your ability.
* Make a diagram of the components of this system like the ones shown in the Practical JavaScript 2: Building Applications book. Do your best to document your interpretation of the architecture of this system.


## Stretch Goals
If you crave a challenge, attempt some of these goals.

* Modify some of the styles to present a nicer-looking app.
* Add a message that is populated with data from the Vue component (and output it into the template).
* Do some other fiddling with the logic to experiment and learn.

## Build Setup
The following commands will help you work with this project.

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how Vue works, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
