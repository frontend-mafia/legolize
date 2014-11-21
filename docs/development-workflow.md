# Development workflow

When working on Legolize we have two workflows, one is for developing and reviewing, and the other is for bower versioning.

## Developing Legolize

1. Always work on a specific branch related to your LEGO

        $ git checkout -b lego/legoname
    
2. When done and pushed, create a pull request, and add reviewers to review changes before you merge to master.

        [https://github.com/frontend-mafia/legolize/pulls](https://github.com/frontend-mafia/legolize/pulls)
    
3. After code review, you can merge to master 

## Releasing a version

Once we have stable version on master we update the version using Bower.

1. Be sure you are working on master

        $ git checkout master

2. Fetch from the remote to get all tags.

    	$ git fetch master	

3. Run bower command to change the version number ( v Major.Minor.Patch )

        $ bower version patch (adds a new version to the last version number) 
        $ bower version minor (adds a new version to the middle version number) 
        $ bower version major (adds a new version to the first version number)

3. Push all changes to master including tags

        $ git push --tags

