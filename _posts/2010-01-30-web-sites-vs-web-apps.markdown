---
layout: post
categories:
- tech
title: "Is a Web Site the Same As a Web App?"
---

This is an article I wish I'd found when I was starting out with web development. It's not meant
to be an exhaustive discussion of what exactly makes up a web application. But hopefully it will inform
and educate a few people and help to reveal how some of the software layers involved with web development
work together. I will probably amend and rework this post as time goes on and I figure out better ways
of explaining some of the concepts.

First we need some background.

*Servers and Clients*

When people talk about developing a web site, or a web app, or even a single web page, they are almost always
working on something with a client/server architecture, althought they might not know it. This isn't
actually complicated. A server is just a piece of software on a computer that "listens" for connections
and requests and "serves" responses. A client is a piece of software that initiates connections and
makes requests to a server and does stuff with the responses. (We use web clients every day, but we call
them web browsers.) A lot of the time the concept of a server
gets tied up with the particular computer the software is running on (as in, "oh that box over there is my
web server, and this one is my email server"). This is purely because someone has decided to isolate a
particular computer for performing a particular function and thus has it primarily running a particular
server software. But the server is still the software, and most internet connected "server" computers are
actually running multiple kinds of server software. For instance, a web server computer often is running
not only a web server, but an ssh server and an ftp server, all listening for different kinds of connections
and requests.

*The Legacy of HTTP and HTML*

Now any client and server need a way to talk to one another that's agreed upon beforehand, something called
a "protocol." For web servers and web clients the standard protocol is the Hypertext Transfer Protocol, or
HTTP. This simple protocol was designed for transferring specially formatted documents from a computer
running web server software to a computer running a web browser, and for passing information back the
other way. Those specially formatted documents are called HTML documents, short for Hypertext Markup Language.
Think of an HTML document kind of like a Microsoft Word document, except that it's way more annoying to
write. For a variety of reasons, including its simplicity, HTTP and the web server/browser ecosystem is the
dominant way that computers interact on the internet.

*OK, so what's a web site?*

A web site is just a collection of HTML documents sitting on a computer running web server software. Nothing
special is going on. When a web client (a web browser like Google Chrome for instance) makes a connection
to a web server, the client uses HTTP to ask for a particular HTML document. The server software then
finds that document and returns it. Think of it kind of like a Powerpoint presentation. A collection of
HTML documents is just like a collection of Powerpoint slides. They pretty much just display information.
Often the HTML documents are linked together. In fact, that's what makes them collectively a "site."
Without links, the HTML documents are just single web pages. The links are a convenience for the
web client. Instead of having to type in a new address every time you want a new HTML document, you can just
click a link.

*Then what's a web application?*

This is where things get interesting. A web application isn't a well-defined thing, so people may disagree
with the way I think about this. But to me, a web application is software that you actually interact with
to do something useful with data, running on an internet connected computer, which is also running web
server software, so that you can connect to the computer (and in turn the web application) in a standard,
well-known way, e.g. with your web browser. This is confusing, and the rest of this post is devoted to
explaining the distinction between a web site and a web application in order to (hopefully) alleviate
some of that confusion.

The most confusing thing is that the way that you interact with a web site and a web application looks
and feels the same from the outside. That's because programmers generally don't like to re-invent things
that are already working and well-accepted. HTTP and HTML and web servers (like Apache) and web clients
(like Firefox) are ubiquitous. So more and more complex ways of interacting with remote, internet-connected
computers got built upon what started out as a simple, HTML document exchanging technology. The tools and
interactions look the same on one level. Yes, your web browser is still talking HTTP to a web server,
and the web server still responds (not always, but generally) with an HTML document. But if you go a
little deeper there's a lot going on behind the scenes.

The extra things that web applications do take place behind the web server. The web server software is
just the gateway to the real application. You can't see what the actual application looks like by looking
at the HTML a web server sends back to your browser. For instance, when you click to add a friend on
facebook (which is most
definitely a full-featured web application), how does facebook's software actually associate you with that
person? There's no way to know, unless you can see facebook's source code. You can make educated guesses
based on the HTML that you get from the web server, but you can't know for sure unless you see the source
code of the software they have written. That's running behind the web server.

This is the major distinction. A web site uses a web server to do what it was originally 

There are lots of ways to write applications behind web servers now. The most common is probably to use PHP,
a programming language that's kind of designed for such uses. You can write applications in the Ruby
programming language using a variety of frameworks such as Ruby on Rails and Sinatra. You can write them
in the Python language using Django and Pylons. You can even write server-side applications in Javascript
with node.js. There will be many many more in the future as people decide they don't like the existing
options and create new choices.


