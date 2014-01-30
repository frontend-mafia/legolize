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
	ui-Section
	ui-Section-content

	ui-LayoutArea
	ui-layoutArea

	For page layout classes
	ui-Page
	ui-PageHeader
	ui-PageNav
	ui-PageFooter

_Q: What defines a layout class (ui-)?_

It's a class used for commonly used layout classes.

###### Example:

#### Functionality specific classes

	fn-MyFunction

###### Example:

	fn-TransactionTable

---

#### For angular specific classes (directives)

	dir-MyDirective

###### Example:

	dir-CategoryTree

---
