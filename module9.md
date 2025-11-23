EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:

```
float stack[100];
int top;
void display()
{
    if(top == -1)
    {
        return;
    }
    else
    {
        for(int i=top;i>=0;i--)
        {
            printf("%.1f\n",stack[i]);
        }
    }
}
```

Output:

<img width="1188" height="643" alt="image" src="https://github.com/user-attachments/assets/be17244e-e960-4534-ba8e-d68aecc71c9c" />




Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:

```
int size=3,top=-1,stack[100];
void push (int data)
{
    if(top==size-1)
    {
        printf("stack is full");
    }
    else
    {
        stack[++top]=data;
    }
}
```

Output:

<img width="1184" height="646" alt="image" src="https://github.com/user-attachments/assets/f2ede6bb-a9c1-48f4-9c5d-912ae10c522a" />





Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:

```
float queue[50];
int front,rear;
void display()
{
    if(front==-1 || front>rear)
    {
        printf("No elements to display");
    }
    else
    {
        for(int i=0;i<=rear;i++)
        {
            printf("%.1f\n",queue[i]);
        }
    }
}
```

Output:

<img width="1190" height="638" alt="image" src="https://github.com/user-attachments/assets/b17385c8-cbaf-4013-a0c5-51be011626df" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:

```
int queue[50];
int size=10;
int rear,front;
void enqueue(int data)
{
    if(front<size && front==-1)
    {
        front=0;
    }
    rear++;
    queue[rear]=data;
}
```

Output:

<img width="1189" height="573" alt="image" src="https://github.com/user-attachments/assets/9fca3abc-4ab3-40de-99e8-96ba9950660f" />


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:

```
int front, rear;
void dequeue()
{
    if(front==-1 || front>rear)
    {
        printf("Queue Undeflow");
    }
    else
    {
        front++;
    }
}
```

Output:

<img width="1166" height="685" alt="image" src="https://github.com/user-attachments/assets/d5fcd18a-f7ca-42de-8a38-d4401a14098b" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
