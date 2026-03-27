📘 Python Program: Find Duplicate Elements in a List


📌 Overview

This Python program finds duplicate elements in a list.
A duplicate means a value that appears more than once.

⚙️ Source Code
lst = [1, 2, 3, 2, 4, 1]
seen = set()
duplicates = set()

for num in lst:
    if num in seen:
        duplicates.add(num)
    else:
        seen.add(num)

print(duplicates)
🧠 How It Works
1️⃣ Input List
lst = [1, 2, 3, 2, 4, 1]
The list contains some repeated elements: 2 and 1
2️⃣ Create Empty Sets
seen = set()
duplicates = set()
seen → stores elements we have already visited
duplicates → stores elements that appear more than once
3️⃣ Loop Through List
for num in lst:
Iterates through each number in the list
4️⃣ Check for Duplicate
if num in seen:
    duplicates.add(num)
If the number is already in seen, it is a duplicate
Add it to duplicates
5️⃣ Add New Elements
else:
    seen.add(num)
If the number is not in seen, add it
6️⃣ Print Result
print(duplicates)
▶️ Output
{1, 2}
🔑 Key Concepts Used
Lists
Sets (set())
Loop (for)
Conditional statements (if-else)
⏱️ Time Complexity

O(n)

Each element is checked once
🚀 Why Use Set?
Sets store unique values only
Fast lookup (O(1) average time)
Automatically avoids duplicates
⚠️ Note

Output is a set, so order may not be the same:

{1, 2} or {2, 1}
🚀 Alternative (Simple Method)
lst = [1, 2, 3, 2, 4, 1]
duplicates = [x for x in lst if lst.count(x) > 1]

print(set(duplicates))
📚 Learning Outcome

After understanding this program, you will learn:

How to detect duplicates in a list
How sets help in solving problems efficiently
How to use loops and conditions together

<img width="520" height="796" alt="image" src="https://github.com/user-attachments/assets/8f4ccab5-af0a-44e4-9cff-e606c99b8743" />
