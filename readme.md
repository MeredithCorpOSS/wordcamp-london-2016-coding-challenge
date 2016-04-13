##Time Inc. Wordcamp London 2016 Coding Challenge
===================

### How to Enter!

*Fix this broken wordpress plugin to enter into a draw for a Raspberry Pi 3 or 6 months Spotify sub.*

__Enter here: http://j.mp/TimeUKCodeComp__

It is a sample [Echo.js](http://toddmotto.com/echo-js-simple-javascript-image-lazy-loading/) based lazy load plugin for WordPress with some failing tests, see if you can fix them and send us a PR to win a Raspberry Pi 3 or 6 months Spotify subscription. Don't worry if you can't get them all passing, just send us your best effort.

It is built using the WordPress coding standards, is designed to be very lite weight on system resources.

Good Luck!!!

### How to run the tests

You should be able to run the tests using a few simple steps, if you need a hand here is a quick guide to running the tests:

1. Ensure you have all the dependencies, at a minimum you will need:
 * git
 * subversion
 * phpunit
 * php5
 * mysql server
1. Checkout the code from github
1. Setup the tests be executing `./tests/bin/install-wp-tests.sh timeinc-wp-coding-challenge root MYSQLPASSWORD localhost 4.4.2` repalcing MYSQLPASSWORD with your root password or just type `''` if you don't have one
1. Run the tests by executing `phpunit`

#### Running on a new DigitalOcean Droplet

This guide is based on using the 14.04.4 Digital Ocean image, use the $5 size and any location to create it. This droplet is only intended for the coding challenge, always remember to set a password for the MySQL root user!

1. Create a [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-create-your-first-digitalocean-droplet-virtual-server) droplet
1. Login to your new server
1. Update the server by executing the command `apt-get update`
1. Install required applications by executing the command `apt-get install -y git subversion phpunit php5 php5-mysql mysql-server-5.5` Don't set a root mysql password (just press enter)
1. Setup your github.com [SSH key](https://help.github.com/articles/generating-an-ssh-key/)
1. Fork https://github.com/TimeIncOSS/wordcamp-london-2016-coding-challenge
1. Checkout the code by executing the command `git clone git@github.com:YOURGITHUBUSERNAME/wordcamp-london-2016-coding-challenge.git`
1. Change into your checkout by executing the command `cd wordcamp-london-2016-coding-challenge/`
1. Install dependencies be executing the command `./tests/bin/install-wp-tests.sh timeinc-wp-coding-challenge root '' localhost 4.4.2`
1. Run the tests by executing the command `phpunit`
1. Fix the tests (you're on your own here but feel free to ask us for help!)
1. Commit and push your shiny bug free code
1. Send us a [Pull Request](https://help.github.com/articles/creating-a-pull-request/)
1. ...
1. Profit!
1. Don't forget to [destroy](https://www.digitalocean.com/community/tutorials/the-digitalocean-control-panel#destroy) your droplet to avoid incurring unnecessary charges

### Disclaimer 

This plugin is for the Wordcamp London 2016 Coding Challenge and will be removed on 1st May 2016.

DO NOT USE THIS PLUGIN FOR PRODUCTION SYSTEMS ;-)

### License

The Echo.js Lazy Load is licensed under the GPL v2 or later.

> This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License, version 2, as
published by the Free Software Foundation.

> This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

> You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
