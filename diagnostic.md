# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
A backend is used to store updates made by the user via the front end and to serve up data to the user when she
requests it from the front end.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
The controller communicates with the model.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because we are focused on creating SPAs in this program.
```

What does C.R.U.D stand for?

```md
Create
Read
Update
Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index, show, create, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. The browser makes the request
2. The web server receives the request
3. The web server's uses routes to find out which controller it should send the request to
4. The router will route the request to the controller - SHOW method in the controller
5. The controller will parse the reuqest and send it to the correct People model
6. THe model will talk to the database, grab the data, sends it back to the controller
7. The controller will return the response to the server
8. THe server will send the response via HTTP back to the user
```

What is the command to generate a new rails-api app?

```bash
bundle install
touch .env
bin/rake secret
*update env file with keys*

```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bin/rake db:drop
bin/rake db:create
bin/rake db:migrate
bin/rake db:seed
bin/rake db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:text age:integer
```
