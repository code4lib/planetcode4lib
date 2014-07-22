# planet.code4lib.org

[Planet Code4Lib](http://planet.code4lib.org/) aggregates feeds and blogs of interest to the [Code4Lib](http://code4lib.org/) community.  It uses [Planet Venus](https://github.com/rubys/venus).

## Installation

    > git clone git@github.com:code4lib/planetcode4lib.git
    > cd planetcode4lib
	> git submodule init
	> git submodule update
	> ./venus/planet.py --verbose

The generated files will be in `output/`.

To test it with one feed, run

    > ./venus/planet.py --verbose test.ini

## Adding a feed

Additions are welcome!

Email [William Denton](mailto:wtd@pobox.com) or submit a pull request modifying `config.ini`.
