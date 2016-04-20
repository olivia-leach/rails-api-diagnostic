# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
One purpose of a backend is to allow users on the same web app to interact with each other. Without a backend, users would not be able to do this, thus limiting what our web app is able to do. Another purpose of a backend is to store data that can persist over time.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because we build our own front-end 'views' with HTML/JavaScript, etc.
```

What does C.R.U.D stand for?

```bash
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, create, show, update, destory
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
* The server receives the GET requests and uses routes to find out which controller to use.
* The web server then uses the dispatcher to create a new controller, call the action and pass the parameters.
* Controllers parse user requests and tell the model to perform the request.
* The model talks to the database, stores and validates data, and performs the business logic.
* The model returns a response to the controller.
* The controller returns the response body and metadata to the server.
* The server combines the raw data into an HTTP response and sends it to the user.
```

What is the command to generate a new rails-api app?

```bash
rails-api new app_name -T --database=postgresql
```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
* rake db:drop
* rake db:create
* rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails-api g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
* Serializers make apps safer by hiding data
* Serializers make it easy to change JSON presentation logic without affecting underlying model logic
```
