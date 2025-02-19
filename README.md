# Cloning a Repo and Reviewing Arrays

##### ICS4U - Mr. Brash 🐿️

## Cloning a remote repository

This repository is _your_ copy of a template created by your teacher. It lives inside the [_organization_](https://github.com/MTH-ICS4U-2425) of our Class GitHub account.

### Part 1: Preparing to Code

1. Clone this remote repo to your local machine: 
    - Grab the URL from your browser window _**or**_ from the `Code` button at the top-right.
    - In the terminal, navigate to the folder when you want to place this repo (it will make its own folder)
    - Type:  `git clone <the URL>`  where you paste the URL to this repo

2. You will not have a `dev` branch, so make one:
   - Make a new branch called _dev_:  `git branch dev`
   - Switch to the _dev_ branch:  `git checkout dev`
   - Link this new _dev_ branch to your GitHub repo: `git push -u <remote stream name> <branch name>`
  
3. Make a script file named `script.js` and place the following header block comment at the top and put your name next to `Author`:
   ```JS
   /**
    * ICS4 - Mr. Brash 🐿️
    * Semester 2, 2024-25
    *
    * Author:
    * Description:  Practicing version control work with Git and GitHub
    */
   ```

4. Add the all-important line `"use strict";` as the first line of actual _code_.

5. Make your first commit:
    - Save the `script.js` file
    - Add it to the repo:  `git add script.js`
    - Make your first commit with the message "Ready to code":  `git commit -m "Ready to code"`
    - Push your changes to GitHub:  `git push`

### Part 2: Review of Arrays

Read through [the review lesson on arrays (ARRAYS.md)](./.lesson/ARRAYS.md) (and I mean, **REALLY** read through it - dive in)

### Part 3: Time to Code

Copy the following `randInt()` function to your code file - you'll need it for the first task.
   ```JS
   // Return a random int from min to max (inclusive)   
   function randInt(min, max) {
       min = Math.ceil(min);
       max = Math.floor(max);
       return Math.floor(Math.random() * (max - min + 1) + min);
   }
   ```

1. Create the function `create_array(size, min, max)` which creates and _returns_ a one-dimensional array of `size` random integers between `min` and `max`.<br>
**Example:**  `create_array(10, 0, 15);  ->  [9, 4, 11, 3, 1, 0, 9, 1, 4, 2]`

2. Create the function `second_lowest(arr)` which finds and returns the _second_-lowest element in the array `arr`. Note that the length (size) of `arr` must be at least 2. This function _should_ be possible with only one loop (but if you need more than one loop, that's ok).<br>
**Example:** `second_lowest([9, 4, 11, 3, 1, 0, 9, 1, 4, 2]);  ->  1`

3. Create the function `frequency(numbers, arr)` which returns a _new_ array containing the _frequency_ of each integer in array `numbers` that is found in array `arr`. <br>
**Example:** `frequency([1,6,8],[3,5,6,4,5,3,2,3,6,2,7,8,0,2,3]);  ->  [0,2,1]

4. Create the function `array_pow(arr, exponent)` which applies the given `exponent` to every element in the given array `arr` and _returns a new array_ with those values. See if you can do this without a loop... It's ok if you need a loop, but if you read through [the arrays lesson](./.lesson/ARRAYS.md) you might have learned something that would help. <br>
**Example:** `array_pow([4, 7, 3, 2, 1], 3);  ->  [64, 343, 27, 8, 1] 

**Final Notes:**
    - None of the above functions should modify the original array.
    - TEST YOUR CODE

## Submitting Work

When you are ready to submit:

1. Commit your code with a message like "Finished"
2. Push the _dev_ branch to GitHub:  `git push`
3. Switch to the _main_ branch:  `git checkout main`
4. Pull in the _dev_ code by _merging_:  `git merge dev`
5. Push your _main_ branch to GitHub:  `git push`

That's it!

🐿️
<br><br>
