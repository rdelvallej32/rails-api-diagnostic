# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The back-end can store different states of a webpage over time as a result of the
ability to store data that can be specific to the user (i.e. profile, email, etc.)
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model layer fetches the data from the database
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller communicates with the model and the database also communicates with the model.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
The view causes the back-end to have mutiple template-views for specific actions
that occur on the webpage, which will mean that the page
will have to reload to show the new view. It is not very SPA.
```

What does C.R.U.D stand for?

```bash
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
In the controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, create, show, update, destroy
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- Ajax sends GET request to server
- Server hands person/1 GET request to Person controller
- Person Controller sends person/1 GET request to Person Model
- Person Model asks database for person/1 database
- Database sends person 1 data to Person Model
- Person Model sends person 1 data to Person controller
- Person Controller sends person 1 data to server
- Server sends person 1 data back to client
```

What is the command to generate a new rails-api app?

```bash
install rails-api
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
- rake db: drop
- rake db: create
- rake db: migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails-api g scaffold pet name:string age:string
```

List two advantages of using serializers? (2 bullet points)

```bash
- Its safer/secure for important information (i.e. passwords)
- Its simple to use because you are rendering information (i.e object) into JSON
that easily facilitates the transportation of the object to a database to store
it.
```
