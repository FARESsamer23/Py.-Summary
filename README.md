<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
   
</head>
<body>

<h1>Python Concepts and Examples</h1>
<p>This repository contains examples of various core concepts in Python programming. Each section includes code snippets demonstrating specific topics.</p>

<h2>1. Core Python Concepts</h2>

<h3>Data Types</h3>
<pre><code># Example of different data types
string_example = "Hello, World!"
list_example = [1, 2, 3, 4]
tuple_example = (1, 2, 3)
dict_example = {"name": "Alice", "age": 30}
set_example = {1, 2, 3}
</code></pre>

<h3>Control Structures</h3>
<pre><code># If statement
number = 10
if number > 0:
    print("Positive number")
else:
    print("Negative number or zero")

# Loop example
for i in range(5):
    print(i)
</code></pre>

<h3>Functions and Modules</h3>
<pre><code># Function definition
def greet(name):
    return f"Hello, {name}!"

# Using the function
print(greet("Alice"))
</code></pre>

<h3>Exception Handling</h3>
<pre><code># Exception handling example
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
</code></pre>

<h2>2. Object-Oriented Programming</h2>

<h3>Classes and Objects</h3>
<pre><code>class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        return f"{self.name} says Woof!"

# Creating an object
my_dog = Dog("Buddy")
print(my_dog.bark())
</code></pre>

<h2>3. Data Structures and Algorithms</h2>

<h3>Basic Algorithm (Sorting)</h3>
<pre><code># Sorting a list
numbers = [5, 2, 9, 1]
numbers.sort()  # In-place sorting
print(numbers)  # Output: [1, 2, 5, 9]
</code></pre>

<h2>4. Libraries and Frameworks</h2>

<h3>Using Pandas</h3>
<pre><code>import pandas as pd

# Creating a DataFrame
data = {'Name': ['Alice', 'Bob'], 'Age': [25, 30]}
df = pd.DataFrame(data)
print(df)
</code></pre>

<h2>5. Database Interaction</h2>

<h3>Using SQLite</h3>
<pre><code>import sqlite3

# Connecting to a database
conn = sqlite3.connect('example.db')
cursor = conn.cursor()

# Creating a table
cursor.execute('''CREATE TABLE users (id INTEGER PRIMARY KEY, name TEXT)''')

# Inserting data
cursor.execute("INSERT INTO users (name) VALUES ('Alice')")
conn.commit()

# Querying data
cursor.execute("SELECT * FROM users")
print(cursor.fetchall())

# Closing the connection
conn.close()
</code></pre>

<h2>6. Testing and Debugging</h2>

<h3>Unit Test Example</h3>
<pre><code>import unittest

def add(a, b):
    return a + b

class TestMathFunctions(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(2, 3), 5)

if __name__ == '__main__':
    unittest.main()
</code></pre>

<h2>7. Version Control</h2>

<h3>Basic Git Commands</h3>
<pre><code># Initialize a Git repository
git init

# Add files to staging
git add .

# Commit changes
git commit -m "Initial commit"

# Check status
git status
</code></pre>

<h2>8. Development Tools</h2>

<h3>Creating a Virtual Environment</h3>
<pre><code># Create a virtual environment
python -m venv myenv

# Activate the virtual environment
# On Windows
myenv\Scripts\activate
# On macOS/Linux
source myenv/bin/activate
</code></pre>

<h2>9. Basic Understanding of Web Development</h2>

<h3>Flask Basic Web App</h3>
<pre><code>from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Welcome to my web app!"

if __name__ == '__main__':
    app.run(debug=True)
</code></pre>

</body>
</html>
