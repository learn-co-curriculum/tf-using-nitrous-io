## PC/Chrome OS: Using Nitrous.io

If you don't currently have access to a mac, the majority of the work here can be done using an IDE (Interactive Development Environment) called Nitrous.io. Below you'll find the steps you need to take in order to set up your development 'box'.

### Initial Set-Up
+ Navigate to and sign up for [nitrous.io](https://www.nitrous.io/). For simplicity's sake, I'd recommend signing up with github.

+ Create a Ruby/Rails box and give it a name.

![box](https://s3.amazonaws.com/after-school-assets/nitrous-box.png)

+ Wait for the box to 'provision' and open up.

+ You'll now be in the IDE. It will look something like this:

![ide](https://s3.amazonaws.com/after-school-assets/nitrous-ide.png)

### Connecting to Github
+ Finally, to set up a connection with your github account (so you can clone/push/pull), head click on the 'boxes' link on the top right of the screen. Open up your box, and click 'reveal public key'. Copy the public key.

![public-key](https://s3.amazonaws.com/after-school-assets/copy-public-key.png)

+ Head to GitHub, and click on your settings (the gear icon). Click 'SSH keys', and then 'Add SSH key'. Give your key a title (like 'nitrous'), and paste in the copied ssh key string. Save.

### Install your first Gem

+ Ok, back to the IDE to install the learn gem.

This gem isn't open-sourced, so we won't be downloading it from RubyGems.org, which is where most gems are hosted. Before we download it, we will need to specify where it's coming from, which is a private server at Flatiron. Type this into your command line:

`gem sources -a http://flatiron:33west26@gems.flatironschool.com/`

Next, download the gem:

`gem install learn-co`

The learn gem will allow us to run the tests for challenges and labs. It's based off of RSpec, a popular testing framework in Ruby, but it does a bit more like help track your progress on labs.

Go ahead and install RSpec too: `gem install rspec`

Normally when we run our tests, we would type rspec, but to run the tests for challenges and labs, you'll type learn into your command line instead, within the root directory of the challenge/lab.

+ Done! In the console, you'll now be able to fork and clone repositories from GitHub.
