# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
// The purpose of the backend is to send, store, or receive data that has been requested, created, updated, or deleted.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
// The model is used by the controller to fetch data.
```

Which layer in the MVC pattern communicates with the model?

```md
// The controller communicateds with the model.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
// The view shows a representation of the data that has been created/modified.
```

What does C.R.U.D stand for?

```md
// Create. Read. Update. Delete/Destroy.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
// We can find the CRUD actions in the models. The controllers communicate the action that was requested to the model, and the model runs and returns the result of that action back to the controller.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
// Index, Create, Show, Update, and Delete.
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
// The request from the client of that user is sent to the web server. The web server sents the request to the people controller. The people controller communicates this GET action to the people model to request data for people/1. If there is information/data stored in people/1, this is returned to the people controller by the people model. The people controller relays this data to the people view. This information is sent back to the web server, and the web server sends this information in a form that can be viewed by the client.
```

What is the command to generate a new rails-api app?

```bash
// bin/rails generate
```

What is the command to start an instance of a rails server?

```bash
// bundle exec rails server OR bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
// bin/rails db:drop
bin/rails db:create
bin/rails db:migrate
bin/rails db:seed and bin/rails bd:examples

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
// bin/rails generate scaffold pet name:text age:integer
```
