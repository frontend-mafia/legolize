# Legolize LESS framework

Legolize is a LESS framework built up on BEM methodology inspired by the [SUIT Framework](https://github.com/suitcss/suit/).

This is the core project where all default Lego's are defined.

To get a scaffolding project that uses this, go to [legolize-base](https://bitbucket.org/meniga/legolize-base) and [legolize-legos](https://bitbucket.org/meniga/legolize-legos)


## Quick start

Two quick start options are available:

- Clone the repo: 

    	via https    
      	$ git clone https://YOUR-USERNAME@bitbucket.org/meniga/legolize.git    
    
      	or
    
      	via ssh    
      	$ git clone https://YOUR-USERNAME@bitbucket.org/meniga/legolize.git

   	
- Install with [Bower](http://bower.io): 
    
        $ bower install legolize. (not implemented yet)


### Naming convention

	u-utilityName
	ComponentName
	ComponentName--modifierName
	ComponentName-descendantName
	ComponentName.is-stateOfComponent
	v1-*
	js-someName
	ui-LayoutComponentName
	fn-FunctionalComponentName
	


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

#### Functionality specific classes

	fn-MyFunction
	fn-TransactionTable
	fn-SearchForm

---

#### Choosing names for classes

_Q: What do I have to think about when writing class names?_

###### All LEGO's should be named singular.

Example:

	Correct: .Button
	Wrong:   .Buttons

###### It might be a good idea to name the classes to describe the visual reference to the object but not it's functionality

Example:

	Correct: .Button--panel
	Wrong: Button--save


