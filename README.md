# Ruby on Rails

Rails is a web-application framework that includes everything needed to create database-backed web applications according to the Model-View-Controller (MVC) pattern.

## Getting Started

Here I'm creating a new demo web application on rails.

## Installation

Before creating a new project on rails, you need to install:

First, update your package manager:

```
    $ sudo apt-get update
```

Install curl in order to get the RVM (Ruby Version Manager). RVM used to manage your ruby and rails version.

```
    $ sudo apt-get install curl
    $ \curl -L https://get.rvm.io | bash -s stable --ruby
```

If you getting the error which is rvm no public key, you must run this command to get the public key.

```
    $ gpg2 --keyserver hkp://keys.gnupg.net --recv-keys D39DC0E3
```

In order to use RVM command, you may need to:

```
    $ source /home/ruby/.rvm/scripts/rvm
```

# Install Ruby

by using RVM

```
    $ rvm get stable --autolibs=enable
    $ rvm install ruby
```

# Install the Node.js

a javascript runtime has been needed on Ubuntu workspace after Rails 3.1 version

```
    $ sudo apt-get install nodejs
```

If you dont install the Node.js, you may need to include the gem for each application you build.

```
    $ gem 'therubyracer'
```

# RVM Gemsets

Display a list of gemsets:

# RVM’s Global Gemset
See what gems are installed in the “global” gemset:

```
    $ rvm gemset use global
    $ gem list
```

# Install Bundler gem

an essential tool for managing gems when developing and running Rails applications.

```
    $ gem install bundler
```
# Install Nokogiri gem

is a gem that is a dependency for many other gems. Nokogiri is a gem that requires compilation for your specific operating system.

```
    $ gem install nokogiri
```

# Install Rails

```
    $ rvm use ruby-2.4.1@rails5.0 --create
```

## Example

Create a workspace

```
    $ mkdir workspace
    $ cd workspace
```

Create new application

```
    $ rails new demo --skip-test-unit
```

Run the servers

```
    $ cd demo
    $ bundle
    $ bin/rails server
```

Open the browser and type the address as: localhost:3000.. Enjoy ruby on Rails.

## Version

Please take note that might minor changes of syntax on different version

```
    ruby     ==   2.4.1
    rails    ==   5.0
    rvm      ==   1.29.3
    curl     ==   7.47
    nodejs   ==   4.2.6
```

## Error

You may face some command is not installed,

```
    1. Open console
    2. Select Edit -> Profile Preferences
    3. Select tab: Title and Command
    4. Check box 'Run command as a login shell'
    5. Restart terminal
```
