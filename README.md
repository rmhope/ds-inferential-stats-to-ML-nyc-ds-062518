

```python
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```

## Inferential Statistics to [Supervised] Machine Learning
As we've seen, we can use sampling techniques and descriptive statistics to learn more about a population. While the overall population itself will undoubtedly differ to some degree from that of our sample, we can quantify the likelihood and scale of the population's differences from the sample across various dimensions or statistical measures. For example, if modelling a dataset that is approximately a normal distribution, we would start by computing the mean and variance for our sample and we could then calculate confidence intervals for those respective measures of the overall population. 

Supervised machine learning applies these same concepts along with additional algorithms in order to mine structure within the data to make predictive models. This always begins with splitting the data into train and test sets so that we can validate our model performance. This process is analagous to if we took multiple samples from a population; assuming our samples are independent and of a sufficient size, we should expect that descriptive measures such as the mean and standard deviation of those samples should be roughly equivalent. Similarly in machine learning, we will train our algorithm to detect and model patterns in the training set. This is typically a random sample of roughly 75% - 80% of the total data available to us. After training a model on this set of data, we can then further test the validity of our model against the remaining hold-out data which (again typically 20-25% of the original data) we intentionally did not train the model on. As you probably have put together, this second hold-out dataset of those observations that we not included in the training is known as the test set.

Implementing a **train-test split** in python is very straightforward using sklearn's built in method. Let's take a look at this in more detail. We start by importing a dataset and choosing X and y values. This is a standard process for all **supervised machine learning** algorithms. A supervised learning algorithm is one in which we feed input examples (X, via the training set) into a model which then attempts to reproduce appropriate output values (Y) associated with those inputs. This can take many forms including regression problems such as, "if I give you a person's height, age, weight, blood pressure, etc. cholestoral level",  to classification problems such as "if I give you details about a plant including color, stem length, and root structure, predict what species it is" or even text processing such as "if I give you a reviewers comments, predict how positive/negative their viewpoint is". All of these problems can initially be formulated as an input output mapping where we are trying to generalize a formula from one space X, to another space y.


```python
#As usual we begin by importing our dataset
import pandas as pd

df = pd.read_csv('')
print('Length of Dataset: ', len(df))
print('Column Names:\n', df.columns)
```


```python
#Define X and y
X = df[]
y = 
```

### Train Test Split


```python
from sklearn.model_selection import train_test_split
```


```python
pwd
```




    '/Users/matthew.mitchell/Documents/Learn_CO/Data_Science_Skills/Inferential_Stats_to_ML_Overview'


