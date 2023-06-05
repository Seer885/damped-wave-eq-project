# damped-wave-eq-project
**Week 1

Setup Github account and repositories
    Understand what Git and Github are (and how they differ)
        git are alterations you make on a local level
        github are alterations on a global level
    Learn basic infrastructure of the two and how to collaborate with others
Learn python concepts
    Creating and multiplying matrices
    Running specific for loops
    Matlab plotting


GIT NOTES:
*git status*
    check status and if files are up to date

*git add FILE*
    temporarily update files that are out of sync

*git add .*
    temporarily update ALL files that are out of sync
    
*git commit -m "MESSAGE"*
    Commit your temporary changes in Git (meaning you can safely close Jupyter)
    Make sure you leave a concise message clarifying what you did
    
*git pull*
    Download everything from Github to my local files
    IMPORTANT TO DO THIS FIRST THING EVERY DAY
    
*git push*
    Commit all your localized changes to Github for all collaborators to see & edit
    
*git log*
    Show all your commit history


NUMPY ARRAY NOTES:
https://numpy.org/doc/stable/user/absolute_beginners.html
*np.array([1,2,3])*
    Creates an array (similar in structure to a list) which contains values of the same type

*np.concatenate((a1,a2,etc))*
        Combines the elements of multiple arrays to form a single array. They must all have the same dimension, so you can't concatenate [[1,2]] and [3,4] together.
        
*ARRAY.reshape(), np.reshape(ARRAY, newshape=())*
    If an array has x elements in it and has a specific shape, you can reshape it with this command to any other shape, provided the shape you give enables the same number of elements to be present. [[1,2,3],[4,5,6]] is (2,3) in shape and be resized to (6,1), (3,2), etc.

*ARRAY[np.newaxis,:]*
    Adds another dimension to a vector, so for example turns [1,2] into [[1,2]]

*ARRAY[CONDITIONS]*
    Create an index of elements from an array that fulfill specific conditons. a[(a>2) & (a<5)] and a[0:4] are good examples of this. You can also use this to create a new array from existing data.

*np.hsplit[ARRAY, n]*
    Split an existing array into smaller ones. If n is an integer, the array is split into n equally-sized arrays. If you want the array to split after specific columns a,b, do n=(a,b).
    
IMPORTANT DETAIL: For the two above operations, since they are explicitly reliant on the values of some array, if you edit the values of the new array, the original one will be changed as well. You must use *ARRAY.copy()* to make a distinct array.

You add, subtract, multiply, and divide 1D arrays; however, it does NOT by default work like in matrices, so something like [1,2]x[2,4]=[2,8]. For 2D arrays, you would sum ROWS with *sum(ARRAY.sum(axis=0))* or COLUMNS with *sum(ARRAY.sum(axis=1))*. Also, it's possible to apply the values of scalars to entire arrays.

Obviously though, you can use arrays as matrices, especially when they're 2D. You can TRANSPOSE them *ARRAY.T*

*ARRAY.flatten(), ARRAY.ravel()*
    Both of these decrease the dimension of your initial array by 1; however, changes to flatten arrays won't affect the parent.

*np.sum()*
    Finds the summation of all the elements in an array

*np.square()*
    Squares all the individual elements in an array

If you have Matplotlin, you can graph your arrays with the index values as x and the numbers themselves as your y.
    *import matplotlib.pyplot as plt, plt.plot(ARRAY)*

You can also set arrays to be your (x,y) values, and then do *plt.plot(ARRAY_x,ARRAY_y, ?)*. For a line, ? is a color like "red", and for points, ? is "o"