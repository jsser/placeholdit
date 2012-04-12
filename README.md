# Placeholdit

A helper for creating placeholder images via http://placehold.it. Works with Rails, or without.

## Installation

Add this line to your application's Gemfile:

    gem 'placeholdit'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install placeholdit

## Usage

A basic 500x500 placeholder image:
		
		$ <%= placeholdit_image_tag "500" %>

A basic 250x250 placeholder image:
		
		$ <%= placeholdit_image_tag "250x250" %>

The same placeholder image with custom text:

		$ <%= placeholdit_image_tag "250x250", text: "Buy me!" %>

The same placeholder image with a blue background:

		$ <%= placeholdit_image_tag "250x250", text: "Buy me!", background_color: '#004eff' %>

The same placeholder image with a blue background and red text (not recommended):

		$ <%= placeholdit_image_tag "250x250", text: "Buy me!", background_color: '#004eff', text_color: '#ff0000' %>

Alternatively, simply calling placeholdit will work just the same:

		$ <%= placeholdit "250x250", text: "Look at me!" %>


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
