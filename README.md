easy-example-module-cmd
===========
[![Build Status](https://travis-ci.org/DANS-KNAW/easy-example-module-cmd.png?branch=master)](https://travis-ci.org/DANS-KNAW/easy-example-module-cmd)

<!-- Remove this comment and extend the descriptions below -->


SYNOPSIS
--------

    easy-example-module-cmd (synopsis of command line parameters)
    easy-example-module-cmd (... possibly multiple lines for subcommands)


DESCRIPTION
-----------

An example module generated with easy-module-archetype stripped down to only command line interface.


ARGUMENTS
---------

    Options:

    --someOption  <arg>   Description of the option
            --help                Show help message
            --version             Show version of this program

EXAMPLES
--------

    easy-example-module-cmd -o value


INSTALLATION AND CONFIGURATION
------------------------------


1. Unzip the tarball to a directory of your choice, typically `/usr/local/`
2. A new directory called easy-example-module-cmd-<version> will be created
3. Add the command script to your `PATH` environment variable by creating a symbolic link to it from a directory that is
   on the path, e.g. 
   
        ln -s /usr/local/easy-example-module-cmd-<version>/bin/easy-example-module-cmd /usr/bin



General configuration settings can be set in `cfg/application.properties` and logging can be configured
in `cfg/logback.xml`. The available settings are explained in comments in aforementioned files.


BUILDING FROM SOURCE
--------------------

Prerequisites:

* Java 8 or higher
* Maven 3.3.3 or higher

Steps:

        git clone https://github.com/DANS-KNAW/easy-example-module-cmd.git
        cd easy-example-module-cmd
        mvn install
