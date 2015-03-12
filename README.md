# json-hyperschemas

## Overview
Within Mozilla, we have several APIs (e.g. buildapi, clobberer, (modern) mapper, mozpool, slavealloc, slaveapi, ...) to talk to our internal systems. This project standardises on a way of defining them, publishing them, documenting them, and sharing them. This project will use json hyperschema (see e.g. https://brandur.org/elegant-apis) to define the apis. Please get involved to help define a framework for auto testing/validating the schemas, auto documenting/publishing the apis, and even auto-generating client libraries for them in languages like python, node.js etc.

Example REST apis that we have are:

* Build API: https://wiki.mozilla.org/ReleaseEngineering/Applications/BuildAPI
* Clobberer: https://api.pub.build.mozilla.org/docs/usage/clobberer/#endpoints
* Mozpool: http://hg.mozilla.org/build/mozpool/file/tip/API.txt
* Slave API: http://mozilla-slaveapi.readthedocs.org/en/latest/api/#slaves-slave-actions-disable

We need help with creating hyperschemas for the above APIs (and potentially others too), finding a good place to publish these references, and look at setting up some tools to generate documentation for these APIs, together with code generation of client libraries, and their associated documentation (godoc, javadoc, …) and auto-generation and deployment of new documentation, libraries, as and when these json hyper schemas get updated (perhaps with travis ci deploying to e.g. github pages or heroku).

## Frameworks in this space
There are some other technologies worth considering in this project:
* http://raml.org/
* http://swagger.io/
* https://apiblueprint.org/

The first phase of this project should be to evaluate these technologies, as well as json hyperschema, to assess relative merits of each, and to evaluate the relative merits of supporting each of them (and whether there exists any automatic translation between the different declarative formats).

## Issues
Issues/bugs etc will be tracked as github issues.

## IRC
We are also on IRC: irc://irc.mozilla.org/json-hyperschemas
