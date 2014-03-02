# So Fresh and So Green Octopress Theme

So Fresh and So Green is a straightforward Octopress theme. It focuses on excellent readability.  

To this end, the Octopress sidebar is disabled and the navigation is affixed to the top.

Improvements will be forthcoming, as inspiration strikes!

### Step 1) Install this bad boy. 

	$ git clone https://github.com/johnkeith/sofreshandsogreen.git .themes/sofreshandsogreen
		
	$ bundle exec rake install['sofreshandsogreen']

Or, if zsh is giving you grief.
		
	$ bundle exec rake install\['sofreshandsogreen'\]

### Step 2) Make these changes to _config.yml. This will remove the sidebar.

	default_asides: []
	sidebar: collapse

### Step 3) Make your codeblocks look better with CodeRay! Add these gems to your gemfile.

	gem 'kramdown'
  gem 'coderay'

Then, back at the terminal, run this command to install Coderay.

	$ bundle install

Oh yeah, Font awesome included, so have fun!
