---
title: Async Starter Project
description: Starter project based on oatpp asynchronous API.
sidebarDepth: 0
---

# Async API - Starter Project <seo/>

Async-API web service starter project.

::: tip
[Github Repo](https://github.com/oatpp/oatpp-starter-async)
:::

## Overview

### Project layout

```

- CMakeLists.txt          // project loader script. load and build dependencies
- main/                   // main project directory
    |
    |- CMakeLists.txt     // projects CMakeLists.txt
    |- src/               // source folder
    |- test/              // test folder

```
```
- src/
    |
    |- controller/              // Folder containing UserController where all endpoints are declared
    |- dto/                     // DTOs are declared here
    |- AppComponent.hpp         // Service config
    |- Logger.hpp               // Application Logger
    |- App.cpp                  // main() is here

```

## Build and Run

### Using CMake

```
$ mkdir build && cd build
$ cmake ..
$ make run        ## Download, build, and install all dependencies. Run project

```

### In Docker

```
$ docker build -t oatpp-starter-async .
$ docker run -p 8000:8000 -t oatpp-starter-async
```
