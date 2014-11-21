# Naming convention & terminology

We follow a BEM naming convention inspired by the [SUIT CSS](https://github.com/suitcss/suit) framework.


## Lego

A Lego is a UI component that serves a single responsibility and is always the same no matter where you use it.

Naming convention: PascalCasing 

example:

	.ListGroup {...}


### All Lego's should be named in a singular fashion:

	.Button		= Correct
	.Buttons	= Wrong


Always name the css classes by describing the **visual reference** to the object but not it's functionality since you might want to use the Lego's elsewhere where it doesn't make sense to have the functionality name.

Example:

	.Button--primary 	= Correct
	.Button--search 	= Wrong


## Modifier
	
A Modifier is a modification on the Core Lego, like making a color change for example.
	
Naming convention:  double dash and a camelCased name.

Example:

	.Panel--someModifier { ... }

## Descendant

A descendant is a child object of a Lego

Naming convention: single dash and a camelCased name.

Example:
	
	.Panel-header {...}

## State
	
State classes are used to describe a display state of the component.

Naming convention:  Starts with a boolean term with a single dash and a camelCased name.

Example:

	.is-active {...}

## Utility
	
Utility classes are used for a specific layout behaviour that's always going go overwrite the objects state or layout behaviour using the !important keyword

Naming conventions: Starts with u- and a camelCased name.

Example:

	.u-pullLeft { float: left !important; }


## Functional
	
Functional classes are used when you need to style a specific Lego component and it doesn't make sense to create a modifier for it because it's only used in that location.

Naming conventions: Starts with fn- and the type of the object and a name using pascalCase.

Example:

	.fn-buttonSearch {...}

## Javascript hook

Javascript classes are used to when you need to hook some javascript event to that element and distinguish from the other classes that control the UI.

Naming convention: Starts with js- and a camelCased name.

Example:

	.js-buttonSearch

	
## Variables

Variable names also have naming conventions

Here is how you define variables:

    @legoName-cssProperty    
    @legoName--modifierName-cssProperty
    @legoName--modifierName-descendandName-cssProperty
	
Examples:

    @button-borderColor: #333;
    @button--primary-borderColor: #333;
    @listGroup--item-backgroundColor: #fff;
   