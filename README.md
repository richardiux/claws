## Command Line AWS

This tool provides a simple and powerful way to interact with the hosts in your Amazon Web Services
account via the command line.  An example of its usage appears below:

* It provides a text based interface of the status of your hosts like similar to the AWS web console:

![Instances](http://i.imgur.com/VEC8V.png)

* It gives you a choice of which host to connect to and invokes the proper ssh command:

![Connecting](http://i.imgur.com/b6ieS.png)

### Installation

It is up on rubygems.org so add it to your bundle in the Gemfile

```bash
gem 'claws'
```

or do it the old fashioned way:

```bash
gem install claws
```

After you have the gem installed you will need to _initialize_ it to install a configuation file:

```bash
claws --init
```

### Usage

Once the initial configuration is completed you can simply run claws from the command line:

```bash
claws
```

The full list of options includes:

```bash
Usage: claws [options]
    -s, --status-only                Display host status only and exit
    -c, --choice N                   Enter the number of the host to automatically connect to
    -i, --init                       Install the default configuration file for the application
```

### To Do

* Add filtering by regular expression for any field

* Integrate with your projects Capistrano definitions so that one can filter by environment and
  roles.

* Add RDS and ELB support

### License

Copyright (c) 2011-2012 Wes Bailey

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute,
sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial
portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT
NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
