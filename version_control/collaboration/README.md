Collaborating with others using Distributed Source Control
-

####Introduction
Git makes it easy for users to collaborate on shared source using a variety of different possible patterns:

+ several users working with the same central git repository to collaborate on development of its content
+ one user serving as a steward for an 'official' repository and one or more 'development' forks for other users to directly
collaborate within.  Other users must collaborate in their specific development fork until they are ready to ask the steward to
review and accept the changes they have made.  A variation of this pattern uses branches instead of forks.
+ one user forking another user's repository, making changes, and then requesting that the other user merge their changes
into their own repository

All of these patterns are based on different ways of utilizing the following git client interactions:

+ Configuring one of your local git repositories to know about one or more 'remote' git repositories.
These remote repositories can be on the same filesystem, or accessible over the network using ssh or http(s)
+ cloning/forking a remote repository to a repository that you own and control
+ pulling committed changesets from a remote repository into your repository
+ merging pulled changesets into your repository, with the possibility of committing them, or restoring to your version
+ fixing conflicts between your code and merged changesets in various ways
+ pushing your committed changesets to a remote repository
+ submitting a patch or pull request to a remote repository owner to allow them to review and apply your changes at their discretion

####Remote Git Repository Hosting Services
There are several prominent git repository hosting services available to users.  Most of them allow users to host and share repositories
for free, up to certain limits in size, or number of different repositories.  Some will incentivize the creation of publicly available repositories
over private repositories. Most allow external users to interact with the users repositories
for free without limits.  Here is a list with some notes about them:

| Hosting Service        | Notes           |
| ------------- |:-------------:|
| (Github)[http://github.com] |  +Largest worldwide network of git repositories.
+Free accounts.  Users can create an unlimited number of free publicly accessible repositories.
+Subscription required to host private repositories.
+Public repositories can still control which users can modify content in the repository.
+All repositories can have an unlimited number of collaborators for free.
+Has been adopted by many systems being designed to facilitate reproducible research
+Has many 'social' features that can be used to enhance your online web presence.
+Has a fantastic online user interface. |
| (Bitbucket)[https://bitbucket.org] | Supports both git and mercurial repositories. |
|   | Free accounts. Users can host an unlimited number of public or private repositories. |
|   | Up to 5 collaborators can work with a repository for free, subscription required for more collaborators |
|   | Not used within the research reproducibility community |
| (Duke Gitorious)[https://gitorious.oit.duke.edu] |  Accounts only available to Duke Faculty, Staff, and Students. |
|   | Public repositories are available read-only to any user on the internet. :|
|   | Account required to collaborate on shared repositories. |
|   | Not used within the research reproducibility community |
