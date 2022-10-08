# CloudFormation - TEMPLATE (the "Blueprint")

> text file that is an input into CloudFormation

## Anatomy

- formats
	- JSON
	- YML

```js
    "AWSTemplateFormatVersion": "version date", // only 1 valid value as of now
    "Description": "JSON string", 
    "Metadata": { template metadata }, 
    "Parameters": { set of parameters }, 
    "Mappings": , 
    "Conditions": , 
    "Transform": , 
    "Resources": , // REQUIRED
    "Outputs": 

```


### Resources

```yml
{
    "Resources": {
        "Logical ID": { # reference resource in OTHER parts of the TEMPLATE
            "Type": "Resource type",
            "Properties": {...}
        }
    }
}
```

-----

- Nested Templates