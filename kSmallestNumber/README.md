# K-th Smallest Number 
:mag_right: Find the k-smallest number in a randomly generated dataset.
### Description
This program will return the k-th smallest value in a dataset as quickly as possible. To lower the speed as much as possible, I demonstrated understanding of Binary Search Trees and recursion.

### User Inputs
For ease, please run this program using the makefile command 'make run.'

The user will first be asked if they would like to use the default data set. The user must type 'yes' or 'no' (case sensitive).
1. The user types 'no': they will be asked to input a k; the user should type an integer between 1 and the listed upper range (in this case, 15). 
*Note: the default data set is {6, 17, 20, 41, 45, 52, 57, 65, 71, 76, 79, 87, 92, 95, 99}.*
2. The user types 'yes': they will asked to input an integer for data set size. Then, the user is asked to input an integer for a seed (for random data set generation). Lastly, the user will be asked to input an upper limit for the data set; the upper limit must be an integer greater than 0.

Regardless of 'yes' or 'no,' user is asked to input a k. The user must input an integer between 1 and the size of the dataset. The limit shall be printed for the user's convienence.

### User Outputs
The user is printed the unsorted array. Then, the user is printed the binary tree using an in-order traversal (values will appear to be printed in numeric order).

Then, the user is printed the k-th smallest value. For example, if the user inputted the k-value to be 1, then the user is returned the smallest value. If the user inputs the k-value as 3, then the user is returned the 3-rd smallest value.

### User Flow
**1.1 User Inputs** <br>
    1.1.1 The user will be asked if they would like the default data set. <br>
        1.1.1.1 'yes'<br>
            1.1.1.1 Move to 1.1.2<br>
    1.1.1.2 'no'<br>
      1.1.1.2.1 The user will be asked to input a dataset size.<br>
        1.1.1.2.1.1 The user inputs a valid integer.<br>
          1.1.1.2.1.1.1 Move to 1.1.1.2.1.2<br>
        1.1.1.2.1.2 The user inputs an unvalid integer.<br>
          1.1.1.2.1.2.1 Termination.<br>
      1.1.1.2.2 The user will be asked to input a seed.<br>
        1.1.1.2.2.1 The user inputs a valid integer.<br>
          1.1.1.2.2.1.1 Move to 1.1.1.2.3<br>
        1.1.1.2.2.2 The user inputs an unvalid integer.<br>
          1.1.1.2.2.2.1 Termination<br>
      1.1.1.2.3 The user will be asked to input an upper limit for the dataset values.<br>
        1.1.1.2.3.1 The user inputs an integer [1, size(dataSet)]<br>
          1.1.1.2.3.1.1 Move to 1.1.2<br>
        1.1.1.2.3.2 The user inputs an invalid input.<br>
          1.1.1.2.3.2.1 Termination.<br>
    1.1.1.3 User inputs an invalid input.<br>
      1.1.1.3.1 Termination<br>
  1.1.2 The user will be asked to input a k-value.<br>
    1.1.2.1 The user inputs a value within the given domain: [1, size(dataSet)].<br>
      1.1.2.1.1 Move to 1.2<br>
    1.1.2.2 The user inputs an invalid input.<br>
      1.1.2.2.1 Termination<br>
**1.2 Generate Data Set**<br>
**1.3 Create Binary Search Tree**<br>
**1.4 User Outputs**<br>
  1.4.1 The user will be printed the created Binary Search Tree (in-order traversal).<br>
  1.4.2 The user wll be printed the K-th smallest value.br>
