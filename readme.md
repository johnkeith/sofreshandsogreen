## So Fresh and So Green Octopress Theme

So Fresh and So Green is a straightforward Octopress theme. It focuses on excellent readability.

To this end, the Octopress sidebar is disabled and the navigation is affixed to the top.

Click here for a [demo](http://www.johnkeith.us)!

Improvements will be forthcoming, as inspiration strikes!

### Step 1) 

Install this bad boy. 

	$ git clone https://github.com/johnkeith/sofreshandsogreen.git .themes/sofreshandsogreen
		
	$ bundle exec rake install['sofreshandsogreen']

Or, if zsh is giving you grief.
		
	$ bundle exec rake install\['sofreshandsogreen'\]

### Step 2) 

Make these changes to _config.yml. This will remove the sidebar.

	default_asides: []
	sidebar: collapse

Also, replace your Markdown settings in your _config file with these lines, which will help make step 3 successfully prettify our code snippets.

~~~
markdown: kramdown
kramdown:
	use_coderay: true
	coderay:
		coderay_line_numbers: nil
		coderay_css: class
~~~

### Step 3)

Make your codeblocks look better with CodeRay! Add these gems to your gemfile.

	gem 'kramdown'
	gem 'coderay'

Then, back at the terminal, run this command to install Coderay.

	$ bundle install

For a great explanation of Coderay and kramdown, see [Codebykat's post](http://blog.codebykat.com/2013/05/23/gorgeous-octopress-codeblocks-with-coderay/) on the subject .

Also, if you want to add a picture of yourself to the homepage as in the [demo](http://www.johnkeith.us), you need replacing the portrait.jpg in the source/images folder of your Octopress installation. Then, add to your _config.yml:

	portrait: true

In order to enable your smiling countenance on the blog's main page. (The entire header is disabled by default on pages and individual post pages). 

Oh yeah, Font awesome is included. Have fun!
