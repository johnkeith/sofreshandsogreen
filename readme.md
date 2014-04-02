## So Fresh and So Green Octopress Theme

So Fresh and So Green is a straightforward Octopress theme. It focuses on excellent readability.

![So Fresh and So Green](http://gdurl.com/i4Wr)

To this end, the Octopress sidebar is disabled and the navigation is affixed to the top.

Click here for a [demo](http://www.sofreshandsogreen.herokuapp.com)!

Improvements will be forthcoming, as inspiration strikes!

### Step 1) 

Install this bad boy. Navigate to the root of your Octopress install, then run these two commands.

	$ git clone https://github.com/johnkeith/sofreshandsogreen.git .themes/sofreshandsogreen
		
	$ bundle exec rake install['sofreshandsogreen']

Or, if zsh is giving you grief, use this instead of the previous line.
		
	$ bundle exec rake install\['sofreshandsogreen'\]

### Step 2) 

Make these changes to your _config.yml. This will remove the sidebar and make the layout look correct.

	default_asides: []
	sidebar: collapse

### Step 3) 

If you want to add a picture of yourself to the homepage as in the [demo](http://www.johnkeith.us), you need to replace the portrait.jpg in the source/images folder of your Octopress installation. Then, add the following somewhere in your _config.yml.

	portrait: true

This will enable your smiling countenance on the blog's main page. (The entire header is disabled by default on pages and individual post pages by using a different layout for these pages, aptly entitled default_no_header.html). 

### (Optional) Step 4)

Make your codeblocks look better with CodeRay! Add these gems to your gemfile.

	gem 'kramdown'
	gem 'coderay'

Then, back at the terminal, run this command to install Coderay.

	$ bundle install

And lastly, hop over to your _config file and replace your Markdown line with the following. 

~~~
markdown: kramdown
kramdown:
	use_coderay: true
	coderay:
		coderay_line_numbers: nil
		coderay_css: class
~~~

For a great explanation of Coderay and kramdown, see [Codebykat's post](http://blog.codebykat.com/2013/05/23/gorgeous-octopress-codeblocks-with-coderay/) on the subject.

### Extra

Oh yeah, Font awesome is included. Have fun!
