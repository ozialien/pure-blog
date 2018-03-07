# pure-blog

My own blog app implementation for the purpose of PurelyFunctional.tv exercise.
See https://purelyfunctional.tv/functional-programming-career-guide/10-side-projects-resume/
for more examples of good side projects.

Project's github page: https://github.com/jumarko/pure-blog
FIXME: description

## Skeleton

Skeleton of this app has been created by `lein duct` template:

```
lein new duct pure-blog +api +ataraxy +example +postgres +site
```

## Developing

### Setup

When you first clone this repository, run:

```sh
lein duct setup
```

This will create files for local configuration, and prep your system
for the project.

### Environment

To begin developing, start with a REPL.

```sh
lein repl
```

Then load the development environment.

```clojure
user=> (dev)
:loaded
```

Run `go` to prep and initiate the system.

```clojure
dev=> (go)
:duct.server.http.jetty/starting-server {:port 3000}
:initiated
```

By default this creates a web server at <http://localhost:3000>.

When you make changes to your source files, use `reset` to reload any
modified files and reset the server.

```clojure
dev=> (reset)
:reloading (...)
:resumed
```

### Testing

Testing is fastest through the REPL, as you avoid environment startup
time.

```clojure
dev=> (test)
...
```

But you can also run tests through Leiningen.

```sh
lein test
```

## Legal

Copyright © 2018 Juraj Martinka (curiousprogrammer.net)
