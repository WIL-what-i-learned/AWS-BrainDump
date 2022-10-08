# Conditions

> used to control the creation of resources or outputs based on a condition
- common
	- env (dev / prod / test)
	- AWS Region
	- any param value
- each condition can reference another condition parameter value or mapping
- create condition
	```yml
	Conditions:
		CreateProdResources: !Equals [ !Ref EnvType, prod ]
	```
- use condition
	```yml
	Resources:
		MountPoint:
			Type: "xxx"
			Condition: CreateProdResources
	```