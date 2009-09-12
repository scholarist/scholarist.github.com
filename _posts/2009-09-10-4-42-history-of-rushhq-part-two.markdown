---
layout: post
categories: personal
title: "History of RushHQ (part II)"
---

This is part two of a multi-part series detailing the history of my web startup [RushHQ][1].
Part one is [here][2].

---

#### Writing RushHQ Ourselves

Before the middle of April, 2008 David, Rick and I had assumed we would pay programmers to build RushHQ
on top of the source code of CASManager, a product that David was selling to help International
Baccalaureate schools manage their CAS programs. We would have had to buy the CASManager source code
from Theodore and Faria Systems, the company David worked was working with. But once it became clear that I would have to
fund the purchase and subsequent programming work out of my own savings, that path became much less
attractive.

So I convinced David and Rick that we could write the software ourselves, despite having no experience
and no time. Luckily David took the initiative and started reading everything he could about Ruby on Rails
(RoR), which is a web-application framework. CASManager is a RoR application, as are huge new sites like
Twitter and Justin.tv, so it was a credible choice for us. It was also relatively new but
had a huge community of developers using it and creating new features.

So David worked really hard on learning RoR. In late April and early May I was very busy trying to
finish my second-year paper for my PhD in Economics, so I didn't spend much time on learning the ways
of web-programming and fell behind David. This would prove to be important later. I was at least
able to contribute as our server administrator, building on the knowledge I had gained fiddling with
Linux in 2000 and 2001. I also handled all of our DNS administration.

On May 9th, 2008 David quit his job selling CASManager for Theodore to work on coding RushHQ. His quitting
had a lot to do with the strained relationship between him and Theodore, Faria's founder. But his
decision to quit gave him tons more free time to teach himself RoR and work on RushHQ, whereas I was again tied down with
studying for my PhD general/comprehensive exams until I completed them in early June. (Admittedly I
didn't actually study very hard since I was taking two of the rather easy exams, but I did pass at least.)

#### David and Andrew Move to Georgia

It was in May that David and I worked out a deal with our mutual friend Adam's mother Judy. She was
the director of an artists residency program in northern Georgia near a town called Dillard, and she kept
a house nearby in the woods as both a vacation home and a place to stay during work visits.
David and I wanted to seclude ourselves in that house in the woods to get a large chunk of RushHQ
coded up. Luckily she needed some database work done for the residency program, so we exchanged database
work for summer housing.

As soon as I finished up my exams at Princeton in early June I drove down to Atlanta to meet up with 
David and pick up the mountain house key from Judy. (There's an amusing story related to my arrival in
Atlanta but it's not appropriate for this post). David and I drove up to Dillard the same night.

During our time in Georgia David and I (mostly David) made a lot of headway into RushHQ. But if you read my
post [here][3] about writing a new version of RushHQ you'll remember that we made some naive decisions that
I consider now to be mistakes. Most of those decisions were made in Georgia while we were really
starting to put the basic pieces of RushHQ together. While in Georgia we also did a bit of hiking and tried to complete
1000 pushups in 24 hours or less (we couldn't).

#### Andrew Leaves the Mountain House

Back in May David and I had also decided to move to San Francisco after the summer. There's no
better place to write software and try to start a startup, so we had to go. We had agreed to live
with our friend Dave Linder in an apartment that he would rent starting July 1st, and the plan was
to move out to SF in August. Unfortunately my mother had planned a family trip to China for mid July,
which would eat into the time I had to contribute to RushHQ. I also decided to leave the mountain
house in GA before my trip to China to fly out to SF and handle the arrangements for the apartment
with Dave. David later admitted that he was frustrated by my lack of commitment during our time in GA,
which was justified considering my early departure. This became a point of contention later (see below).

I was able to contribute quite a bit still by learning Subversion (the most popular scm at the time)
and trying to get our application "deployed" to our server after returning from China.

#### What Happened to Rick Fox?

You might be wondering this. To be honest I don't exactly remember what Rick was doing this whole time.
He had his full-time job still, and wasn't a programmer at all, so he didn't have much to do. We weren't
communicating regularly. I think he probably worked on some marketing copy for the public website at some
point.

#### David Gets Angry

David put a lot of effort into RushHQ in its infancy. Almost the entire first iteration was his code.
He was justifiably upset with me (and Rick) for not carrying our weight. And before I arrived in
San Francisco in early August he called and told me he wanted to take the project and make it his own.
He wanted me and Rick out.

Needless to say I was not happy about this. I was moving to San Francisco to live and work with David.
I wanted to work on RushHQ. Obviously there was no money from the business to fight about yet. It was
mostly that I had put in some work already and I felt like I had a lot more to offer, so it was
frustrating that David didn't see it that way.

Making matters worse was that David incorporated the business in Delaware without discussing it with
Rick and me. He also moved forward on asking our mutual friend Andrew Glantz to design the public
website. Neither decision in isolation was a big deal. They were more symbolic of David's go-it-alone
attitude at that point.

So I arrived in San Francisco under these somewhat awkward circumstances. I remember having lots of discussions
with David about how to move forward. Some of these involved me spinning off what existed of the RushHQ
source code into a product for sororities. Most of the discussions involved me trying to explain to
David that RushHQ wasn't his to take. It was a contentious time. A lot of trust was damaged.

#### Moving Towards Launch

But in the end David came around to the idea of the three of us working together still. I'm not sure exactly
how it all shook out. But I know that I started coding on the project again, and we started moving rapidly
towards an early September launch. I remember coding a bunch of raw SQL during that time, since RoR's
native ActiveRecord ORM doesn't handle JOINs very well.

I made a lot of cosmetic changes to the application, trying to simplify and standardize the look and feel.
David was trying to complete a few key features. We hired a flash programmer to take care of a
crucial piece of RushHQ called DoorManager. The idea was to have fraternity members be able to set up
a computer with a built-in camera so that recruits coming to rush events could submit their information
and a photo to the fraternity's recruitment database. We needed the flash work done to hook into a
computer's built-in camera.

We collected email addresses for as many fraternity contacts as we could. David's girlfriend Sarah-Jane
was amazingly helpful with that effort. She spent hours each day scouring fraternity websites for
contact information.

We were trying to launch before the start of the college rush season in late August, so things started
moving very quickly. Andrew Glantz came up with a passable public website for us. David and Rick worked
out some marketing copy they liked. I worked furiously getting up to speed
on server administration tasks, and figuring out how to deploy a RoR application. In the end
we ended up paying a little money for our hosting provider to deploy the app the first time.

And after a couple of delays, we finally launched with an email to our contact list on September 5th, 2008.
Little did we know that most of the hard work was still to come.

Part III coming soon...

[1]:http://rushhq.com
[2]:/personal/2009/07/24/14-45-history-of-rushhq-part-one.html
[3]:/personal/2009/07/27/9-33-writing-rushhq-2-0-part-I.html
