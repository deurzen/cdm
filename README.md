CDM: The Console Display Manager
================================

Adds on top of `pale3/cdm-0.7`:

	- invocate bin from binlist (e.g. `startx ${bin} -- ${serveropts}`, where ${bin} comes from cdm selection)

Invocation
----------

To run cdm, use

    $ cdm [RCFILE]

cdm tries to source configuration files in this order, and uses the first
existing one:

    [RCFILE specified on command line]
    $HOME/.cdmrc
    /etc/cdmrc

To autostart cdm when you log in your account, copy the content of
/usr/share/doc/cdm/profile.sh to the tail of your shell profile (~/.profile,
etc.).


Customisation
-------------

See /etc/cdmrc for examples.


Copying
-------

Copyright (C) 2009-2012, Daniel J Griffiths <dgriffiths@ghost1227.com>
Thanks to:

    Andrwe          beta-testing and submitting the fix for the all
                    important X incrementation function
    brisbin33       code cleanup
    tigrmesh        finding a critical issue with the gnome-session handler
    Profjim         several incredibly useful patches
    lambchops468    consolekit and hibernation patches
    CasperVector    Massive rearchitecturing and code sanitation

Licensed under GPLv2+
