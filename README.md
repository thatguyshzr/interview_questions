# Interview Questions
List of questions I've been asked during interviews. They usually ask about projects in my resume, but here are questions that apply to everyone.

* [Python](#python)
* [Flask](#flask)
* [SQL](#sql)
* [Machine Learning](#machine-learning)
* [Deep Learning](#deep-learning)
* [GenAI](#genai)

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

13) How to find missing values in a dataset?

14) Sort e_list based on age.
```
    class Employee:
        def __init__(self, name, age):
            self.age= age
            self.name= name
            
    e_list= [Employee('a', 25),
            Employee('b', 22),
            Employee('c', 26),
            Employee('d', 21),
            Employee('e', 20)]
```
A14.
```
    sorted_e_list = sorted(e_list, key=lambda employee: employee.age)

    for employee in sorted_e_list:
        print(f"Name: {employee.name}, Age: {employee.age}")
```

15) Write a function to sort this list with minimum number of swaps: a= [10, 3, 1, 6, 7, 2]
```
def func(l):
    sor= list(set(a))  # create a sorted list to compare nos
    
    while l!=sor:    # keep sorting each element until list is same as sorted list
        for i in range(len(sor)):
            if l[0]==sor[i]:
                position= i
                break

        l[0], l[i]= l[i], l[0]
    
    return l
```

----------------------------------
## Flask
1) What is cacheing in flask?

2) What are HTTP methods?

- GET, POST, PUT, PATCH, DELETE

3) Difference between POST and PUT?

4) What are sessions?

5) How to create API with flask?

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
## Machine Learning
1) What are the advantages of Decision Tree/Random forest?

2) Linrear regression for feature importance.

3) What are the assumptions of a linear regressions?

4) What is supervised and unsupervised learning?

5) Examples of clustering?

6) What is cross validation?

7) Why Use Ensemble Learning?

8) Difference between recall and precision.
- Precision: when the model predicts, how often does it predict correctly.
- Recall: does the model predict everytime it should have.

9) What are the parameters of random forest?
- 3 mains parameters are:
- - <u>n_estimators</u>- number of trees in the forest
- - <u>max_features</u>- number of features to consider when looking for the best split
- - <u>max_depth</u>- maximum depth of the tree

10) To get better result from your ML model, what can you do?
- Change the parameters of the model or add more data.\
Changing parameters is a better option since adding more data with bad parameters means data doesn't get trained in the best way.\
(There are more methods to improve a model but this answer was relevant to the project in my resume.)

11) How to deal with imbalanced data?

12) What are Regularization techniques. What are L1 and L2 regularization?

13) How to fix overfitting?

14) Ways to detect outliers?

15) What is gradient descent?

16) Feature reduction steps?

17) What is stationarity in time series?

18) What are (p,d,q) in arima model?

19) What is F1 score and why is it called so?

20) Difference between parameters and hyper-parameters?

----------------------------------
## Deep Learning
1) What is the last layer of a yolo model?
- For any neural network, the last layer will be a dense layer with number of nodes = number of classes to detect.

2) Yolo structure.

3) What is CNN (convolution neural network)? CNN architecture.

4) What are anchor points in yolo?

5) Does yolo structure has maxpooling?

6) How to augment images?

7) What are better ways to label augmented data?

8) What are checkpoints in tensorflow yolo?

9) Can shapley be used for DNN?

10) What are epochs? How to decide number of epochs?

11) What is the structure of LSTM?

12) In LSTM, what is gradient clipping and gradient explosion?

13) Resnet (residual network) architecture?

14) What makes YOLO faster than other models?

15) Segment Anything Model (SAM)

16) Why are activation functions used?

17) Why is CNN used for images as opposed to text or numeric data?

----------------------------------
## GenAI
1) What are the concepts of GenAI?

2) What are RAG (retrieval augmentated generation) models?

3) IP adaptors.

4) Few shot or zero shot models.

5) CLIP.

6) VLM (visual language models).

7) Semantic search.

8) How to evaluate a LLM model?
- One way is to use RAGAS
