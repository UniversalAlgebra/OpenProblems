# OpenProblems

This repository collects lists of open problems in universal algebra and related
areas. **Contributors welcome!**

If you would like to contribute and make additions or
revisions to the files in this repository, the best way is to
[fork](https://help.github.com/articles/fork-a-repo/)
the repo to your own GitHub account and then
submit a [pull request](https://help.github.com/articles/creating-a-pull-request/).

If you don't know what the last sentence means, don't worry---there are detailed
instructions below.  But if this all seems too complicated, feel free to simply
post a message on the
[Wiki pages](https://github.com/UniversalAlgebra/OpenProblems/wiki), or
[open a new issue](https://github.com/UniversalAlgebra/OpenProblems/issues), or
[send email](mailto:williamdemeo@gmail.com).

### Contributing using fork and pull requests

To [fork](https://help.github.com/articles/fork-a-repo/) the OpenProblems
repository to your own GitHub account login to your GitHub account,
navigate to the
[UniversalAlgebra/OpenProblems](https://github.com/UniversalAlgebra/OpenProblems)
repository, then click the
[Fork link](https://github.com/UniversalAlgebra/OpenProblems#fork-destination-box)
on the upper right.  Then clone the forked repository to your
local drive with a command like 

    $ git clone git@github.com:your-user-name/OpenProblems.git

or

    $ git clone https://github.com/your-user-name/OpenProblems.git

Now you can modify the files in your local copy of the repository as you see fit
and then, if you want to recommend that your changes be incorporated into the main
[UniversalAlgebra/OpenProblems](https://github.com/UniversalAlgebra/OpenProblems)
repository, follow these steps:

1. Commit your changes to your local repository. (Please include an informative
   commit message.)

        $ git commit -m "crossed an open problem off the list after solving it"

2. Push the changes to your remote repository (i.e., to the fork you created above).

		$ git push origin master
		
3. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/)
   by navigating to your fork's GitHub page and clicking the `Pull
   Request` link (which appears next to a message like, "This branch is 1 commit
   ahead of UniversalAlgebra:master"). 

   Be sure to include an informative comment justifying the
   recommendation to merge your changes into the main respository.

To keep your fork current with the main
[UniversalAlgebra/OpenProblems](https://github.com/UniversalAlgebra/OpenProblems)
repo, see the section [Updating your fork](#updating-your-fork) below.

### Updating your fork

When improvements are made to the "upstream"
[UniversalAlgebra/OpenProblems](https://github.com/UniversalAlgebra/OpenProblems)
repo, you will probably want to update your fork to incorporate these
changes.  Below is a list of the commands that accomplish this, but see 
[this page](https://help.github.com/articles/configuring-a-remote-for-a-fork/) and
[this page](https://help.github.com/articles/syncing-a-fork/)
for more details.

1. Change to the working directory of your local copy of the repository and
   specify the upstream repository. 

        $ cd ~/git/OpenProblems
        $ git remote add upstream git@github.com:UniversalAlgebra/OpenProblems.git

2. Verify that it worked.

        $ git remote -v

   The output should look something like this:

        origin	git@github.com:your-user-name/OpenProblems.git (fetch)
        origin	git@github.com:your-user-name/OpenProblems.git (push)
        upstream	git@github.com:UniversalAlgebra/OpenProblems.git (fetch)
        upstream	git@github.com:UniversalAlgebra/OpenProblems.git (push)

   If the foregoing fails, try

        git remote add upstream https://github.com/UniversalAlgebra/OpenProblems.git


3. In the working directory of your local project, fetch the branches and their
   respective commits from the upstream repository and merge upstream/master
   into your local master branch.

        git fetch upstream
        git checkout master
        git merge upstream/master

   This brings your fork's master branch into sync with the upstream repository,
   without losing your local changes. 

4. Finally, commit the changes and push to your remote fork.

        git commit -m "merged changes from upstream"
        git push origin master

   If you now visit the GitHub page for your fork's repo, it should show the
   message, "This branch is even with UACalc:master." 

5. If there are other branches besides `master` that you want to update, repeat
   the checkout and merge steps above replacing `master` with another branch name.

## Bugs and Other Issues
If you encounter a problem with the instructions on this page, or if you have
any other issue that you'd like to call attention to, please
[create a new issue](https://github.com/UniversalAlgebra/OpenProblems/issues).
