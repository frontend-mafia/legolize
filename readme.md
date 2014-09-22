# Legolize LESS framework

Legolize is a LESS framework built up on BEM methodology inspired by the [SUIT Framework](https://github.com/suitcss/suit/).

This is the core project where all default Lego's are defined.

To get a scaffolding project that uses this, go to [legolize-base](https://bitbucket.org/meniga/legolize-base) and [legolize-legos](https://bitbucket.org/meniga/legolize-legos)


## Quick start

Two quick start options are available:

- Clone the repo: 

    	via https    
        	$ git clone https://YOUR-USERNAME@bitbucket.org/meniga/legolize.git
        	     
        via ssh    
        	$ git clone git@bitbucket.org:meniga/legolize.git
    
  	
- Install with [Bower](http://bower.io): 
    
        $ bower install legolize. (not implemented yet)


---

## Naming convention

### Class names

	LegoName
	LegoName--modifierName
	LegoName-descendantName
	LegoName.is-stateOfLego
	v1-*
	js-someName
	ui-LayoutLegoName
	fn-legoNameFunctionalName
	u-utilityName

example:

    .fn-buttonSearch
	.u-pullRight
	
### Variable names

    @lego--modifier-descendand-property 
	
example:

    @button--primary-borderColor: #333;
    @listGroup-itemHeading-fontSize


---
	
## Examples

### Lego

    .Heading
    .Heading--one 
    
    .ListGroup-itemHeader
    .ListGroup-item.is-active


### Layout classes

Layout classes are different from standard Lego's, they are primary used to descibe a specific layout unit.
There are no Layout classes in this core project since they are not supposed to be used here.

This is just to demonstrate naming conventions.

	.ui-Page
	.ui-PageHeader
	.ui-PageNav
	.ui-PageFooter

	.ui-Section
	.ui-Section-content
	.ui-Section-container


### Choosing names for classes

_Q: What do I have to think about when writing class names?_

#### All LEGO's should be named in a singular fashion:

	.Button		= Correct
	.Buttons	= Wrong


It's also a good idea to name the classes by describing the visual reference to the object but not it's functionality since you might want to use the Lego's elsewhere where it doesn't make sense to have the functionality name.

Example:

	.Button--primary 	= Correct
	.Button--search 	= Wrong


