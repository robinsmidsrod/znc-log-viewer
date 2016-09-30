znc-log-viewer
==============

A simple Perl script to view and search your ZNC bouncer IRC logs.

It expects your logs to be located in
`~/.znc/users/<user>/networks/<network>/moddata/log/<logfile>`.

You run it like this:

    znc-log-viewer [<user/network>] [<channel>] [<date>]

User and network names must always be specified in full, but the channel
parameter is a simple sub-string match, and the date is a prefix sub-string
match.  If you omit parameters, it will show you a list of valid user,
network and channel names.

If you want to look for all messages in January 2012 on the #perl6 channel on
FreeNode, you type this:

    znc-log-viewer freenode perl6 201201

If you use multiple networks per user, then you should type something like
this to search the network `freenode` under the user `robin`:

    znc-log-viewer robin/freenode perl6 201201

INSTALLING DEPENDENCIES
=======================

If you use `cpanm`, then installing the dependencies should be a breeze
using the included `cpanfile`.

    cpanm --installdeps .

SEE ALSO
========

* The ZNC log module - http://wiki.znc.in/Log
* cpanm - https://github.com/miyagawa/cpanminus
* cpanfile - https://github.com/miyagawa/cpanfile

LICENSE
=======

Same as Perl.

COPYRIGHT
=========

Robin Smidsrød <robin@smidsrod.no>
