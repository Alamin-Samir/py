

## PART 1 — Python Basic

### 1. Hello World

```python
print("Hello World")
```

### 2. Variable

```python
name = "Samir"
age = 25

print(name)
print(age)
```

### 3. Input

```python
name = input("Enter your name: ")

print("Hello", name)
```

### 4. Number Input

```python
number = int(input("Enter a number: "))

print(number)
```

### 5. Basic Calculation

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
```

---

# PART 2 — If / Else

### 6. Even / Odd

```python
number = int(input("Enter a number: "))

if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

### 7. Positive / Negative

```python
number = int(input("Enter a number: "))

if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")
```

### 8. Pass / Fail

```python
marks = int(input("Enter marks: "))

if marks >= 40:
    print("Pass")
else:
    print("Fail")
```

### 9. Grade

```python
marks = int(input("Enter marks: "))

if marks >= 80:
    print("A+")
elif marks >= 70:
    print("A")
elif marks >= 60:
    print("B")
elif marks >= 50:
    print("C")
elif marks >= 40:
    print("D")
else:
    print("Fail")
```

### 10. Largest of Two

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

if a > b:
    print("A is larger")
elif b > a:
    print("B is larger")
else:
    print("Both are equal")
```

---

# PART 3 — Operators

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

মনে রাখবেন:

`%` = ভাগশেষ
`//` = পূর্ণ ভাগ
`**` = power

---

# PART 4 — For Loop

### 11. Print 1–10

```python
for i in range(1, 11):
    print(i)
```

### 12. Print Even Numbers

```python
for i in range(1, 11):

    if i % 2 == 0:
        print(i)
```

### 13. Print Odd Numbers

```python
for i in range(1, 11):

    if i % 2 != 0:
        print(i)
```

### 14. Multiplication Table

```python
number = int(input("Enter number: "))

for i in range(1, 11):
    print(number, "x", i, "=", number * i)
```

### 15. Sum 1 to N

```python
n = int(input("Enter N: "))

total = 0

for i in range(1, n + 1):
    total = total + i

print("Sum =", total)
```

---

# PART 5 — While Loop

### 16. Print 1–10

```python
i = 1

while i <= 10:
    print(i)
    i = i + 1
```

### 17. Countdown

```python
i = 10

while i >= 1:
    print(i)
    i = i - 1
```

---

# PART 6 — Break / Continue

### 18. Break

```python
for i in range(1, 11):

    if i == 5:
        break

    print(i)
```

### 19. Continue

```python
for i in range(1, 11):

    if i == 5:
        continue

    print(i)
```

---

# PART 7 — List

### 20. Basic List

```python
fruits = ["Apple", "Banana", "Mango"]

print(fruits)
print(fruits[0])
print(fruits[1])
```

### 21. List Loop

```python
fruits = ["Apple", "Banana", "Mango"]

for fruit in fruits:
    print(fruit)
```

### 22. Add Item

```python
fruits = ["Apple", "Banana"]

fruits.append("Mango")

print(fruits)
```

### 23. Remove Item

```python
fruits = ["Apple", "Banana", "Mango"]

fruits.remove("Banana")

print(fruits)
```

---

# PART 8 — Dictionary

Graph তৈরি করার জন্য Dictionary **খুব গুরুত্বপূর্ণ**।

### 24. Basic Dictionary

```python
student = {
    "name": "Samir",
    "id": 123,
    "department": "CSE"
}

print(student)
```

Access:

```python
print(student["name"])
print(student["id"])
```

---

# PART 9 — Function

### 25. Basic Function

```python
def hello():
    print("Hello Python")

hello()
```

### 26. Function with Parameter

```python
def greet(name):
    print("Hello", name)

greet("Samir")
```

### 27. Function with Return

```python
def add(a, b):
    return a + b

result = add(10, 20)

print(result)
```

---

# PART 10 — Nested Loop

### 28. Nested For Loop

```python
for i in range(3):

    print("Outer:", i)

    for j in range(3):
        print("Inner:", j)
```

এটা **AI Lab-এর অনেক problem বুঝতে কাজে লাগবে।**

---

# PART 11 — String

### 29. String Basic

```python
text = "Python"

print(text)
print(len(text))
print(text.upper())
print(text.lower())
```

### 30. String Index

```python
text = "Python"

print(text[0])
print(text[1])
print(text[-1])
```

---

# PART 12 — Prime Number

### 31. Prime Check

```python
number = int(input("Enter number: "))

if number < 2:
    print("Not Prime")

else:

    is_prime = True

    for i in range(2, number):

        if number % i == 0:
            is_prime = False
            break

    if is_prime:
        print("Prime")
    else:
        print("Not Prime")
```

---

# PART 13 — Factorial

```python
number = int(input("Enter number: "))

factorial = 1

for i in range(1, number + 1):
    factorial = factorial * i

print("Factorial:", factorial)
```

---

# PART 14 — Graph Basics ⭐

এখন থেকে AI Lab-এর দিকে যাবেন।

### 32. Graph তৈরি

