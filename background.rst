Background
==============

Anyone who is involved with a school will know that they are immensely
busy places with far more going on than just the timetable would indicate.
Scheduler started as a project in a single school to try to keep
track of everything which was happening.

Although staff did their
best to make each other aware of planned events, this was mainly
done by means of public announcements in weekly meetings and lists
of pupils pinned to boards.  The overhead of every member of staff
reading all these lists and mentally comparing them with their
own set lists (and taking into account the timing of the events) was
considerable.

For some reason, pupils never think to mention that they seem to
be scheduled both to play in a concert and to go on a theatre
trip on the same evening - not until the actual day arrives anyway.

Early versions worked by parsing PDFs of all the staff and pupil
timetables in order to populate the events database!  Over time
a better import mechanism was constructed and Scheduler now has
the means to interface with Schola (an in-house developed MIS),
SchoolBase (using direct database access), iSAMS (using a mixture
of the iSAMS Batch API, and direct database access where the Batch API is
lacking) and WCBS/Pass (using their ODBC interface).

The largest school using it has just over 1000 pupils and 400 staff, and
it is the prime repository for much of the school's scheduling information.
The timetable, cover and regular activities come automatically from the
school's MIS (updated nightly) and then Scheduler holds the school's
calendar, plus all the other events which aren't on the timetable.

It handles room bookings (with or without approvals), plus services
like catering or cleaning.  For any resource, versatile forms can be
created through a drag-and-drop interface, allowing rich detail to
be collected on, for instance, what catering is required.

Some resources can naturally be organised in pools - for example, minibuses.
A trip might need two minibuses, but it doesn't matter to the trip
organiser which ones they are.  The person responsible for administering
minibuses decides which two to allocate.  Scheduler provides versatile
facilities to facilitate this process.
