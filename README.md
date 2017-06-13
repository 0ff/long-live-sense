# long-live-sense
As Hello said Goodbye, this repo is in an effort to keep the Hardware alive

# Motivation
Hello, inc. yesterday [announced](https://twitter.com/hello/status/874362590045937664) that they'd be shutting down in the foreseeable future.
As a first-minute user of Sense, I'd hate to see this beautiful piece of hardware turn into a beautiful paperweight.

This repository should become a central hub to coordinate the efforts of reverse-engineering the following parts that, in sum, make up Sense.
## Parts 
### Sense Server
#### Sense API
This API is needed to allow for the basic operation of the Sense hardware.
We will need to implement a custom server that provides the same calls so that Sense keeps running.

##### Todos
* [ ] Connect Sense via MITM Proxy to the server
* [ ] Document used Endpoints and existing responses
* [ ] Mock API

#### App API
This API is consumed by the Sense App and allows reading stats and setting up alarms.

##### Todos
* [x] Connect Sense App via MITM Proxy to the server (see References)
* [ ] Document used Endpoints and existing responses
* [ ] Mock API

##### References
* https://github.com/fredkelly/sense-client
* https://github.com/chendo/sense-api.cr

### Sense Firmware
These are the bits and bytes that power the Sense Hardware. At the very least, we will need to figure out how to make Sense connect to a custom API URL.

##### Todos
* [ ] Fetch existing firmware from the Sense Server
* [ ] Figure out how to change the API URL
* [ ] Figure out how to update Sense with custom firmware

### Sense App

# Contributing
This project will live through contributions, so please, if you have anything to add - fork it, submit a PR and be part of it.
