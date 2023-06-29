# machine-learning-crash-course-google-developer
## ML Concepts
### 1. Framing
#### Key ML Terminology
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


### 2. Descending into ML

#### Linear Regression `y=mx+b`

| Terminology | Description |
| --- | --- |
| `bias` | in the formula `y=mx+b`: `b` is the **bias** term which indicates the value of the model when every weights values are zeros |
| `inference` | inference is the practice of feeding unseen data into a **trained model** to calculate the output |
| `linear regression` | machine Learning model which learns the pattern from the input data and then predicts **floating point number**. The input features dimension is two |
| `weight` | set of **parameters** resulted from training the model, these **weights** then multiplying with features for inference  |

#### Training and Loss

| Terminology | Description |
| --- | --- |
| `empirical risk minimization` | choosing a function that minimizes loss manually, contrast to **structural risk minimization**  |
| `loss` | **loss** is the value that we try to minimize when learning, the loss value is calculated at the end of  the **forward** pass of the **training**|
| `mean squared error` | this is one kind of **loss function** used mostly for **linear regression** problems and **mean squared error = squared loss/number of examples** |
| `squared loss` | one kind of **loss function** used mostly for **regression** problems|
| `training` | the practice of updating model weights that minimize **loss** to learning the patterns from the training data set |


### 3. Reducing Loss

#### An interactive approach
| Terminology | Description |
| --- | --- |
| `convergence` | is the state in the training process when the **training loss** and the **accuracy** are not improved after iterations  |

#### Gradient Descent
| Terminology | Description |
| --- | --- |
| `gradient descent` | the algorithm to find the best params to **minimize loss** through gradually tiny steps of updating parameters |
| `step` | one single iteration to update parameters after **forward** and **backward** which passes one training batch|

#### Learning Rate
| Terminology | Description |
| --- | --- |
| `hyperparameter` | these parameters are not learned by the ML algorithm itself but can be **tuned** and **chosen** by the ML engineer to optimize the loss function |
| `learning rate` | one of hyperparameters (floating point number) that define the rate at which we update the **weight (bias)** in the **backward step**, the learning rate multiplied by the **gradient** then plus with current *weight (bias)** values to calculate the **new weight(bias)** values|
| `step size` | one synonym of the **learning rate**, some time this two-term can be used interchange|


#### Optimize Learning Rate
| Terminology | Description |
| --- | --- |
| `hyperparameter` | these parameters are not learned by the ML algorithm itself but can be **tuned** and **chosen** by the ML engineer to optimize the loss function |
| `learning rate` | one of hyperparameters (floating point number) that define the rate at which we update the **weight (bias)** in the **backward step**, the learning rate multiplied by the **gradient** then plus with current *weight (bias)** values to calculate the **new weight(bias)** values. If the learning rate is too small, it will take a lot of time to get **convergence**, in contrast, if the learning rate is too large the model will never **converge**, appropriate learning help model learning fast and efficient |
| `step size` | one synonym of the **learning rate**, some time this two-term can be used interchange|


#### Stochastic Gradient Descent
| Terminology | Description |
| --- | --- |
| `batch` | describe set of training examples passing through model in one single iteration |
| `batch size` | number of training **examples** in one **batch**. For example: if **batch_size=50** we process 50 data examples in one **iteration** |
| `mini-batch` | describe practice to pass a **batch** of randomly traininig examples with **batch size** greater than 10 and smaller than 1000 to model in one **iteration** |
| `Stochastic Gradient Descent(SGD)` | describe practice to pass a **batch** with batch size equal 1 to model |
