SUIT defaults
------------------------------------------------


u-utilityName
ComponentName
ComponentName--modifierName
ComponentName-descendantName
ComponentName.is-stateOfComponent
v1-*
js-someName


- What defines a utility?


Meniga add-ons
------------------------------------------------


/********** For layout specific classes **********/
ui-LayoutArea
	or
ui-layoutArea

- What defines a layout class (ui-)?
- Is a layout a component or is it like a utility? (PascalCase vs camelCase)

Example:

ui-pageNav
	ui-pageNav--someModifier

ui-pageNav-descendantName

ui-pageNav.is-stateOf


/********** For angular specific classes (directives) **********/
dir-MyDirective
	or
dir-myDirective

Example:

dir-CategoryTree

/********** For functionality specific classes (describes functionality) **********/
fn-MyFunction
	or
fn-myFunction

- When do we want to use fn- vs ui-?

Example:

fn-TransactionTable


-------------------------
Brainstorm from the Mooverang project

Before:
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

After:
Not perfect but...

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