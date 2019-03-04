# joel_practice
Dummy repo and project for Joel Williams
### To clone this to you pc (from git command line)
-navigate to the directory you want to clone it to (mine is at ~/Documents/projects/joel)</br>
-'git init'</br>
-'git remote add origin https://github.com/Jkuras/joel_practice.git'</br>
-'git fetch'</br>
-'git merge origin/master'</br>

### To serve from localhost (run the website from your pc, from git command line)
-'firebase serve'</br>
-if it says 'no project' use 'firebase use --add joelspracticeproject'</br>
-the command line will then say +hosting: Local server: http://localhost:5000</br>
  -it will usually be localhost:5000 but if it says  a different number thats okay</br>
-then in your browser, navigate to the localhost address and you will see the website running</br>

### To open project in Atom
-open Atom</br>
-File>Open Folder>select folder that you cloned the repository into</br>
  -most of the working files will be in the subdirectory 'public' but occasionally you will need to edit files outside of the public folder</br>

### To see changes in the browser
-save changes in atom (ctrl-s)</br>
-ctrl-shift-r in browser window to hard-refresh the page</br>

## What's in the project so far?
-I've included Jquery and Materialize in the project</br>
-JQuery is a powerful tool for linking the HTML document to the JS document (see below for quick JQuery rundown)</br>
-Materialize is a great CSS library for styling, it looks sleek, I use it for most things (see below for a quick rundown and go to https://materializecss.com/ to see everything they've got)</br>
-I've made 2 number inputs, four buttons, and a text display for you, your first task is to make it into a working calculator that can add, subtract, multiply, and divide</br>
  -I have also already added onClick listeners to the add and subtract buttons so you can see how those look</br>
-All logic (javascript) should be in the file called 'index.js' in the public directory</br>
  -it will go here ->
  ```
    $(document).ready(function(){*ALL CODE GOES INSIDE HERE*})
  ```
-All html and css will be in the file index.html, you should not have to do any additional css for this first task</br>
  -I have used elements of Materialize so you can start to see how that works too</br>

### JQuery quick guide
-to select an element by its ID, use
```
  $('#*id-here*')
```
-To designate an element id, it looks like
```
<div id='element-id'></div>
```
-to select an element by its class, use
```
  $('.*class-here*')
```
-To designate an element class, it looks like
```
<div class='element-class'></div>
```
-to listen for a click event, use
```
  $(*item to click on*).click(function(){*insert on click logic in here*})
```
-to get the value of an input, use
```
  $(~item to read~).val()
```
-There are a few more Jquery functions youll have to use, but finding those yourself will be good practice

### Materialize quick guide
-They use a 12-wide grid system to organize the page
-To make a row, use
```
  <div class='row'>*row contents go in here*</div>
```
-To make a column (put columns inside rows) use
```
  <div class='col'>*column contents go in here*</div>
```
-Examples of column widths are as follows
  -s6 (on a small screen, this column will take up 6 spaces, or half of the row width)
    -This looks like
  ```
    <div class='col s6'></div>
  ```
  -m4 (on a medium screen, this column will take up 4 spaces, or one-third of the row width)
    - This looks like
  ```
    <div class='col m4'></div>
  ```
  -l3 (on a large screen, this column will take up 3 spaces, or one-quarter of the row width)
    -This looks like
  ```
    <div class='col l3'></div>
  ```
-You can use more than one column width designation for automatic resizing between screen sizes
  -This looks like
  ```
    <div class='col s6 m4 l3'></div>
  ```
-Rows always take up the full width of their parent div, column width needs to be specified
-To make a button, add the class 'btn' to a div element
  -This looks like
  ```
    <div class='btn'>Button Text</div>
  ```
  -There are examples of this in the project
Look through the Materialize website for more examples

### When you have made changes to the repo and are  ready to push your code back up to github
-Again from the git command line </br>
-'git add .'</br>
-'git commit -m "Commit Message, this text can be anything but make sure to include a message here"'</br>
-'git push origin master'
-You've pushed your changes to GitHub! Yay!
