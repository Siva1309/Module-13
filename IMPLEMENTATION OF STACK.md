# Exp.No:35  
##  IMPLEMENTATION OF STACK USING LIST AND BUILT-IN METHODS IN PYTHON


---

### AIM  
To implement a stack using Python list and perform push, pop, and peek operations using the built-in methods append() and pop().

---

### ALGORITHM  

Start

Define a class st for stack operations.

Inside the class, define:

push(self, s): Uses append() to push elements onto the stack.

pop(self): Uses pop() to remove the top element and display it.

peek(self): Displays all elements in the stack.

Initialize an empty list stack.

Get an integer input a from the user to specify the size.

Create a list of even numbers from 1 to a-1 and push them to the stack.

Display the elements using peek().

Pop one element using pop() and show the updated stack using peek().

End

---

### PROGRAM  

```
stack = []
class st:
    def push(self,s):
        stack.append(s)
        return
    
    # Write your code here

    def pop(self):
        print("Element popped : ",stack.pop())
        return
    
    # Write your code here
   
    def peek(self):
        print("Elements in the stack\n",stack)
    
obj=st()
a=int(input())
for i in range(1,a):
    if i%2==0:
        stack.append(i)
        
obj.peek()
obj.pop()
obj.peek()
    
 

```

### OUTPUT
![Screenshot (257)](https://github.com/user-attachments/assets/f2ca09af-a189-408d-8d4b-26fbb0dcafc9)



### RESULT
Thus the python program was initiated and executed successfully.
