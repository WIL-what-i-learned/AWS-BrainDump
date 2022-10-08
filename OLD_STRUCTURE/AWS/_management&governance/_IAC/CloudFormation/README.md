# Cloud Formation
_competitors: terraform, chef, puppet_

> AWS DECLARATIVE Infrastructure Provisioning Tool (Infrastructure as Code: IAC)  
> repeatable process for provisioning resources

- 💰 Using Cloud Formation is free but you pay for the resources you provision

## Pro / Con

- Pro
	- no resource is manually created
		- less human risk
	- the code can be version controlled
		- infrastructure changes are reviewed through code
	- only 'deploying engineer' has access to the main VPC deployment file but lower departments can own theirs

- Con
	- learning curve


### Stacks

> a provisioned instance of the template | = "stack" CloudFormation(InputConfigYml) 

### Change Set

> shows how the potential changes will place your running resources

1. Create
2. View
3. Execute
4. Delete

-----



- separation of concerns 👉 can create many stacks for many apps, and many layers
	- VPC stacks
	- Network stacks
	- App Stacks

- steps
	- templates are uploaded to S3
	- updating
		- can't edit an old template 👉 must upload a new version
	- deleting
		- deleting a stack delete every artifact that was created by CloudFormation

- building blocks
	- Resources 👉 your AWS resources declared in the template (MANDATORY)
	- Parameters 👉 dynamic inputs for your template
	- Mappings 👉 the static variables for your template
	- Outputs 👉 refers to what has been created
	- Conditionals 👉 list of conditionals to perform resource creation
	- Metadata

- cost
	- each resource within the stack is tagged with an identifier so you can easily see how much a stack costs you
	- can estimate costs of your resources using the CloudFormation template
	- savings strategy
		- in DEV - you could automate deletion of templates at 5PM and recreated at 8AM safely

- don't reinvent the wheel
	- leverage existing templates on the web
	- leverage documentation



## Rollbacks

- Stack Fails
	- DEFAULT: everything rolls back (gets deleted) 👉 can look at log
	- option to disable rollback and troubleshoot what happened

- Stack Update Fails
	- stack automatically rolls back to the previous known working state
	- can see the log of what happened in error message