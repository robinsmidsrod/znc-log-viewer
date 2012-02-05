znc-log-viewer
==============

A simple Perl script to view your ZNC bouncer IRC logs.

It expects your logs to be located in
~/.znc/users/<username>/moddata/log/<logfile>.

You run it like this:

znc-log-viewer <username> <channel> <date>

Username must always be specified in full, but the channel parameter is a
simple substr match, and the date is a prefix substr match. If you omit
parameters, it will show you a list of valid users and channel names.

If I want to look for all messages in January 2012 on the #perl6 channel on
FreeNode, I type this:

znc-log-viewer freenode perl6 201201

LICENSE
=======

Same as Perl.

COPYRIGHT
=========

Robin Smidsrød <robin@smidsrod.no>
