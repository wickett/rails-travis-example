[![Build Status](https://travis-ci.org/wickett/rails-travis-example.svg?branch=master)](https://travis-ci.org/wickett/rails-travis-example) [![Code Climate](https://codeclimate.com/github/secure-pipeline/rails-travis-example.png)](https://codeclimate.com/github/secure-pipeline/rails-travis-example)

# Rails Travis Example

## Overview
This repo contains a Ruby on Rails Application that is being tested with Travis CI.  Travis CI is running security tests and attacks against the application. This is meant to be an example of how to setup security testing inside your CI environment.

## About the Ruby on Rails Application

The app, Triage, was written by [Matt Konda](https://github.com/mkonda) and he awesomely donated it to be used for the secure pipeline project as the demo rails application.  Thanks Matt! Please see [Triage's README.md](https://github.com/Jemurai/triage/blob/master/README.md) for more infomation on the application. 

### Branches

Note that Triage *intentionally* has two branches:  
* security_errors :  contains many security holes
* security_fixes : attempts to illustrate how to fix the holes

### Setup

Once cloned, you should only have to: 
```bash
$ bundle install
$ rake db:migrate
$ ./set_token.sh
$ bundle exec start_services
```

The app should be responding on http://localhost:3000

## License

This repo and the entire secure-pipeline organization is licensed under the [MIT license](http://opensource.org/licenses/mit-license.php).
Triage is licensed under the [MIT license](http://opensource.org/licenses/mit-license.php).
Please see Triage's main repo for more information: https://github.com/Jemurai/triage
