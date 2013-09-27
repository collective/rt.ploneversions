rt.ploneversions
================

Retrieve information from dist.plone.org to safely
and easily pin your egg versions.

Motivation
----------

Generally Plone buildouts extend online configuration files with
known good working sets of eggs, which can extend other resources.

This means that your buildout will have to rely on the fact that
the external resources should be available
before it can start its job: if you have network problem you can be lost!

I don't want to cross my finger and wait for those versions to be
retrieved on the net, so I wanted to merge all those
known good working versions in a file.

It is tedious to do it by hand, so I wrote this script.
Enjoy it!

Installation
------------

You can install **rt.ploneversions** with pip or easy_install::

    pip install rt.ploneversions

Usage
-----

Launch the `ploneversions` script
passing a valid Plone version. You can check them here:

 - http://dist.plone.org/release/

Example output (with some ellipses)::

    $ ploneversions 4.3-latest
    ## http://download.zope.org/zopetoolkit/index/1.0.8/ztk-versions.cfg
    zope.annotation = 3.5.0
    ...
    zope.kgs = 1.2.0

    ## http://download.zope.org/Zope2/index/2.13.21/versions.cfg
    Zope2 = 2.13.21
    ...
    zope.testbrowser = 3.11.1

    ## http://download.zope.org/zopetoolkit/index/1.0.8/zopeapp-versions.cfg
    zope.app.applicationcontrol = 3.5.10
    ...
    zope.rdb = 3.5.0

    ## http://dist.plone.org/release/4.3-latest/versions.cfg
    docutils = 0.9.1
    ...
    zc.relation = 1.0


Authors
=======

This product was developed by RedTurtle Technology team.

.. image:: http://www.redturtle.net/redturtle_banner.png
   :alt: RedTurtle Technology Site
   :target: http://www.redturtle.it/
