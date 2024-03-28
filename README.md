# Interview Questions
List of questions I've been asked during interviews. They usually ask about projects in my resume, but here are questions that apply to everyone.

If any answer is wrong or if there's a better way to answer it, create a pull request.

* [Python](#python)
* [Flask](#flask)
* [SQL](#sql)
* [Data Science](#data-science)

----------------------------------
## Python
1) What are different data structures in python?

- List, tuple, set, dictionary, dataframes (if using pandas), arrays (if using numpy)

2) Can we have dictionary like this ```d= {1:'a', True:'q', 1.2:'asd'}```
- Yes

3) What is the different between list and tuple?
- Elements of lists can be changed, tuples cannot.

4) How to get last element of a list?
- ```my_list[-1]```


5) Is python object oriented language or procedure oriented?

6) What will be the output of this?
```python
def product(a,b):
    return a*b

def product(a,b,c):
    return a,b,c

print(product(2,3))
```
- Since the function name is same, python will consider the later one and throw an error because it expects 3 arguments but only 2 are given.

7) What is deep and shallow copy?

8) What is faster, list or tuple?

- Tuple. List stores each element in vairable one by one, tuple stores the whole thing in one go.

9) What are local and global variables?

10) What are OOP concepts in python?

- <u>Encapsulation</u>- This puts restrictions on accessing variables and methods directly and can prevent the accidental modification of data.

- <u>Abstraction</u>- Hides code.

- <u>Polymorphism</u>- Python allows different classes to have methods with the same name.

- <u>Inheritance</u>- capability of one class to derive or inherit the properties from another class)

11) What will be the output of:
```
first= [1,2,3]
second= first
second.append(4)
print(first)
```
- [1,2,3,4] since both variable are stored in same memory location, updating one updates the other. To prevent this, do ```second= first.copy()```

12) Count the occurrence of each character in a string. Input = 'hello'. Output = h-1,e-1,l-2,o-1

----------------------------------
## Flask
1) What is cacheing in flask?

2) What are HTTP methods?

- GET, POST, PUT, PATCH, DELETE

3) Difference between POST and PUT?

4) What are sessions?

----------------------------------
## SQL
(Interviewing for Python developer or Data Scientist)
1) What will be the output of this?
```
select * from subject_name, AVG(marks) from table_name
where AVG(marks) > 75
GROUPBY subject_name
```

2) How to get unique values from a table?

- Using "distinct" keyword.

3) How to remove repeating values from table?

4) What is index?

5) What is deadlock?

6) What are primary and foreign key?

7) Group by vs order by
- <u>Group by</u> used to group the rows that have the same value. <u>Order by</u> sorts the result-set in ascending or descending order.

----------------------------------
## Data Science
1) What are the advantages of Decision Tree/Random forest?

2) What is the last layer of a yolo model?
- For any neural network, the last layer will be a dense layer with number of nodes = number of classes to detect.

3) What are the assumptions of a linear regressions?

4) What is supervised and unsupervised learning?

5) Examples of clustering?

6) What is cross validation?

7) Why Use Ensemble Learning?

8) Difference between recall and precision.

9) What are the parameters of random forest?
- 3 mains parameters are:
- - <u>n_estimators</u>- number of trees in the forest
- - <u>max_features</u>- number of features to consider when looking for the best split
- - <u>max_depth</u>- maximum depth of the tree

10) To get better result from your ML model, what can you do?
- Change the parameters of the model or add more data.\
Changing parameters is a better option since adding more data with bad parameters means data doesn't get trained in the best way.\
(There are more methods to improve a model but this answer was relevant to the project in my resume.)
