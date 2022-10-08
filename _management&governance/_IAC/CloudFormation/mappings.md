# Mappings

> use an input value to determine another value

1. Define Mappings w/ key value pairs
2. use `FN::FindInMap` Mapping

- fixed (hardcoded) variable within CloudFormation Template
- used to differentiate between different environment groups / regions / AMI types
- EX: `Region Map`
	```yml
	Mappings:
		RegionMap:
			us-east-1:
				"32" : "ami-#####"
				"64" : "ami-#####"
			us-west-1:
				"32" : "ami-#####"
				"64" : "ami-#####"
	```
- access a mapped value with the `FindInMap` function
	- `!FindInMap` 👉 returns a names value from a specific key