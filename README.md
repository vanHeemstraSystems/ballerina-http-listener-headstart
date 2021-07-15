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
Compiling source
  willemvanheemstra/pickagift:0.1.0
  
Running executable

Hello World!
```

Now we will be making use of the search API of [Apple](www.apple.com)'s online music store called "iTunes", as documented at https://affiliate.itunes.apple.com/resources/documentation/itunes-store-web-service-search-api/

![iTunes_API](https://user-images.githubusercontent.com/12828104/125810436-f25a857b-02bd-47a3-b21f-3c656ba66d04.png)



more ...
