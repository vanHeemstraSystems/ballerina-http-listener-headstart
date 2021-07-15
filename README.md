ballerina-http-listener-headstart
# Ballerina HTTP Listener - Headstart

Based on "Creating a Service in Ballerina - Tutorial" at https://www.youtube.com/watch?v=NxyIKoHl3Dw

## 100 - Prerequisites

- Docker Engine, see
- Ballerina, see
- Visual Studio Code (Optional)
- Visual Studio Code Extension for Ballerina (Optional)

## 200 - Creating a Ballerina Package

Inside ```containers/sample/``` directory run below command to create a new Ballerina package (here: called ```pickagift```):

```
$ cd containers/sample
$ bal new pickagift
Created new Ballerina package 'pickagift' at pickagift.
```

The content of the new directory 'pickagift' is as follows:

```
containers/
  sample/
    pickagift/
      .gitignore
      Ballerina.toml
      main.bal
```

```.gitignore``` contains:

```
target
```

```Ballerina.toml``` contains:

```
[build-options]
observabilityIncluded = true
```

```main.bal``` contains:

```
import ballerina/io:

public function main() {
  io:printlin("Hello, World!");
}
```

Try running the new Ballerina package with the following command:

```
$ cd packagift
$ bal run


```

more ...
