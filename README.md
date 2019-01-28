# Slowcat

Like `cat`, just slow. Quick and dirty solution to show files slowly or slow down STDIN and output as if typed by a human.

## Why??

Needed a solution to slowly pipe into asciinema so I can have reproducible command line demos.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'slowcat'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install slowcat

## Usage

`slowcat` `{file name}` `{characters per second}` `delay between lines` `fuziness in %`

* `slowcat README.md` - will slowly output the content of README.md
* `cat README.md | slowcat` - will do the same
* `slowcat README.md 40 0.5 1000` - will slowly output the content of README.md at 40 characters per second with 0.5 seconds delay between lines and a fuzzying factor of 1000% (these are the default values)

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/slowcat. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Slowcat project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/slowcat/blob/master/CODE_OF_CONDUCT.md).
