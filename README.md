# sprintf.js alias: npm-sprintf.js

npm package of sprintf at alexei/sprintf.js

this is a repo to hold different versions of github.com/alexei/sprintf.js
you may need.

This master repo only hold this readme. to upgrade add branches of versions


# sprintf.js ready to run files

Downloaded from [https://github.com/alexei/sprintf.js](https://github.com/alexei/sprintf.js)
and merged to the "packages" branch to have the versions an application may need.

If you want several versions of sprintf.js this will be your primary branch to choose:

    $ git checkout packages

If you just need a special version then checkout the branch you need or create
a new branch including the version you want.

If you need several versions? Then merge it to the packages branch an switch
back to the packages branch.



## Examples/ Howto add new versions


### branch master

    ./README.md (copy of this readme incl. updates of changes/ additions)


### branch of version 'vA-B-C;
    ./vA.B.C/sprintf.js
    ./vA.B.C/README.txt (eg the README of sprintf.js vA.B.C)
    ./README.md (copy of this readme (from the master branch))


### Add newer versions

If a new version exists and you need it globaly/ in packages branch:
Don't drop other versions! Add your version to a new branch and merge it to the
packages branch! Not vice versa merges!

Eg: You need also version 2.0.0:

    $ git checkout master
    $ git checkout -b "v2-0-0" # (branches needs "-" and NO dots!)
    $ mkdir v2.0.0/

    # Download the files *.js/*.css to v2.0.0/

    $ git add -a
    $ git commit -m "Adds version 2.0.0"
    $ git push -u origin v2-0-0

Now merge the branch to packges branch if you want/need it:

    $ git checkout packages
    $ git merge v2-0-0
    # commit and push, done

Result of packages branch:

    ./vA.B.C/sprintf.js
    ./vA.B.C/README.txt

    ./v2.0.0/sprintf.js
    ./v2.0.0/README.txt

    ./README.md (copy of this readme on creation time)

    The ./README.md of the packages branch contains all updates in changelog
    section. if you update i on each version branch.



# Changelog

2021-01

 + Init adding sprintf.js as alias: npm-sprintf.js

