##When you mess up your fork

And all you want to do is to go back to the original code in the original repo and you don't care if your local changes are lost.

    git remote add upstream /url/to/original/repo
    git fetch upstream
    git checkout gh-pages
    git reset --hard upstream/gh-pages  
    git push origin gh-pages --force 
    
Assuming you're using the branch gh-pages in your fork.

Snagged from [StackOverflow](http://stackoverflow.com/a/9646323/1075304).
