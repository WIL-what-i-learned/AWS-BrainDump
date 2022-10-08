# Intrinsic Functions

> build in functions that help you manage your stack

	- `Ref`
		- `!Ref`
		- Parameters 👉 returns the value of a parameter
		- Resources 👉 returns the physical ID of the underlying resource
	- `Fn::GetAtt`
		- get specific attribute that is attached to a resource
	- `Fn::FindInMap`
		- returns value for a specific map key
	- `Fn::ImportValue`
		- import values that are exported in other templates
	- `Fn::Join`
		- joins value w/ delimited
	- `Fn::Sub`
		- substitute variables values into variables
	- Condition Functions
		- `Fn::And`
		- `Fn::Equals`
		- `Fn::If`
		- `Fn::Not`
		- `Fn::Or`
