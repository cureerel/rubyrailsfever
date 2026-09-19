# Rails Application Structure & Setup Steps

## Important Files

- **Layout file:** `views/layouts/application.html.erb`
- **Route registration:** `config/routes.rb`

---

## Project Structure

```text
Rails application
│
├── Backend
│   ├── Models
│   ├── Controllers
│   ├── Services
│   ├── Jobs
│   └── Database
│
└── Frontend
    ├── Views
    ├── JavaScript
    ├── assetts/stylesheets + images
    └── Images
```

---

## Setup Steps

### 1. Controller
Create your controller in:

```
app/controllers/
```

### 2. View
Create the corresponding view for each route:

```
app/views/<route-x>/<x>.html.erb
```

### 3. Stylesheets
Place CSS assets in:

```
app/assets/stylesheets/
```

---

## Backend & Database

### 4. Model & Database
Define models in:

```
app/models/
```

Run migrations to set up the database:

```bash
rails db:migrate
```

### 5. Database Calls
Query the database from your controller (or via a service):

```ruby
# app/controllers/x_controller.rb
def index
  @records = YourModel.all
end
```

For complex queries, extract logic into a service:

```
app/services/
```

### 6. Routes
Register routes in:

```ruby
# config/routes.rb
Rails.application.routes.draw do
  resources :your_resource
end
```

### 7. Background Jobs
For async tasks, place jobs in:

```
app/jobs/
```

---
