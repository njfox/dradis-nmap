# Nmap plugin for Dradis

[![Build Status](https://secure.travis-ci.org/dradis/dradis-nmap.png?branch=master)](http://travis-ci.org/dradis/dradis-nmap) [![Code Climate](https://codeclimate.com/github/dradis/dradis-nmap.png)](https://codeclimate.com/github/dradis/dradis-nmap.png)

Upload Nmap files into Dradis.

The add-on requires [Dradis CE](https://dradisframework.org/) > 3.0, or [Dradis Pro](https://dradisframework.com/pro/).

## Installation
1. Clone the develop branch:
```
$ git clone -b develop/nmap_filtering https://github.com/njfox/dradis-nmap.git
```
2. Stop the Dradis server
3. Switch into the Dradis install directory, comment out the existing `dradis-nmap` gem in the Dradis `Gemfile.plugins` file and point it to the new installation:
```
$ cd path/to/dradis/install
$ nano Gemfile.plugins

 22 gem 'dradis-acunetix',    '~> 3.6', github: 'dradis/dradis-acunetix'
 23 gem 'dradis-brakeman',    '~> 3.6', github: 'dradis/dradis-brakeman'
 24 gem 'dradis-burp',        '~> 3.6', github: 'dradis/dradis-burp'
 25 gem 'dradis-metasploit',  '~> 3.6', github: 'dradis/dradis-metasploit'
 26 gem 'dradis-nessus',      '~> 3.6', github: 'dradis/dradis-nessus'
 27 gem 'dradis-nexpose',     '~> 3.6', github: 'dradis/dradis-nexpose'
 28 gem 'dradis-nikto',       '~> 3.6', github: 'dradis/dradis-nikto'
 29 #gem 'dradis-nmap',        '~> 3.6', github: 'dradis/dradis-nmap'
 30 gem 'dradis-ntospider',   '~> 3.6', github: 'dradis/dradis-ntospider'
 31 gem 'dradis-openvas',     '~> 3.6', github: 'dradis/dradis-openvas'
 32 gem 'dradis-qualys',      '~> 3.6', github: 'dradis/dradis-qualys'
 33 gem 'dradis-zap',         '~> 3.6', github: 'dradis/dradis-zap'
 34 gem 'dradis-nmap',        path: '/path/to/dradis-nmap'
```
4. Install gems and start Dradis:
```
$ bundle install
$ bundle exec rails server
```
## More information

See the Dradis Framework's [README.md](https://github.com/dradis/dradisframework/blob/master/README.md)


## Contributing

See the Dradis Framework's [CONTRIBUTING.md](https://github.com/dradis/dradisframework/blob/master/CONTRIBUTING.md)


## License

Dradis Framework and all its components are released under [GNU General Public License version 2.0](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) as published by the Free Software Foundation and appearing in the file LICENSE included in the packaging of this file.


## Feature requests and bugs

Please use the [Dradis Framework issue tracker](https://github.com/dradis/dradis-ce/issues) for add-on improvements and bug reports.
