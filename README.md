# Interview Questions
List of questions I've been asked during interviews. They usually ask about projects in my resume, but here are questions that apply to everyone.

----------------------------------
## Python
- What are different data structures in python?

List, tuple, set, dictionary, dataframes (if using pandas), arrays (if using numpy)

- Can we have dictionary like this ```d= {1:'a', True:'q', 1.2:'asd'}```

Yes

- What is the different between list and tuple?

Elements of lists can be changed, tuples cannot.

- How to get last element of a list?

```my_list[-1]```


- Is python object oriented language or procedure oriented?

- What will be the output of this?
```python
def product(a,b):
    return a*b

def product(a,b,c):
    return a,b,c

print(product(2,3))
```
Since the function name is same, python will consider the later one and throw an error because it expects 3 arguments but only 2 are given.

- What is deep and shallow copy?

- What is faster, list or tuple?

- What are local and global variables?

- What are OOP concepts in python?

Encapsulation- This puts restrictions on accessing variables and methods directly and can prevent the accidental modification of data.

Abstraction- Hides code.

Polymorphism- Python allows different classes to have methods with the same name.

Inheritance- capability of one class to derive or inherit the properties from another class)

----------------------------------
## Flask
- When would you use flask and when django?

- What is cacheing in flask?

- What are HTTP methods?

GET, POST, PUT, PATCH, DELETE

- Difference between POST and PUT?

- What are sessions?

----------------------------------
## SQL
(Python developer)
- What will be the output of this?
```
select * from subject_name, AVG(marks) from table_name
where AVG(marks) > 75
GROUPBY subject_name
```

- How to get unique values from a table?

Using "distinct" keyword.

- How to remove repeating values from table?

- What is index?

- What is deadlock?

- What are primary and foreign key?

----------------------------------
## Data Science
- What are the advantages of Decision Tree/Random forest?

- What is the last layer of a yolo model?

For any neural network, the last layer will be a dense layer with number of nodes = number of classes to detect.

- What are the assumptions of a linear regressions?

- What is supervised and unsupervised learning?

- Examples of clustering?

- What is cross validation?

