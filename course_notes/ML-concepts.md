# machine-learning-crash-course-google-developer
## ML Concepts
### Framing
Key ML Terminology
| Terminology | Description |
| --- | --- |
| `classification model` | the output of the classification model should be **categorical values** |
| `example` | one **single data record** to feed into the model whether for training, validating, or testing |
| `feature` | **numeric values** to describle many characteristics of data. For example: Book Data: pages_of_book(100, 200, or 300), published_date(20230623), etc |
| `inference` | the action of passing unseen example from **test data** to trained model to produce the output |
| `label` | the actual **ground truth** of input data example on training set |
| `model` | the **algorithm** to learning **pattern** from data, the model can be implemented in any programming language |
| `regression model` | the output of the regression model should be **continuous number values** |
| `training` | the practice of feeding **training data** to model then **update the parameters** of models over series of **iteration** |


### Descending into ML

Linear Regression `y=mx+b`

| Terminology | Description |
| --- | --- |
| `bias` | In the formula `y=mx+b`: `b` is the **bias** term which indicates the value of the model when every weights values are zeros |
| `inference` | Inference is the practice of feeding unseen data into a **trained model** to calculate the output |
| `linear regression` | Machine Learning model which learns the pattern from the input data and then predicts **floating point number**. The input features dimension is two |
| `weight` | Set of **parameters** resulted from training the model, these **weights** then multiplying with features for inference  |
