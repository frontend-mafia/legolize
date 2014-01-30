# Meniga's Legolize Less/Css framework

_Q: What is Legolize?_

Legolize is a LESS framework built up on BEM methodology inspired by the SUIT framework.


### SUIT defaults

	u-utilityName
	ComponentName
	ComponentName--modifierName
	ComponentName-descendantName
	ComponentName.is-stateOfComponent
	v1-*
	js-someName

[SUIT on GitHub](https://github.com/suitcss/suit/tree/master/doc)

---

# Legolize improvements on SUIT

We have defined the following types for improvements

* Layout classes
* Function classes
* Angular directives classes


#### Layout classes

	ui-Page
	ui-PageHeader
	ui-PageNav
	ui-PageFooter

	ui-Section
	ui-Section-content
	ui-Section-container


_Q: What defines a layout class (ui-)?_

It's a class used for commonly used layout classes.

###### Example:

#### Functionality specific classes

	fn-MyFunction
	fn-TransactionTable
	fn-SearchForm

---

#### For AngularJs directives

	dir-SomeDirective
	dir-CategoryTree
	dir-TransactionRow

---

#### Choosing names for classes

_Q: What do I have to think about when writing class names?_

* All LEGO's should be named singular?

Example:

	Correct: .Button
	Wrong: .Buttons

* We should try to name the class to describe the visual reference to the object but not it's functionality

Example:

	Correct: .Button--panel
	Wrong: Button--save


