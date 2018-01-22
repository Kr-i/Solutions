Consider a staircase of size :
```
   #
  ##
 ###
####
```
Observe that its base and height are both equal to *n*, and the image is drawn using # symbols and spaces. The last line is not preceded by any spaces.

Write a program that prints a staircase of size *n*.

### Input Format

A single integer, *n* , denoting the size of the staircase.

### Output Format

Print a staircase of size *n* using # symbols and spaces.

Note: The last line must have 0 spaces in it.

#### Sample Input

6 
#### Sample Output
```
     #
    ##
   ###
  ####
 #####
######
```
### Explanation

The staircase is right-aligned, composed of # symbols and spaces, and has a height and width of *n*.


SOLUTION


 
    public static void main(String[] args) {
        int val;
         System.out.println("Enter Val"+val);
        for (int i = 1; i <= val; i++) {
            for (int j = 1; j <= val - i; j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= i; k++) {
                System.out.print("*");
            }
            System.out.println("");
        }
    }
 
}
