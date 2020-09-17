# GitFlow

![GitFlowPattern](https://www.campingcoder.com/post/20180412-git-flow.png)

With GitFlow, many organizations/startups developing web, mobile or game applications are able to
utilize a model that allows for features to be developed independently and allow developers to
work in parallel between different tasks without the risk of losing changes. 

It all starts with feature branches, branches that are branched off of the develop(development) branch. These branches
allow for developers to be able to commit their code in their own feature branch for a specific functionality 
they are developing for. Whether it be a small bug fix or a new feature, developers can switch branches as needed 
with feature branches.

![FeatureBranching](https://backlog.com/app/themes/backlog-child/assets/img/guides/git/collaboration/using_branches_002.png)

When developers feel that the work they've finished in their respective feature branch and are unit tested, they can
make a pull request to the develop branch which will be merged later. The develop is the branch where all feature level
changes that are ready to be released are and haven't been released yet.  

A release branch is created off of the develop branch when changes needed for a release have made it into develop. From
the release branch, it can be deployed to any testable environment to be thoroughly tested and vetted out through either
stress, load and regression tests.

![DevelopersWorkingTogether](https://miro.medium.com/max/1400/1*SocipNKmX8WP0uJR6W3xpw.jpeg)

When the release changes are ready, they can be staged to be merged into master and also develop as well. The release
branch has to be merged back with develop to make sure the changes between master and develop are in sync. The master branch
contains all of the code that has been released only through the release branches and a hotfix branch.

If, an issue in master (production) is found, a hot fix branch can be made that contains the code to fix
the issue within master. The changes, when ready, will be merged in develop and master to make sure both branches are in
sync.