- Consider your main branch is `mainBranch` and working branch is `featureBranch`. Considering you are currently at the featureBranch
    
- cd to root folder, Create a patch
    
    `git diff mainBranch -- folderA/ > diff.patch`
    
    This will create a patch file with the file changes in folderA only.
    
- Checkout mainBranch & create a new branch from mainBranch
    
- Apply the patch
    
    `git apply diff.patch`
    
- commit and push to raise PR
    

This will create a PR with changes in folderA only. Repeat for other folders.