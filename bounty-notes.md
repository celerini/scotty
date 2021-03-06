# leg20170214 -*- mode: markdown -*-

The FlightAware Bounties
========================

Introduction
------------

On November 15th of 2016 Karl Lehenbauer annouced on GitHub,
[FlightAware][]s bounty program for improvements to Tcl and certain
Tcl packages.

This document sums up the requirements for the bounty on scotty and
then lists the respective references from where they are derived.

The last section is a verbatim copy of the bounty rules.


Scotty Improvement Requirements
-------------------------------

+ Change build system to compile under TEA 3.10.

* Compile under the following operating systems:
    + FreeBSD 
        + 10.3
        + 11.0
    * Debian GNU/Linux:
        - Jessie:
            -  8.2
            +  8.7
		- Wheezy: 7.9
		  + 7.11
        - Stretch: Sid
    + Ubuntu 16.10, Yakkety Yak
    - macOS Sierra

+ Stub support.

- Figure out official hosting situation.

- Update Scotty page on [Tclers Wiki][]



Upgrade the scotty extension
----------------------------

(20170214: https://github.com/flightaware/Tcl-bounties)

$1000 to update Scotty to modern Tcl Extension Architecture (TEA)
build standards, compilling properly under FreeBSD, Debian and macOS,
with stub support.

$1000 to fix bugs in Scotty's UDP stuff -- "configure/cget" of config
vars working and configured host and port to be used if not specified
in "send".


Dibs on scotty
--------------

(20170114: https://github.com/flightaware/Tcl-bounties/issues/7)

bovine commented on Nov 22, 2016

For reference, FlightAware has a fork of Scotty here:
https://github.com/flightaware/scotty (I believe our fork was taken
from some other obsolete source?)

But it appears that someone else has a 2015 fork on SourceForge, which
may have possibly been based off of ours, but may now be abandoned
again? https://sourceforge.net/p/tkined-scotty/code/HEAD/tree/ It
appears to possibly have some Linux porting fixes that could be useful
to incorporate.

It would be nice to figure out the official hosting situation and
update http://wiki.tcl.tk/691
     

Rules for Tcl bounties
----------------------

- All code must be released under the BSD license.

- For bounties under $10,000, the bounty will be paid when the code is
  accepted into the Tcl core, or if not part of the core, accepted by
  the package maintainer.

- For bounties $10,000 and over, we’ll pay 50% of the bounty will be
  paid out when the code is accepted into the Tcl core and the
  remaining 50% when it appears in a release of Tcl.

- The first person or team to succeed wins the bounty.

- If you succeed in fulfilling the conditions for receiving a bounty
  as a team then the team has to apportion the bounty among
  themselves; we are not getting involved in any disputes over who
  deserves what.

- We request that people or teams publicly announce
  their intention to pursue a bounty to reduce the likelihood of
  wasted work, hard feelings, etc.
  
    - That being said we understand that some people or teams may
      announce and not succeed, so the fact that someone has announced
      they are pursuing a bounty does not prevent others from pursuing
      it as well.

- If due to the nature of their employment someone is not allowed to
  accept a bounty or their share of a bounty, they can assign their
  share to others on their team, to a charity of their choosing, or to
  the Tcl Community Association.

- FlightAware employees can participate but not double-dip; i.e. don't
  work on it at work.

- When appropriate, the TIP process may need to be followed for
  changes that impact the public interfaces of Tcl core.


[FlightAware] https://flightaware.com/
[Tclers Wiki]: http://wiki.tcl.tk/691
