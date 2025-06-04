# OmniAuth Monday

This forks the official OmniAuth strategy for authenticating to Monday.

## Installation

```ruby
gem 'omniauth-monday'
```

## Basic Usage Rails

In `config/initializers/monday.rb`

```ruby
  Rails.application.config.middleware.use OmniAuth::Builder do
    provider :monday, ENV['MONDAY_CLIENT_ID'], ENV['MONDAY_CLIENT_SECRET']
  end
```
