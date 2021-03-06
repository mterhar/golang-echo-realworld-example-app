# Honeycomb take-home test

Instrumenting Conduit backend.

1. Auto-instrument Echo with the honeycomb wrapper
1. Add some general context like `user.email`
1. Add child spans for articles

If this was serious and it was worth the time: 

1. Create a [custom `gorm` logger](https://gorm.io/docs/logger.html#Customize-Logger) that sends child spans
1. Instrument comments like articles
1. Use beeline's error unpacking
1. Add `user.email` to traces via middleware rather than endpoints

# ![RealWorld Example App](logo.png)

> ### Golang/Echo codebase containing real world examples (CRUD, auth, advanced patterns, etc) that adheres to the [RealWorld](https://github.com/gothinkster/realworld) spec and API.

### [Demo](https://github.com/gothinkster/realworld)&nbsp;&nbsp;&nbsp;&nbsp;[RealWorld](https://github.com/gothinkster/realworld)

[![Build Status](https://travis-ci.org/xesina/golang-echo-realworld-example-app.svg?branch=master)](https://travis-ci.org/xesina/golang-echo-realworld-example-app)

This codebase was created to demonstrate a fully fledged fullstack application built with **Golang/Echo** including CRUD operations, authentication, routing, pagination, and more.

## Getting started

### Install Golang (go1.11+)

Please check the official golang installation guide before you start. [Official Documentation](https://golang.org/doc/install)
Also make sure you have installed a go1.11+ version.

### Environment Config

make sure your ~/.*shrc have those variable:

```bash
➜  echo $GOPATH
/Users/xesina/go
➜  echo $GOROOT
/usr/local/go/
➜  echo $PATH
...:/usr/local/go/bin:/Users/xesina/test//bin:/usr/local/go/bin
```

For more info and detailed instructions please check this guide: [Setting GOPATH](https://github.com/golang/go/wiki/SettingGOPATH)

### Clone the repository

Clone this repository:

```bash
➜ git clone https://github.com/mterhar/golang-echo-realworld-example-app.git
```

Or simply use the following command which will handle cloning the repo:

```bash
➜ go get -u -v github.com/mterhar/golang-echo-realworld-example-app
```

Switch to the repo folder

```bash
➜ cd $GOPATH/src/github.com/mterhar/golang-echo-realworld-example-app
```

### Install dependencies

```bash
➜ go mod download
```

### Run

```bash
➜ go run main.go
```

### Build

```bash
➜ go build
```

### Tests

```bash
➜ go test ./...
```
