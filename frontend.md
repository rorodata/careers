# Problem Set for Frontend Engineer
Solve the problem below and write back to us with your solution repo and link to the deployed app raghav [at] rorodata [dot] com [More details on the position](https://cutshort.io/startup-job/VueJS-Engineer-Bengaluru-Bangalore-Algoshelf-IAsEO5w4)

## **Reimagine [Github](https://github.com)**

Implement a webapp to reimagine github using [GitHub API](https://developer.github.com/v3/). The suggested technology is VueJS.

The webapp should contain the following pages.

**Landing page**

Ask the site visitor to input a github handle(username) they wish to explore. The visitor should be then taken to the Repo Page (see below) that has the profile picture of the user and all the user's public repos with title and description. Details of the repo page are below.

**Repo page**

Each repo page should show the list of files in that repo and allow navigating though directories and download files.

For example:

'/test-user/sample-repo' will list the contents of the repo
'/test-user/sample-repo/Readme.txt' will show the contents of the file Readme.txt
'/test-user/sample-repo/src/' will list the contents of the directory src/ in the repo

For simplicity, limit the implmentation only to the master branch.

Deliverables:
* Deployed webapp - we recommend Ziet or Netlify but you can choose any platform of your liking
* Unit tests
* Code repo

**Bonus Page** 

**History Page**

The repo pages should have link to the corresponding history pages.

The history page should show all the commits on the repo or a subdirectory inside it.

For simplicity, limit the implmentation only to the master branch.

Make sure that you support pagination wherever the number of entries are more than 50.
