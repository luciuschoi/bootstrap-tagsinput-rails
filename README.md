# Bootstrap::Tagsinput::Rails

Original Git source - https://github.com/timschlechter/bootstrap-tagsinput

To gemify the assets of `bootstrap-tagsinput` jQuery plugin for Rails >= 3.1

[![Gem Version](https://badge.fury.io/rb/bootstrap-tagsinput-rails.png)](http://badge.fury.io/rb/bootstrap-tagsinput-rails)

## Compatibility

Designed for Bootstrap 2.3.2 and 3

## Installation

Add this line to your application's Gemfile:

    gem 'bootstrap-tagsinput-rails'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install bootstrap-tagsinput-rails

## Usage

in app/assets/application.js

```
//= require bootstrap-tagsinput
```

in app/assets/application.css

```
*= require bootstrap-tagsinput
```

in form view, you should add `data-role='tagsinput'` within input tag as the follows: for example, in `simple-form` view template,

```
<%= f.input :tag_list, input_html:{data:{role:'tagsinput'}} %>
```

Or if using Rails 4 with Bootstrap, use the following,

```
<%= f.text_field :tag_list, 'data-role'=>'tagsinput' %>
```

That's it

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
