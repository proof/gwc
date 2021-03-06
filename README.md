# GWC (Go Web Client)
[![Go Report Card](https://goreportcard.com/badge/github.com/delicb/gwc)](https://goreportcard.com/report/github.com/delicb/gwc)
[![Build Status](https://travis-ci.org/delicb/gwc.svg?branch=master)](https://travis-ci.org/delicb/gwc)
[![codecov](https://codecov.io/gh/delicb/gwc/branch/master/graph/badge.svg)](https://codecov.io/gh/delicb/gwc)
![status](https://img.shields.io/badge/status-beta-red.svg)
[![GoDoc](https://img.shields.io/badge/godoc-reference-blue.svg)](http://godoc.org/github.com/delicb/gwc)



GWC is GoLang HTTP client based on [Cliware](https://github.com/delicb/cliware)
client middleware management library and its [middlewares](https://github.com/delicb/cliware-middlewares).

Basic idea is to use same middleware mechanism on client side as many projects
use it for server development. 

Because it is based on middlewares client is very pluggable. However, even out 
of box it should support most common use cases.

# Install
Run `go get go.delic.rs/gwc` in terminal.


# State
This is early development, not stable, backward compatibility not guarantied.
**Not recommended for use in production yet**.

# Credits
Idea and bunch of implementation details were taken from cool GoLang HTTP client
[Gentleman](https://github.com/h2non/gentleman).

Difference is that GWC is based on Cliware, which supports `context` for client
requests and has more simple idea of middleware. Also, GWC is lacking some
features that Gentleman has (like mux). For now I do not plan on adding them
to GWC, but I might write middleware that support similar functionality in the
future. 
