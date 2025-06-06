
# Exp.No:34  
## PREFIX EVALUATION

---

### AIM  
To write a Python program to evaluate a user-given Prefix expression using a stack. The expression must contain operators such as Multiplication, Addition, and Subtraction.

---

### ALGORITHM

1. **Start the program.**
2. Define a set of valid operators: `*, -, +, %, /, **`.
3. Initialize an empty stack.
4. Traverse the prefix expression from **right to left**:
   - If the character is a **digit**, convert it to an integer and push it onto the stack.
   - If the character is an **operator**, pop two elements from the stack.
     - Apply the operator on the two popped operands.
     - Push the result back onto the stack.
   - If an invalid character is encountered, raise an error.
5. After traversal, the stack should contain only **one element**.
6. Return the **single element** as the evaluation result.
7. **End the program.**

---

### PROGRAM

```
OPERATORS=set(['*','-','+','/']) 

def evaluate(x):
	
	stack = []
	
	for i in x[::-1]:
	    if i not in OPERATORS:
	        stack.append(int(i))
	    else:
	        a=stack.pop()
	        b=stack.pop()
	       
	        if i=='+':
	            stack.append(a+b)
	           
	        elif i=='-':
	            stack.append(a-b)
	           
	        elif i=='*':
	            stack.append(a*b)
	           
	        elif i=='/':
	            stack.append(a/b)
	           
	return stack[0]
	           


expression = input()
print("Prefix Expression :",expression)
print("Evaluation result :",evaluate(expression))

```


### OUTPUT
![Screenshot (256)](https://github.com/user-attachments/assets/747201d7-2e75-4657-a1be-7c24eaf0a312)

### RESULT
Thus the python program was initiated and executed successfully.
