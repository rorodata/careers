**Problem Set for Full Stack Engineer**

Solve the problem below and write back to us with your solution repo and link to the deployed app raghav [at] rorodata [dot] com

File upload service with Dropbox
Build a webapp for data upload using the [Dropbox API](https://www.dropbox.com/developers/documentation/python#overview). The suggested technologies are Flask + Jinja templates + Bootstrap CSS.

The user should be able to do the following
1. Upload csv files in dropbox folder
2. View the file data as a table (with pagination) in a web browser
3. View the history of all the files uploaded to the app
4. View record of errors in file upload. Error-type Supported: mis-match of columns i.e if the columns files do not match then upload is rejected

Note: Data from new files is appended to the existing data. The appended data can be stored in S3/CloudStore

The webapp should contain the following pages.

**Data page**

This page should show the data in tabular form with pagination

**History page**

This page will have table of all files pulled from dropbox and appended to the base data

For simplicity support on one type of file error tracking - mis-match of columns

**Deliverables**

1. Deployed webapp - we recommend digital ocean or heroku but you can choose any platform
2. Unit tests
3. Code repo
