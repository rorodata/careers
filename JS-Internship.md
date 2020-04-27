# Problem Set for JS Engineer Intern
### Solve any one problem and write back to us with your solution repo raghav [at] rorodata [dot] com
##### More details [here](https://angel.co/rorodata/jobs/234424-javascript-frontend-intern)

## **Problem 1: Reimagine Github User Profile**

Implement a vue.js application to display profiles of a Github user. 

The application will have two pages.

The home page of the application will have a textbox to enter the username. On submit, it should render the profile containing the following details:
- name of the user
- picture of the user
- list of repositories of the user with descriptions.

Deliverables:
- Link to the github repo
- URL of the deployed application (you can deploy to Netlify/Heroku)

## **Problem 2: Reimagine Open Library search page

Build a simple vue.js application to search for books in [Open Library][ol] using the [Open Library Search API][search-api].

[ol]: https://openlibrary.org/
[search-api]: https://openlibrary.org/dev/docs/api/search

The home page of the application should show a textbox for searching and on submit, it should make an API request and render the results. Each result should include the following things:

* cover of the book
* title of the book
* number of editions
* "Read Online" button if the book can be read online

Here are the sample API resposne:

```
$ curl https://openlibrary.org/search.json?q=tom+sawyer
{
    "start": 0,
    "num_found": 366,
    "numFound": 366,
    "docs": [
        {
            "title": "Tom Sawyer",
            "author_name": [
                "Tim Mucci",
                "Mark Twain"
            ],
            "cover_edition_key": "OL25615999M",
            "edition_count": 4,
            "availability": {
                "status": "error"
            }  
        },
        {
            "title": "The Adventures of Tom Sawyer",
            "author_name": [
                "Mark Twain"
            ],
            "cover_edition_key": "OL23269295M",
            "edition_count": 416,
            "availability": {
                "status": "open",
                "identifier": "advtomsawyer00twairich"
            }
        },
        ...
    ]
}
```

The `title`, `author_name` and `edition_count` fields are self-explainatory. The `cover_edition_key` can be used to construct the URL of the cover. The URL will be `https://covers.openlibrary/org/b/olid/${cover_edition_key}-S.jpg`.

If the `status` is `open` in `availability`, then the book is readable online and the "Read Online" button should link to `https://archive.org/stream/${identifier}`.


Deliverables:
- Link to the github repo
- URL of the deployed application (you can deploy to Netlify/Heroku)
