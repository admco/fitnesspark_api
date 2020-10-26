# FitnessparkApi

You can use this Gem to get data from the [Fitnesspark API](https://www.fitnesspark.ch/).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'fitnesspark_api'
```

And then execute:

```bash
$ bundle install
```

Or install it yourself as:

```bash
$ gem install fitnesspark_api
```

## Usage


```ruby
require 'fitnesspark_api'

FitnessparkApi.stores # returns a hash with base data of all centers
# => {"stores"=>[{"localized_slugs"=>{"de"=>"activ-fitness-acacias", "it"…

FitnessparkApi.store('fitnesspark-eichstaette') # returns a hash with detailed data of a center
# => {"markets"=>[{"closing_date"=>nil, "media"=>…

FitnessparkApi.visitors('fitnesspark-eichstaette') # returns a hash with visitor data
# => {"centerId"=>12, "centerIdTac"=>45, "currentVisitors"=>169, "maxVisitors"=>300}
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/alexanderadam/fitnesspark_api. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/alexanderadam/fitnesspark_api/blob/master/CODE_OF_CONDUCT.md).


## Code of Conduct

Everyone interacting in the FitnessparkApi project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/alexanderadam/fitnesspark_api/blob/master/CODE_OF_CONDUCT.md).
