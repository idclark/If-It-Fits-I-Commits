[![Actions Status](https://github.com/idclark/go101-rest-api/workflows/Test/badge.svg)](https://github.com/idclark/go101-rest-api/actions)
[![Coverage Status](https://coveralls.io/repos/github/jandelgado/golang-ci-template-github-actions/badge.svg?branch=main)](https://coveralls.io/github/jandelgado/golang-ci-template-github-actions?branch=main)
## If It Fits... I Commits 
... and if it doesn't fit you can still commit because this is distributed. Yay!


#### Motivation
Intended for learning purposes only. I wanted to gain experience with golang while learning about distributed
data systems. 

Some of the most helpful links:
* [Martin Kleppmann's class](https://www.cl.cam.ac.uk/teaching/2021/ConcDisSys/dist-sys-notes.pdf)
* [MIT 6.824](https://www.youtube.com/channel/UC_7WrbZTCODu1o_kfUMq88g/videos)
* [Travis Jeffrey's book](https://pragprog.com/titles/tjgo/distributed-services-with-go/)

Service discovery is enabled by [HashiCorp Serf](https://www.serf.io/intro/index.html) while consensus across nodes is provided by [HashiCorp Raft](https://github.com/hashicorp/raft). 

### Build a Log

* Record: The literal stored data. 
* Store: File that stores records.
* Index: File that holds indexes.
* Segment: Abstraction tying together Indexes and Stores. 
* Log: Abstraction tying together multiple Segments.
