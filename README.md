# PPC Sloth (Ruby on rails)

PPC Sloth is a quick and dirty keyword analyzer for Amazon Search Term Reports. It'll
help in creating better advertising campaigns by optimizing keywords.

## Basic Overview

    bundle install
    rake db:reset
    rails s

Get a database dump file and run:

    pg_restore --verbose --clean --no-acl --no-owner -d ppc_sloth_development DUMPFILE # Make sure to substitute DUMPFILE with the correct file name.
    rake db:migrate

The seeds file is a decent representation of a typical production database with
randomized data. If running it for the first time with `rake db:reset`, this should
already be loaded. Otherwise run:

    rake db:seed

##### Export local database

    pg_dump -Fc --no-acl --no-owner ppc_sloth_development > local.dump

## Where to find things

todo

#### The app interface

* Dashboard
* Campaigns

## Future Goals

* Add Users
* Admins
* ...