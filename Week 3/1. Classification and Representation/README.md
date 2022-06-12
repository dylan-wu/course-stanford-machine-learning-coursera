How do we attempt classification?
- Use linear regression and map all predictions greater than $0.5$ as $1$ and all less than $0.5$ as $0$
	- This method doesn't work well because classification is not a linear function
- Similar to the regression problem, except that avlues we now want to predict have a small number of discrete values.

What is the binary classification problem?
- $y$ can only take two values, $0$ and $1$

What is a sigmoid function?
- Also called a logistic function
- 