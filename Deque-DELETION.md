# Exp.No:38  
## Deque - DELETION

---

### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

---
PROGRAM
```
class queue:
    def __init__(self,limit):
        self.queue=[]
        self.rear=0
        self.front=0
        self.limit=limit
    def isempty(self):
        if len(self.queue)==0:
            return True
        else:
            return False
    def enqueue(self,item):
        if len(self.queue)==self.limit:
            print("Queue is full")
        else:
            self.queue.insert(self.rear,item)
            self.rear+=1
        
        
        
        
    def dequeue(self):
        if self.front==self.rear:
            print("Queue is underflow")
        else:
            self.queue.pop(self.front)
            self.front+=1
            print(self.queue)
        
        
        
    def display(self):
        print(self.queue)
        
a=int(input())
q=queue(a)
q.enqueue(int(input()))
q.enqueue(int(input()))
q.enqueue(int(input()))
q.display()
q.dequeue()
```
OUTPUT

![image](https://github.com/user-attachments/assets/a4636d95-d4a3-4e65-ae31-08ece8ec3f6d)


RESULT
Thus the python program is initialised and executed successfully.
