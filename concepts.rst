Concepts
========

Scheduler is built around two basic concepts - events and
resources.

======
Events
======

An event is an instance of something
happening. It has a time when it happens, and possibly a duration.
However, events are for the most part not very interesting unless
they involve people or things. The main thing that Scheduler does is to
keep track of which resources are involved in each event, and then let
events be selected, based on the resources which they
involve.

=========
Resources
=========

Scheduler understands five different kinds of resources which can be used by
events, plus two kinds of pseudo-resource used to categorize events.

* Staff
* Pupils
* Groups
* Locations
* Services

* Properties
* Subjects

Staff, Pupils and Locations are fairly self-explanatory.

Services are things like Catering, Parking, Porters or Cleaning.

Properties are used to categorize events - the largest category is
Calendar, for events in the school's public calendar, but you can set
up as many other ones as you like.  Obvious candidates are "Sport
Calendar", "Music Calendar", "Drama Calendar" etc.  Any event can belong
to as many or as few of these as you like.

Subjects are used to keep track of which subject any given lesson
is devoted to.  In a typical school, it is possible to derive this
information from the name of the lesson, but by storing it explicitly,
one can then select lessons based on the subject.

Groups are the odd man out in the list of resources. They don't represent
anything on their own, but instead allow you to group together any of
the other resources. They can do obvious jobs like representing
teaching groups or tutor groups, but they impose no restrictions on what
resources can be put into each group. Rather than just being
groups of pupils, you can potentially create a group containing 6
pupils, 3 members of staff, 2 rooms, plus the Music Calendar. You
can also nest groups within groups, and even subtract one group from
another.

======================
Structured information
======================
Much of what Scheduler does could be done with a general purpose calendaring
program like Google Calendar, except that they don't usually understand
structured information. You'd need to create
thousands of separate calendars to cover all the resources within the
school, then spend thousands of man hours copying all the events between
the calendars.

Instead Scheduler uses just a single place to store all its event
information, along with details of what resources are used by each
event - staff, pupils, rooms and services.  A single medium-sized
school can easily have several million such records, and so much has
been done to allow selective viewing of just what the user wants to
know.

