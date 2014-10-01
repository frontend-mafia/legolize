# Legolize LESS framework

Legolize is a LESS framework built up on BEM methodology inspired by the [SUIT Framework](https://github.com/suitcss/suit/).

This is the core project where all default Lego's are defined.

To get a scaffolding project that uses this, go to [legolize-base](https://bitbucket.org/meniga/legolize-base) and [legolize-legos](https://bitbucket.org/meniga/legolize-legos)


# How to install

Two quick start options are available:

- Clone the repo: 

    	via https    
        	$ git clone https://YOUR-USERNAME@bitbucket.org/meniga/legolize.git
        	     
        via ssh    
        	$ git clone git@bitbucket.org:meniga/legolize.git
    
  	
- Install with [Bower](http://bower.io): 
    
        $ bower install legolize ( only available privately for now  )


---

# Development workflow

When working on Legolize we have two workflows, one is for developing and reviewing, and the other is for bower versioning.

## Developing Legolize

1. Always work on a specific branch related to your LEGO

        $ git checkout -b lego/legoname
    
2. When done and pushed, create a pull request, and add reviewers to review changes before you merge to master

        [https://bitbucket.org/meniga/legolize/pull-requests](https://bitbucket.org/meniga/legolize/pull-requests)
    
3. After code review, you can merge to master 

## Releasing a bower version

Once we have stable version on master it's time to give it a version tag

1. Be sure you are working on master

        $ git checkout master

2. Run bower command to change the version number ( v Major.Minor.Patch )

        $ bower version patch (adds a new version to the last version number)
        $ bower version minor (adds a new version to the middle version number)
        $ bower version major (adds a new version to the first version number)

3. Push all changes to master including tags

        $ git push --tags

---

## Naming convention

This section is not 100% up to date since a few changes have been made, 

### Class names

	LegoName
	LegoName--modifierName
	LegoName-descendantName
	LegoName.is-stateOfLego
	u-utilityName
	fn-elementFunctionName
	js-someName


Examples:
   
    Button
    Button--primary
    ListGroup-item
    Nav-item.is-active	
    .u-pullRight
    .fn-buttonSearch
    .js-tabContent
	
### Variable names

    @legoName-cssProperty    
    @legoName--modifierName-cssProperty
    @legoName--modifierName-descendandName-cssProperty
	
Examples:

    @button-borderColor: #333;
    @button--primary-borderColor: #333;
    @listGroup--item-backgroundColor: #fff;
    


---
	
### Choosing names for classes

_Q: What do I have to think about when writing class names?_

#### All LEGO's should be named in a singular fashion:

	.Button		= Correct
	.Buttons	= Wrong


Always name the css classes by describing the **visual reference** to the object but not it's functionality since you might want to use the Lego's elsewhere where it doesn't make sense to have the functionality name.

Example:

	.Button--primary 	= Correct
	.Button--search 	= Wrong


If you want to have a **functionality reference**, just add the fn-elementFunctionName

Example: 

    .fn-buttonSearch