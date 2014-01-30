# Meniga's Legolize Less/Css framework

_Q: What is Legolize?_

--- Legolize is a LESS framework built up on BEM methodology inspired by the SUIT framework.


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

#### For functionality specific classes (describes functionality)

	fn-MyFunction
	or
	fn-myFunction

_Q: When do we want to use fn- vs ui-?_

###### Example:

	fn-TransactionTable

---

#### For angular specific classes (directives)

	dir-MyDirective
	or
	dir-myDirective

###### Example:

	dir-CategoryTree

---

### Random thoughts

_Q: Where do we want to write page specific overrides for Lego's whether it's a modifier, descendant or whatever, in the customized lego css file itself or in a page css or where?_


###### Example:

	// Standard
	.ListGroup-item{
		border: 1px solid #000;
	}

	// Budget page
	.ListGroup-item{
		border: none;
	}


---

### Brainstorm from the Mooverang project

_Before:_

	<div class="budget-row-directive list-group-item">
    	<div class="content-container list-item-row">
        	<section class="item-title-container">
            	<h2 class="h4 text-upper">{{ title }}</h2>
    	    </section>
        	<section class="item-info-container">
            	<h3>{{ amount }}</h3>
	        </section>
    	</div>
	</div>




_After: Not perfect but..._

	<div class="dir-BudgetBar ListGroup-item">
    	<div class="ListGroup-itemRow ui-contentContainer">
        	<section class="ui-itemPrimaryContainer">
            	<h2 class="ListGroup-heading Heading--size4 u-textUpper">{{ title }}</h2>
	        </section>
    	    <section class="ui-itemSecondaryContainer">
        	    <h3>{{ amount }}</h3>
	        </section>
    	</div>
	</div>
