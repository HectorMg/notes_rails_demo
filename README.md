# Notes App

## About

The Notes App is a Ruby on Rails application designed to give a quick
introduciton to Ruby on Rails for beginners. As such, the application is
very simple, light and easy to reproduce.

The Notes App was created specifically to be used as a demo application
during an Intro to Ruby on Rails workshop @TecDeMonterrey 2018.

## Running the app


### Installing Ruby on Rails

We'll be using Ruby on Rails during the Workshop, so it's important that you install the newest (stable) version of Rails (Rails 5.1.4 at the moment of writing this).

You can find a guide to installing Ruby on Rails [here](http://guides.rubyonrails.org/getting_started.html).

### Clone the project

First of all, make sure you have `git` installed. Git is what's known as version control software, which will help us clone this and other projects to your machine.  To check if it is installed, open a terminal window (macOS, linux) or the command prompt (Windows) and execute the `--version` command. 

```bash
$ git --version
```

If git is installed, you'll see something like:

```bash
git version 2.7.3
```

Don't worry if the version doesn't match exactly.

If you do have `git` installed, go the next step. If you don't (you get something along the lines of "git is not installed" or "couldn't find command 'git' ", then take a look at [this guide](https://gist.github.com/derhuerst/1b15ff4652a867391f03) and then come back.

Now, run the following command to clone the project to your machine.

```bash
$ git clone https://github.com/HectorMg/notes_rails_demo.git
```

The above is the way to clone using the HTTPS protocol. If you're more advanced (or have used Git enough to have SSH setup), you may instead use the SSH version of the command:

```bash
$ git clone git@github.com:HectorMg/notes_rails_demo.git
```

Both commands do the exact same thing, the second one just takes more configuration the first time.

### Installing Dependencies

Once you've cloned this repository, change into the project's repository and install the project's 'gems' (Ruby's name for libraries or dependencies).

```bash
$ cd notes_rails_demo
$ bundle install
```

The `bundle install` command may take a while to finish, be patient!

### Migrate the Database

This application has a couple database models that are important for its execution, so go ahead, create and migrate the database!

```bash
$ rails db:create
$ rails db:migrate
```

### Start the Application

Once you get control of your terminal back, go ahead and start the application with the following command!

```bash
$ rails start
```

Or if you're really lazy

```bash
$ rails s
```

You should see something like:

```
=> Booting Puma
=> Rails 5.1.4 application starting in development 
=> Run `rails server -h` for more startup options
Puma starting in single mode...
* Version 3.11.2 (ruby 2.5.0-p0), codename: Love Song
* Min threads: 5, max threads: 5
* Environment: development
* Listening on tcp://0.0.0.0:3000
Use Ctrl-C to stop
Started GET "/" for 127.0.0.1 at 2018-02-09 18:52:00 -0600
```

Now go to your favorite browser, hit up `localhost:3000` on the address bar and enjoy!





