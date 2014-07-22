# planet.code4lib.org

[Planet Code4Lib](http://planet.code4lib.org/) aggregates feeds and blogs of interest to the [Code4Lib](http://code4lib.org/) community.  It uses [Planet Venus](https://github.com/rubys/venus).

## Installation generally

    > git clone git@github.com:code4lib/planetcode4lib.git
    > cd planetcode4lib
	> git submodule init
	> git submodule update
	> ./venus/planet.py --verbose

The generated files will be in `output/`.

To test it with one feed, run

    > ./venus/planet.py --verbose test.ini

## Installation on the code4lib.org server

Downloading and cloning is done over HTTPS so it's as generic as possible.  No updates are to be made on the server; they should be made locally, pushed to GitHub, then pulled down.

	> # Become the c4l user
    > cd /var/www/code4lib.org/planet_new
    > git clone https://github.com/code4lib/planetcode4lib.git
    > cd planetcode4lib
	> git submodule init
	> git submdule update
	> ./venus/planet.py --verbose --expunge

To update:

    > # Become the c4l user
    > cd /var/www/code4lib.org/planet_new/planetcode4lib
	> git pull

## Adding a feed

Additions are welcome!

Email [William Denton](mailto:wtd@pobox.com) or submit a pull request modifying `config.ini`.
