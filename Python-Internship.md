# Problem Set for Python Engineer Intern
### Solve both and write back to us with your solution repo


## Problem 1

Write a program to find the longest word in the longest paragraph in the given text. The program should accept a filename as command-line argument and print the word it has found.

For a sample input, you can use:
https://anandology.com/tmp/twain.txt

Sample Usage:

```
$ python longest.py twain.txt
thelongestword
```

## Problem 2

Implement an API to search github repositories. The applcation will make use of the Github API to perform the search, however the request and response format will be different from that of the offical github API.

The requirements of the API along with the request and response formats are explained below. All the examples below asssume that the API server is running at `http://localhost:5000`.

The folllowing example searchs for all repositories matching the query "covid19".

```
$ curl http://localhost:5000/repos?q=covid19
{
    "repos": [
        {
            "name": "tokyo-metropolitan-gov/covid19",
            "url": "https://github.com/tokyo-metropolitan-gov/covid19r",
            "description": "東京都 新型コロナウイルス感染症対策サイト / Tokyo COVID-19 Task Force website",
            "language": "Vue"
        },
        {
            "name": "someshkar/covid19india-cluster",
            "url": "https://github.com/someshkar/covid19india-cluster",
            "description": ":microscope: COVID19 India Cluster Network",
            "language": "Javascript"
        },
        ...
    ]
}
```

The number of results included in the response is controlled by a query paramater `limit`, which defaults to 10.

To get the top 2 repos for query `covid19`, the URL would be: 

    http://localhost:5000/repos?q=covid19&limit=2

This endpoint also supports a query parameter `language` which limits the response to the repos with code written in that language.

For example, the following request finds all the "covid19" repositories written in language Python.

```
$ curl 'http://localhost:5000/repos?q=covid19&language=python'
{
    "repos": [
        {
            "name": "daenuprobst/covid19-cases-switzerland",
            "url": "https://github.com/daenuprobst/covid19-cases-switzerland",
            "description": "Data from BAG Tweets made useful.",
            "language": "Python"
        },
        ...
    ]
}
```

You are expected to consume the github API directly using urllib or requests library, and not use any other third-party library that exposes the github API.

Deliverables:
- README with usage instructions
- Implementation of the API in Python
- Deploy the API on Heroku/Digital Ocean/AWS and send us the URL endpoint as well
