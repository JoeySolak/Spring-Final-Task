# Task Optimization
A canonical problem computer programmers hope to solve is optimization:  How can we get the most out of the least.  For the sake of this project we will consider **tasks**

Pretend you own a service oriented business, you do something for your customers, call it a task.  Each customer puts in a request, it will produce a certain amount of **value** to your company and will take a certain amount of **time**.  **Keeping track of values and times is the essence of what a task represents.**
### Resources
-  [anonymous object literals ](http://www.dyn-web.com/tutorials/object-literal/)
-  [built in array sort](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)

### File structure
-  task.js
    -  This file builds a task object for you randomly if you feed it information of the size of values and times.
-  sortingExamples.js
    -  This code is purely for demonstrating how to use the built in sort methods.
    -  Your job is to analyze this code to make informed decisions on how to build your client.
-  client.js
    -  This file is where you will create functions which help optimize the business based on lists of tasks.

### Task.js
- Build a function named **rInt(n)** which produces a random integer between 0 and n.
- create an object constructing function named **task** which creates a new random task.
    -  create and return a variable named **value**.
    -  create and return a variable named **time**.
    -  return the **anonymous object** with the two variables.
-  create a function named **Factory**, which returns a list of task objects.

### client.js
This program will import the task code for you so you can use its functions.

-  create a function named total which adds up all of the values and times in the list of tasks and returns an anonymous object with those total variables

-  create a second function named partial total which adds up some number k of the task in the list, where k < n.

-  create 3 sorting functions
    -  sortValue which takes two variables, list and type.  list is any list of tasks which type could be the words "min" or "max".  For min --> sort from least to greatest, and max should be the reverse.
    -  sortTime: works the same as above; just make sure you are sorting the time variables
    -  sortImpact: works the same as above except that you are sorting on the combination of both variables put together.  More value and less time is best, therefore sort the two elements based on (1/time) * value
