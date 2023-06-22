# machine-learning-crash-course-google-developer
## Jupyter notebook files contain my solutions for programming exercise of Machine Learning Crash Course Google
### First Step With Tensorflow

| files | Description |
| --- | --- |
| [programming_exercise_1_numpy_ultraquick_tutorial.ipynb](first-step-with-tensor-flow/programming_exercise_1_numpy_ultraquick_tutorial.ipynb) | Quick tour go through numpy `np.arrange()` `np.random.randint()`|
| [programming_exercise_2_pandas_dataframe_ultraquick_tutorial.ipynb](programming_exercise_2_pandas_dataframe_ultraquick_tutorial.ipynb) |  Quick tour go through pandas dataframe `pd.DataFrame(data=df_data, columns=df_column_names)`|
| [programming_exercise_3_linear_regression_with_synthetic_data.ipynb](first-step-with-tensor-flow/programming_exercise_3_linear_regression_with_synthetic_data.ipynb) | Hyperparams tuning with synthetic dataset: `learning_rate`, `epochs`, `batch_size` |
| [programming_exercise_4_linear_regression_with_a_real_dataset.ipynb](first-step-with-tensor-flow/programming_exercise_4_linear_regression_with_a_real_dataset.ipynb) | Make prediction from trained model, find out correlated features with `median_house_value` for **linear regression** problem|

**@take_aways**:
- One `iteration` include one loop of  `forward` and `backward` that ended up updating params after passing through one batch of data. 
- One `epoch` consists `iteration_nums` that passing `entire_dataset` one time. 
- `learning_rate` indicate the rate of increase or decrease params value in one iteration.
- `iteration_nums` = `entire_dataset_size`/`batch_size`

### Validation

| files | Description |
| --- | --- |
| [programming_exercise_5_validation_and_test_sets.ipynb](validation/programming_exercise_5_validation_and_test_sets.ipynb) |Determine why loss curve of training and validation differ, as such, we need to shuffle training set before split data|

**@take_aways**:
- Need to randomize the dataset before split training and validation
- If the `validation_split` ratio is below 0.15 the model has a high change of overfitting since we do not have enough validation examples to feedback to the model
- High `validation_split` is good, however, need to balance the `training_examples`to the point that enough for getting the reach of underfitting
- `validation_split` ratio should be around 0.2
