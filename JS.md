#Problem Set VueJS


Problem 1: Reimagine Github
Implement a webapp to reimagine github using GitHub API. The suggested technologies are VueJS + Bootstrap CSS.

The webapp should contain the following pages.

User / Org page

This page should list the profile picture and all the public repos with title and description.

Repo page

Each repo page should show the list of files in that repo and allow navigating though directories and download files.

For example:

'/test-user/sample-repo' will list the contents of the repo
'/test-user/sample-repo/Readme.txt' will show the contents of the file Readme.txt
'/test-user/sample-repo/src/' will list the contents of the directory src/ in the repo
For simplicity, limit the implmentation only to the master branch.

Deliverables:

Deployed webapp - we recommend netlify but you can choose any platform
Unit tests
Code repo

Bonus - History Page

The repo pages should have link to the corresponding history pages.

The history page should show all the commits on the repo or a subdirectory inside it.

For simplicity, limit the implmentation only to the master branch.

Make sure that you support pagination wherever the number of entries are more than 50.
