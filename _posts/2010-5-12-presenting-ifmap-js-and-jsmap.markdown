---
layout: post
category: open-source
title: "Presenting ifmap.js and jsmap"
---

I've spent the past six months as a contractor with [Infoblox][1] in Santa Clara California working on projects related to
[IF-MAP][2], a client/server protocol for network-connected devices. I should have written a post describing the protocol
long ago, but I wanted it to be entertaining and have pretty pictures which ended up deterring me from ever starting.
So for the purposes of this post it's enough to say that a MAP server is pretty much just a graph database with
publish, search and subscribe operations, and a MAP client uses the IF-MAP protocol to perform those operations.
The IF-MAP protocol itself is really just a specific [SOAP][3] format built on top of HTTPS as a transport layer.

So with that little bit of background, I'm announcing the open-source release of two related software projects:
[ifmap.js][4] and [jsmap][5]. I'll describe each briefly below. See the README documents in each project's repository for
more information.

### [ifmap.js][4] ###

ifmap.js is an IF-MAP client library implementation in JavaScript. It depends on [jQuery][6]'s $.post(), $.each() and
$.proxy() functions. Due to browsers' [same-origin policy][7] a JavaScript IF-MAP client can't send requests directly
to a remote MAP server. All requests must be sent through a proxy, sold separately. For a simple example of how this
might work, see...

### [jsmap][5] ###

jsmap uses ifmap.js to build an actual IF-MAP client that runs in the browser. You can point and click to build
IF-MAP requests, submit them to a MAP server and see the responses. Requests are proxied through a simple
[Sinatra][8] application.

Comments and suggestions are most welcome. Just send me an email; my address is pretty easy to find. For more information about IF-MAP see [ifmapdev.com/documentation][2] and join the [ifmapdev Google Group][9].

[1]:http://www.infoblox.com/
[2]:http://ifmapdev.com/documentation
[3]:http://en.wikipedia.org/wiki/SOAP
[4]:http://github.com/andrewmbenton/ifmap.js
[5]:http://github.com/andrewmbenton/jsmap
[6]:http://api.jquery.com/
[7]:http://en.wikipedia.org/wiki/Same_origin_policy
[8]:http://www.sinatrarb.com/
[9]:http://groups.google.com/group/ifmapdev
