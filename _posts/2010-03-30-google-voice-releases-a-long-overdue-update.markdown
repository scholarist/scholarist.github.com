---
layout: post
category: tech
title: "Google Voice Releases a Long-Overdue Update"
---

Last week [Google Voice released an update for Android][1] that made the service essentially perfect as
far as I'm concerned. The update makes SMS and voicemail notifications to your Android phone appear
almost instantly. Previously SMS and voicemail messages would take up to five minutes to appear on your
phone. And in the early days of the service back in July 2009 it was taking even longer. I sometimes saw
delays of up to 45 minutes back then, which obviously makes any kind of SMS conversation impossible.

Without knowing for sure I'd say that this update must change SMS and voicemail delivery from pull to push.
Previously the Google Voice application running on your Android phone would poll the Google Voice server
every five minutes, pulling in new messages at regular intervals. If you received a message just after
one of those polls, you wouldn't see it on your phone until the next poll was sent. With push delivery,
anytime the Google Voice server receives a message addressed to you it immediately sends it down to your phone.

Push notification is very popular right now. New services like [Boxcar][2] and [Notifo][3] allow developers
to build push notification into their mobile apps. I'm glad to see Google pushing forward in this
direction with Google Vloice as well.


[1]:http://googlevoiceblog.blogspot.com/2010/03/faster-google-voice-experience-on.html
[2]:http://boxcar.io/
[3]:http://notifo.com/
