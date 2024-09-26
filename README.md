# java-intellij-idea-and-maven

This is a simple project to demonstrate how to create a Java project using IntelliJ IDEA and Maven.

It contains a simple Java class that uses [`picocli`](https://mvnrepository.com/artifact/info.picocli/picocli/4.7.6) to
parse command line arguments and greet the user.

## Executing the application

```shell
$ java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar --help
Usage: java-intellij-idea-and-maven-1.0-SNAPSHOT.jar [-hV] <name> [COMMAND]
A small CLI with subcommands to demonstrate picocli.
      <name>      The name of the user (default: World).
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  hello    Print a 'Hello World!' type of message.
  goodbye  Print a 'Goodbye World!' type of message.
```

```shell
$ java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello --help
Usage: java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello [-hV]
       [-g=<greetings>]
Print a 'Hello World!' type of message.
  -g, --greetings=<greetings>
                  The greetings to address the user (default: Hello).
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
`
```

```shell
$ java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye --help
Usage: java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye [-hV]
       [-f=<farewells>]
Print a 'Goodbye World!' type of message.
  -f, --farewells=<farewells>
                  The farewells to address the user (default: Goodbye).
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
```

