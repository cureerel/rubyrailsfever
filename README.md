# RubyFever


A Ruby on Rails application.

## Prerequisites

- Ruby >= 4.0 (check with `ruby -v`)
- Rails 8.1.2 (`gem install rails`)
- SQLite3 (default) or another supported database
- Bundler (`gem install bundler`)

## Setup

Install dependencies:

```bash
bundle install
```

Set up the database:

```bash
rails db:setup
```

Run the development server:

```bash
rails server # default 3000
rails s -p 4000 # specified 4000
```


## Development

* Models: `app/models`
* Controllers: `app/controllers`
* Views: `app/views`
* Routes: `config/routes.rb`

Generate resources:

```bash
rails generate model User name:string email:string
rails generate controller Home index
```

Run migrations:

```bash
rails db:migrate
```

## Testing

Rails comes with Minitest by default:

```bash
rails test
```

## Notes
This project uses Rails’ **full-stack framework**, including ORM (ActiveRecord), routing, views, and assets.
---
