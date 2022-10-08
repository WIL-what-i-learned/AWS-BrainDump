# Parameters

> a way to provide inputs to your CloudFormation template

- needed to reuse template across the company 👉 some inputs can not be determined ahead of time
- use when your answer to `is this CloudFormation resource configuration likely to change in the future` is YES
- `!Ref` references parameters


## Param Settings

- type
	- string
	- number
	- comma delimited list
	- List<Type>
	- AWS Parameter (to help catch invalid values - match again existing values in the AWS Account)

- description
- constraints
- constraint description
- Min / Max Length
- Min / Max Value
- Defaults
- AllowedValues (Array)
- AllowedPattern (regexp)

