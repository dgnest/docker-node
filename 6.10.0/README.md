# dgnest/node:6.10.0

[![Build Status](https://travis-ci.org/dgnest/docker-node.svg)](https://travis-ci.org/dgnest/docker-node)
[![GitHub issues](https://img.shields.io/github/issues/dgnest/docker-node.svg)](https://github.com/dgnest/docker-node/issues)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)](LICENSE)

Requirements
------------

None

## Dependencies

none

## Usage

In order to run a basic container start a container as follows:

`docker run -P --name nodejs -e ENV=DEV dgnest/node:6.10.0`

## Environment Variables

This is a list of the available environment variables which can be set at runtime using -e KEY=value.
For example, to change the default environment you can issue
`docker run -P --name nodejs -e ENV=dev dgnest/node:6.10.0`
