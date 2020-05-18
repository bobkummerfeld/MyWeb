+++
title = "Secondpost"
date = 2018-12-10T14:57:11+11:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []
categories = []

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
# Use `caption` to display an image caption.
#   Markdown linking is allowed, e.g. `caption = "[Image credit](http://example.org)"`.
# Set `preview` to `false` to disable the thumbnail in listings.
[header]
image = ""
caption = ""
preview = true

+++

This is my second blog entry, still recounting my history.

## History – part 2

My story continues in 1980 when I was a tenured lecturer in Computer
Science. At that time I had become interested in networks and the
emerging internet in particular.  Australia had a fragmented academic
network at the time with the public X25 network and CSIROnet the
only long haul options, with some use of dialup modems. It was also
the time when Unix was starting to takeoff in Universities - having
arrived in 1975 but now becoming suitable for large scale teaching.

At the end of 1979 the Basser Dept of Computer Science at Sydney
installed a DEC VAX780. Through our close relationship with the
Bell Labs Unix group we were able to use the latest Version 8 Unix
and our programming staff (led by Piers Lauder) did extensive work
to make it handle large numbers of dumb terminals in a student
teaching environment.  Looking back on it this was amazing work.
The machine was powerful for its day but less powerful than the
Apple watch of today!  It had 4Mbytes main memory (no typo - that
was MEGA bytes) and a 1MIP processor. Yet it handled up to 100
student terminals running a text editor, compiler and utilities.
At 100 it was only just usable but at 60 terminals it was fine.
Part of the secret was the development of an inovative scheduler
(the "fair-share" scheduler) that scheduled processes on the basis
of resource usage (cpu/mem/IO etc) rather than just CPU, and had
an approach that shared the resources equitably over of long period
(eg days). This work (mostly by Piers Lauder and Judy Kay) is
the foundation for fair-share scheduling right up to the present
day.

The early 1980's was also the beginning of cheap academic networking
in Australia.  Fixed line modems were cheap and accessible allowing
a simple async character connection between two machines. Our first
such connection was a 2400 bps line to UNSW where a lot of Unix
development was going on.  This allowed remote interactive sessions
and our programming staff could work with UNSW programmers on Unix
development.  The missing service was the ability to send email and
files. Unix had a primitive system called UUCP (Unix to Unix copy)
but it was direct from one machine to another without any routing
capability. Routing of messages was performed manually by embedding
the route in the address. This was primitive and inconvenient and
inspired me to propose a system that exchanged routing tables and
did the routing automatically.   With Piers Lauder the first version
was developed (called the Sydney Unix Network or SUN) and deployed
around Australia to create the Australian Computer Science Network
or ACSnet.

Things really took off at that point with all University CS departments
joining the network and new versions of the system produced with
more facilities. Eventually we commercialised the system (renamed
as MHSnet - more on that later) and continued to develop it for
many years after.

The key architecture of  MHSnet is that it was a store-and-forward
message system with a very flexible transport layer that could run
over any sort of underlying communication link, and a flexible
application layer that could provide message services for things
such as email and file transfer among many.  The transport layer
could run over dialup, fixed lines or services such X25 and the
emerging TCP/IP networks. The core of MHSnet was a heirarchical
message routing service that exchanged routing tables between
neighbouring nodes but automatically pruned the table where possible.

On a personal note, the 1980s were when my incredible children were
born - Sarah in 1980, Rebecca in 1985 and Jonathan in 1988.  All
now with PhDs and in senior positions in research and academia.
