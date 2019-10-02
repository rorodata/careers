# Design a RESTful API for managing machines in the cloud

Note: There is no need for actual cloud integration

## Context

There will be multiple clusters and each cluster will have zero or more
machines. Each machine will have zero or more tags.

Also, each cluster will have a name and a cloud region, each machine
will have a name, ip address, an instance-type.

The system should allow users to create clusters, create machines in a
cluster, add tags to the machine when creating them, delete machines and
clusters and perform operations like start, stop, reboot on a group of
machines using tags.

## Problem Statement

Your API should do everything required to manage the clusters and
machines, except actually creating the machines in the cloud.

### Deliverables:
- Implementation of the API in Python using Flask or Go lang
- Test cases
- A README explaining the API instructions about how to run it locally
- URL of the application deployed to Heroku/Digital Ocean/GCP/AWS


### What are we looking for?
- Problem solving approach
- API design and it's completeness