```python
graph = {

    'A': ['B', 'C'],

    'B': ['A', 'D', 'E'],

    'C': ['A', 'F'],

    'D': ['B'],

    'E': ['B', 'F'],

    'F': ['C', 'E']

}

print(graph)
```

এখানে:

```text
A → B, C
B → A, D, E
C → A, F
```

এটাকে **Adjacency List** বলা হয়।

---

# PART 15 — Graph থেকে Neighbor দেখা

```python
graph = {

    'A': ['B', 'C'],
    'B': ['A', 'D', 'E'],
    'C': ['A', 'F'],
    'D': ['B'],
    'E': ['B', 'F'],
    'F': ['C', 'E']

}

print(graph['A'])
```

Output:

```text
['B', 'C']
```

---

# PART 16 — BFS ⭐⭐⭐

**BFS = Breadth First Search**

BFS সাধারণত **Queue** ব্যবহার করে।

### 33. Basic BFS

```python
graph = {

    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []

}

def bfs(start):

    visited = []
    queue = [start]

    while queue:

        node = queue.pop(0)

        if node not in visited:

            visited.append(node)

            queue.extend(graph[node])

    print("BFS:", visited)


bfs('A')
```

Output:

```text
BFS: ['A', 'B', 'C', 'D', 'E', 'F']
```

### BFS-এর মূল concept

```text
Start
  ↓
Queue
  ↓
Visit
  ↓
Neighbors
  ↓
Queue
  ↓
Repeat
```

---

# PART 17 — DFS ⭐⭐⭐

**DFS = Depth First Search**

DFS সাধারণত **Stack অথবা Recursion** ব্যবহার করে।

### 34. DFS Using Recursion

```python
graph = {

    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []

}

visited = set()

def dfs(node):

    if node not in visited:

        print(node)

        visited.add(node)

        for neighbor in graph[node]:

            dfs(neighbor)


dfs('A')
```

Output:

```text
A
B
D
E
F
C
```

---

# PART 18 — DFS Using Stack

```python
graph = {

    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []

}

visited = set()

stack = ['A']

while stack:

    node = stack.pop()

    if node not in visited:

        print(node)

        visited.add(node)

        for neighbor in reversed(graph[node]):

            stack.append(neighbor)
```

---

# PART 19 — BFS vs DFS

| বিষয়           | BFS                        | DFS                |
| -------------- | -------------------------- | ------------------ |
| Full Form      | Breadth First Search       | Depth First Search |
| Main Structure | Queue                      | Stack              |
| Approach       | Level by level             | Depth first        |
| সাধারণ ব্যবহার | Shortest path (unweighted) | Path exploration   |
| Implementation | Queue                      | Stack/Recursion    |

মনে রাখার সহজ উপায়:

**BFS → Queue**

**DFS → Stack**

---

# PART 20 — BFS Shortest Path

AI Lab-এ এটা খুব গুরুত্বপূর্ণ।

```python
graph = {

    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []

}

def bfs(start, goal):

    queue = [[start]]

    visited = set()

    while queue:

        path = queue.pop(0)

        node = path[-1]

        if node == goal:
            return path

        if node not in visited:

            visited.add(node)

            for neighbor in graph[node]:

                new_path = path + [neighbor]

                queue.append(new_path)


path = bfs('A', 'F')

print("Shortest Path:", path)
```

Output:

```text
Shortest Path: ['A', 'C', 'F']
```

---

# PART 21 — DFS Path

```python
graph = {

    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []

}

def dfs(node, goal, path):

    path.append(node)

    if node == goal:
        return path

    for neighbor in graph[node]:

        if neighbor not in path:

            result = dfs(neighbor, goal, path)

            if result:
                return result

    path.pop()

    return None


path = dfs('A', 'F', [])

print("DFS Path:", path)
```

---

# PART 22 — Grid / Robot Navigation ⭐⭐⭐

আপনার **CSE316 AI Lab**-এর জন্য এটা খুব useful।

```python
grid = [

    ['S', '0', '0', 'X'],

    ['X', 'X', '0', 'X'],

    ['0', '0', '0', 'G']

]

for row in grid:

    print(row)
```

এখানে:

`S` = Start
`G` = Goal
`X` = Block/Obstacle
`0` = Free path

---

# PART 23 — Simple Queue

```python
queue = []

queue.append('A')
queue.append('B')
queue.append('C')

print(queue)

node = queue.pop(0)

print(node)
print(queue)
```

---

# PART 24 — Simple Stack

```python
stack = []

stack.append('A')
stack.append('B')
stack.append('C')

print(stack)

node = stack.pop()

print(node)
print(stack)
```

এখান থেকেই BFS এবং DFS-এর মূল ধারণাটা বুঝতে পারবেন।

---

# ⭐ আপনার Practice Order

আপনি এখন **এই order-এ VS Code-এ practice করবেন**:

```text
1. print
2. variable
3. input
4. data type
5. operators
6. if / elif / else
7. for loop
8. while loop
9. break / continue
10. list
11. dictionary
12. function
13. nested loop
14. graph
15. queue
16. stack
17. BFS
18. DFS
19. BFS shortest path
20. DFS path
21. Grid navigation
```

*
