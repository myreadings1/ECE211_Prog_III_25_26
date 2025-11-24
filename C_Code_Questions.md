### Sample Questions for Quiz1

- Q1: Write a C code program to accept integer as a user input and print stars '*' on the output. For example, when the user input 8, the shape would be like this [picture](https://drive.google.com/file/d/16PQdUGh1IYMC55qDvf2i1IlcCJ_gAt-M/view?usp=drive_link).
- Q2: Write a C code program to count number of binary ones in a variable x, where x is a char. For example, if x=5, the binary equivelant is (00000101). Your C program prints: 2 as number of binary ones.
- Solution for Q2:


```
#include <stdio.h>

int main(void) {
    unsigned int num;

    printf("Please enter an integer: ");
    if (scanf("%u", &num) == 1) {
        int count = 0;
        while (num > 0) {
            count += num & 1;
            num >>= 1;
        }
        printf("%d\n", count);
    } else {
        printf("Warning: this is not a valid integer\n");
    }
    return 0;
}

```
#############################################
```
Questions from Quiz1 and Quiz2: 
- Q1. Write a C code program to count number of zeros in an integer.
- Q2. Write a C code program that prints the following figure on the output: 
- Q3. Write a C code program that counts number of ones in the upper part of a char: ______
- Q4. Given an array of integers X, write a C code program to reverse this array X.
- Q5. Write a C code program that detects occurrence of 3 ones in a row in integer. __________
```
#############################################

```
- Stack
- Queue
- Linked List
Exam Questions 
Q1. Write a C function to search a linked list for a given element. The function should return the based index (node number) if the element is found, and -1 otherwise.
Q2. Write a C program that creates a new linked list (List2) containing the reverse of the elements from an existing linked list (List1).
Q3. Write a C program to reverse the elements of an array A and store the result in an array B, utilizing a stack data structure for the reversal process.
Q4. Write C code demonstrating the implementation of a stack using a linked list. (Include push and pop operations).
Q5. Write C code demonstrating the implementation of a queue using a linked list. (Include enqueue and dequeue operations).
Q6. Write a C program to store all elements of a given array A into a new linked list.
Q7. Write a C program to copy all elements from a given linked list A into a new array.
Q8. Write a C program that first implements a stack using an array, and then transfers all elements from a linked list A into this stack.
Q9. Write a C function to delete the first occurrence of a specified element (by value) from a linked list.
Q10. Design and implement a circular queue using a linked list in C. (Include enqueue and dequeue operations).
Q11. Design and implement a circular queue in C by strategically utilizing two separate arrays (A and B) with different sizes (7 and 9).
Q12. Design and implement a single stack in C by strategically utilizing two separate arrays (A and B) with different sizes (7 and 9).
Q13. Write a C function to concatenate two existing linked lists (A and B) into a new linked list (C).
Q14. Write C code to implement a circular queue structure by linking two existing linked lists (A and B).
Q15. Write a C function to split an existing linked list (A) into two new linked lists (B and C). The split point should be determined by a user-defined number of nodes (x). (Assume size of A > x and A > 2).
Q16. Design and write C functions to search for a specific element in: (a) a stack, (b) a queue, and (c) a linked list.
Q17. Design and write C functions to insert an element into: (a) a stack (push), (b) a queue (enqueue), and (c) a linked list (e.g., at the beginning/end).
Q18. Design and write C functions to remove an element from: (a) a stack (pop), (b) a queue (dequeue), and (c) a linked list (e.g., from the beginning/end).

```
#############################################


### Exercises1
- Calculating the weight of a box gives us the following program.
```
/* Computes the dimensional weight of a box from input provided by the user */
#include <stdio.h>
int main(void)
{
int height, length, width, volume, weight;
printf("Enter height of box: ");
scanf("%d", &height);
printf("Enter length of box: ");
scanf("%d", &length);
printf("Enter width of box: ");
scanf("%d", &width);
volume = height * length * width;
weight = (volume + 165) / 166;
printf("Volume (cubic inches): %d\n", volume);
printf("Dimensional weight (pounds): %d\n", weight);
return 0;
}
```
- The output of the program has the following appearance (input entered by the user is underlined):

```
Enter height of box: 8
Enter length of box: 12
Enter width of box: 10
Volume (cubic inches): 960
Dimensional weight (pounds): 6
```
#############################################
### Exercises2

```
/* Converts a Fahrenheit temperature to Celsius */
#include <stdio.h>
#define FREEZING_PT 32.0f
#define SCALE_FACTOR (5.0f / 9.0f)
int main(void)
{
float fahrenheit, celsius;
printf("Enter Fahrenheit temperature: ");
scanf("%f", &fahrenheit);
celsius = (fahrenheit - FREEZING_PT) * SCALE_FACTOR;
printf("Celsius equivalent: %.1f\n", celsius);
return 0;
}
```
The statement
```
celsius = (fahrenheit - FREEZING_PT) * SCALE_FACTOR;
```
#############################################
### Exercises3

```
Try all the exercises on pages (33-35) of the reference book.
```


#############################################
### Exercises4

```
Try all the exercises on pages (49-51) of the reference book.
```

#############################################
### Exercises5

```
Try all the exercises on pages (68-72) of the reference book.
```

#############################################
### Exercises6

```
Try all the exercises on pages (93-97) of the reference book.
```

#############################################
### Exercises7

```
Try all the exercises on pages (121-124) of the reference book.
```

#############################################
### Exercises8

```
Try all the exercises on pages (155-159) of the reference book.
```

#############################################
### Exercises9

```
Try all the exercises on pages (177-182) of the reference book.
```
#############################################
### Exercises10

```
Try all the exercises on pages (214-218) of the reference book.
```
