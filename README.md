# RubyRailsFever

A Ruby on Rails application.

<div align="center">
  <img src=".github/assets/github_landing.png" width="1080" height="480" />
</div>

---

## Prerequisites

| Requirement | Version / Install |
|-------------|-------------------|
| Ruby        | `>= 4.0` — check with `ruby -v` |
| Rails       | `8.1.2` — `gem install rails` |
| SQLite3     | Default (or another supported database) |
| Bundler     | `gem install bundler` |

---

## Setup

**1. Install dependencies**

```bash
bundle install
```

**2. Set up the database**

```bash
rails db:setup
```

**3. Run the development server**

```bash
rails server          # default port 3000
rails s -p 4000       # custom port 4000
```

---

## Development

### Key Directories

| Path | Purpose |
|------|---------|
| `app/models` | ActiveRecord models |
| `app/controllers` | Request handling logic |
| `app/views` | ERB templates |
| `config/routes.rb` | Route definitions |

### Generate Resources

```bash
rails generate model User name:string email:string
rails generate controller Home index
```

### Run Migrations

```bash
rails db:migrate
```

---

## Testing

Rails ships with **Minitest** by default:

```bash
rails test
```

---

## Notes

> This project uses the Rails **full-stack framework**, including ORM (ActiveRecord), routing, views, and the asset pipeline.

## DockerImage

```bash
docker pull cureerel/rubyrailsfever:1.0.0
```