# Scala Devcontainer

A [VS Code](https://code.visualstudio.com) [devcontainer](https://containers.dev) 
to be used for [Scala](https://www.scala-lang.org) (Version 3) development. The
devcontainer includes all required tools and example code as well as tests to get
quickly started or try out Scala.

## Running the devcontainer

To run the devcontainer, check out the the git repository, open the folder in
VS Code and execute the task `>Dev Containers: Open Folder in Container...`.

You can also use GitHub Codespaces to run the devcontainer. On GitHub, open the
git repository, click on `Code`, then `Codespaces`, and select `Create codespace
on main`.

## Using Metals

The [Metals](https://scalameta.org/metals/) extension is installed as part of this 
devcontainer and is the recommended way to run, test and debug Scala files. 
To get started, run

```
>Metals: Import build 
```

from the VS Code command palette.

## Running from the command line

As an alternative to Metals, the [sbt](https://www.scala-sbt.org) build tool is 
also available from the codespace terminal. To compile the provided Hello World 
example, run the following command in the VS Code terminal:

```
$ sbt compile
```

To execute the resulting program, use the following command:

```
$ sbt run
```
### Starting a Scala script

Scala can be used to write scripts. If you want to try out using Scala in scripts,
you can start with the file `scripts.scala`. To run the script, run the following
command:

```
$ scala script.scala
```

### Running tests

The devcontainer includes a basic sketch of [ScalaTest](https://www.scalatest.org)
for unit testing. To run the provided example tests, execute the following command:

```
$ sbt test
```