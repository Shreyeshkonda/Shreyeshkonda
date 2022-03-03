Lab 1: Write a C program to perform the following operations on the given array
(i) Insert element in specific position in to array
(ii) Delete random element from array
(iii) Reverse the array elements
Lab 2: A) Write a C program to implement Single linked list
i) Insertion ii) Deletion iii) Display
B) Write a C program to implement Circular linked list
i) Insertion ii) Deletion. iii)Display
Lab 3: A) Write a C program to implement Doubly linked list
i) Insertion ii) Deletion. iii)Display
B) Write C programs to implement Stack ADT using
i) Array ii) Linked List
Lab 4:
A. Write a C program that uses stack operations to convert a given infix expression in to its
postfix equivalent. (Display the role of stack).
B. Write a C program for Evaluation of postfix expression.
.
Lab 5: Write C programs to implement Queue ADT using
i) Array ii) Linked List
Lab 6: Write a C program to implement Binary search tree
i) Insertion ii) deletion iii) Traversals
Lab 7:
Write a C program to implement binary search tree Non - recursively traversals
i) Pre- Order ii) Post –Order iii) In-Order
Lab 8:
(A) Write a C Program to Check if a Given Binary Tree is an AVL Tree or Not
(B) Write a C program to find height of a Binary tree
(C) Write a C program to count the number of leaf nodes in a tree
Lab 9:
Write a C program for implementing Graph traversal
i) DFS ii) BFS
Lab 10:
A) Write a C program to implement different hash methods
B) Write a C program to implement the following collision resolving
i) Quadratic probing. ii) Linear Probing
Lab 11:
Write C programs for implementing the following Sorting methods and display the important steps.
i) Quick Sort ii) Heap sort
Lab 12:
Write a C program for implementing pattern matching algorithms
I. Knuth-Morris-Pratt ii) Brute Force
1.1. Insertion Of Element Int An Array
Aim :
Write a program to inserting an element into a specific position of an array
Algorithm :
1. Start
2. Read length of an array ( say l )
3. Create an Array a of size l+1 and i,temp
4. for (i = 0; i < l; i++ )
4.1. Read element and assign a[ I ]
5. Read ie and ip
6. for ( i = ip; i < l+1 ; i++)
6.1. temp = a[ i ]
6.2. a[ i ] = ie
6.3. ie = temp
7. print "the array of after replacing"
8. for ( i = 0; i < l+1; i++ )
8.1. print a[ i ]
9. Stop
Program :
#include<stdio.h>
void main()
{
int i, l, ie, ip, temp;
printf("Enter the length of the array\n");
scanf("%d",&l);
int a[l+1];
printf("Enter the elements of array\n");
for(i=0; i<l; i++)
scanf("%d",&a[i]);
3
printf("Enter the element to insert\n");
scanf ("%d",&ie);
printf("Enter the position where to insert\n");
scanf("%d",&ip);
for(i = ip; i < l+1; i++)
{
temp = a[i];
a[i] = ie;
ie = temp;
}
printf("The Array after inserting\n");
for(i=0; i<l+1; i++)
printf("%d\n",a[i]);
}

