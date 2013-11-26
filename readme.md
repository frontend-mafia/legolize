# Legolize Less/Css framework

### SUIT defaults

	u-utilityName
	ComponentName
	ComponentName--modifierName
	ComponentName-descendantName
	ComponentName.is-stateOfComponent
	v1-*
	js-someName
		
_Q: What defines a utility?_

---

# Meniga add-ons

#### General layout classes
	ui-LayoutArea
	ui-layoutArea

_Q: Lowercase or uppercase?_

_Q: What defines a layout class (ui-)?_

_Q: Is a layout a component or is it like a utility? (PascalCase vs camelCase)_

###### Example:

	ui-pageNav
		ui-pageNav--someModifier

	ui-pageNav-descendantName

	ui-pageNav.is-stateOf

---

#### For angular specific classes (directives)

	dir-MyDirective
	or
	dir-myDirective

###### Example:

	dir-CategoryTree

---

#### For functionality specific classes (describes functionality)

	fn-MyFunction
	or
	fn-myFunction

_Q: When do we want to use fn- vs ui-?_

###### Example:

	fn-TransactionTable

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
            	<h2 class="Heading--size4 u-textUpper">{{ title }}</h2>
	        </section>
    	    <section class="ui-itemSecondary-Container">
        	    <h3>{{ amount }}</h3>
	        </section>
    	</div>
	</div>
