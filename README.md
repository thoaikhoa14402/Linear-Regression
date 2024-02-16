# Linear-Regression
Data fitting using linear regression

1. Building a model for *predicting average lifespan* **using linear regression**.

- Requirement 1a: Utilize all 10 features provided in the assignment
	- Train only once for all 10 features on the entire training dataset (`train.csv`)
	- Express the formula for the linear regression model (predicting $y$ based on 10 features in $X$)
	- Report **one result on the test set (`test.csv`)** for the trained model
    
- Requirement 1b: Construct a model using only 1 feature, find the best-performing model for the optimal outcome
	- Test on the entire set of provided 10 features
	- Requirement: Utilize the **5-fold Cross Validation method** to identify the best-performing features.
	- Report **10 corresponding results for 10 models** from 5-fold Cross Validation (take the average).
	
	<center>

	| NO. | Model with 1 feature    | RMSE |
	|:---:|:-----------------------:|:----:|
	|  1  | Adult Mortality         |      |
	|  2  | BMI                     |      |
	|     | ...                     |      |
	|  10 | Schooling               |      |

	</center>

	- Express the formula for the linear regression model with the best-performing feature (predicting $y$ based on the identified best feature)
    	- Report **one result on the test set (test.csv)** for the best-performing model found
	
- Requirement 1c: Construct a model, seeking the best-performing model for optimal results
	- Construct `m` different models (at least 3), each distinct from the models in 1a and 1b
		- Models can be a combination of 2 or more features
		- Models may use standardized or transformed features (squared, cubed, etc.)
		- Models can incorporate features generated from 2 or more different features (addition of 2 features, multiplication of 2 features, etc.)
		- ...
	- Requirement: **Utilize the 5-fold Cross Validation method** to identify the best-performing model
	- Report **`m` corresponding results `m` models** based on 5-fold Cross Validation (averaged)

	<center>

	| NO. |           Models           | RMSE |
	|:---:|:--------------------------:|:----:|
	|  1  | Using   2 features  (a, b) |      |
	| ... | ...                        |      |
	|  m  | ...                        |      |

	</center>

	- Express the formula for the best-performing regression model that the student identified
	- Report **one result on the test set (test.csv)** for the best-performing model found.

- <ins>NOTE:</ins>
    - The test.csv dataset is only to be used three times, as mentioned earlier.
    - The reported result is a measurement [RMSE](https://www.sciencedirect.com/topics/engineering/root-mean-squared-error)
    

2. Report on the results, evaluate, and provide comments on the constructed models (3 points)
    - The report should include personal information (full name, student ID), page count, and references (specifying the documents used for each part of the assignment)
    - List ALL libraries used and the reasons for their utilization
    - Enumerate ALL functions used and describe each of them
    - Report and provide feedback on the results from ALL constructed models (with $1 + (10 + 1) + (m + 1)$ results)
    - With requirements 1b and 1c: explain or state hypotheses for the model that achieved the best result.
    - With requirement 1c: explain the reasons for selecting/designing features for the `m` models.
