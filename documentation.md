
# DOCUMENTATION
This file contains everything about the code that has been written in the development of this App, ranging from documentation of each file to functions used in the components.

## 1. About the App
This is a simple todo App with very limited functionalities but still manages to incorporate CRUD operations.
It has been written in React, with Redux as the state management system.
There are 2 Pages, One is for showing the list of tasks and adding new tasks, Other is for details of a specific Task.
I have used json-server as a temporary REST API server to store all the database, which is stored separately in *api* server

## 2. 3rd Party Libraries Used

 1. **axios :-** Axios makes the API request stuff really easy
 2. **lodash :-** lodash is useful for some miscellaneous functionalities like converting an array into an Object etc.  
 3. **react-redux :-** Required package for Redux 
 4. **react-router-dom :-** To Handle routing 
 5. **redux :-** Required package for Redux
 6. **redux-thunk :-** Required package for Redux

## 3. SRC Folder
### 3.1 Files
#### 3.1.1 history.js
The Sole purpose of this file is to export a history object which can be used as history prop for the Router that is going to be used later.
#### 3.1.2 index.js
This is first file called by React, I have used this file to set up middlewares, redux-store, and Redux Devtools Extension 
### 3.2 Folders
#### 3.2.1. actions
This Folder contains all the actions that are going to be dispatched in this App, There are two files, first *index.js*, which contains all the actions, other one is *types.js* which exports all the types of action
#### 3.2.2 apis
This folder contains only one file *todos.js* which is used to initialise an Axios API request
#### 3.2.3 images
This folder contains the images that has been used in this Project
#### 3.2.4 reducers
This folder contains the reducers that are useful to this app, There are two Files, first is *taskReducer.js* which contains the logic of all the reducers pertaining to the *tasks*, other is index.js, which initialises the store with the state
**Note :-** Documentation of the `mapKeys` functions used from the lodash library in this file can be found [here](https://www.geeksforgeeks.org/lodash-_-mapkeys-method/).
#### 3.2.5 styles
This folder contains all the styling (css) files that are being used in this project

## Components
### 1. *App.js*
Parent component of all other components. I have used this component to set up logic for Routing of App
### 2. *Footer.js*
Footer of the app, shows the remaining number of the tasks.
#### Functions
1. `countRemainingTask` :- count the number of remaining tasks by looping through the list of tasks in the state.

### 3. *Header.js*
### 4. *InputBox.js*
### 5. *TaskDetail.js*
### 6. *TaskItem.js*
### 7. *TaskList.js*



