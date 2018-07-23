[![Build Status](https://jenkins.sonata-nfv.eu/buildStatus/icon?job=tng-api-gtw/master)](https://jenkins.sonata-nfv.eu/job/tng-api-gtw/master)
[![Join the chat at https://gitter.im/5gtango/tango-schema](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/5gtango/5gtango-sp)

<p align="center"><img src="https://github.com/sonata-nfv/tng-api-gtw/wiki/images/sonata-5gtango-logo-500px.png" /></p>

# 5GTANGO DOCUMENTATION
This is the 5GTANGO Documentation Repository.

Please see [details on the overall 5GTANGO architecture here](https://5gtango.eu/project-outcomes/deliverables/2-uncategorised/31-d2-2-architecture-design.html). 

## How does this work?

After creating a new API or modifyng an existing one, the developer must create/update a swagger spec description file. This document will help the current team and newcomers to understand how their API works.

Here [https://swagger.io/docs/specification/about/], you can get full detailed info on how to create the swagger files.

After created, you only need to add the link to this file in 'urls' section in the 'index.html' of this project. And after some seconds your swagger spec doc file will be available in the tng-doc page [https://sonata-nfv.github.io/tng-doc/].

Other components are the following:

* [tng-common](https://github.com/sonata-nfv/tng-gtk-common/);
* [tng-gtk-sp](https://github.com/sonata-nfv/tng-gtk-sp);
* [tng-gtk-vnv](https://github.com/sonata-nfv/tng-gtk-vnv);
* [tng-policy-mngr](https://github.com/sonata-nfv/tng-policy-mngr);
* [tng-sla-mgmt](https://github.com/sonata-nfv/tng-sla-mgmt);
* [tng-slice-mngr](https://github.com/sonata-nfv/tng-slice-mngr);

## Developing

You can fork this repository, and add your new entries (links to your swagger files) to the index.html, in the urls section like this:

		urls: [ 
{url: "https://raw.githubusercontent.com/sonata-nfv/repository_X/rest_api_model.json", name: "5GTANGO Repository X API v1"},
{url: "https://raw.githubusercontent.com/sonata-nfv/repository_Y/rest_api_model.yaml", name: "5GTANGO Repository Y v1"},
	],

After the pull request is accepted, new elements will be published in https://sonata-nfv.github.io/tng-doc/

