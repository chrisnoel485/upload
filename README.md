# Broken Environment

`Broken Environment` is a test environment where you need to fix the environment so it is run as needed.

> Do read all the scripts given to you before executing any (:

## Dependencies

- docker
- shell (bash)
- make
- jq

## Goals

- `broken-env:demo` docker image is created successfully by using `make build`
- `broken-env:demo` docker image endpoint is accessible from host machine by using `make run` and `curl -s localhost:8228/` from host machine
- `broken-env:demo` docker image endpoint is returning a JSON similar to this `{"built_at":"date"}` where `date` is the datetime the image is built generated by the `pre.sh` with predefined format
- `broken-env:demo` docker image and running container can be removed by using `make cleanup`

## Scope

You can change basically every files inside this directory except `test.sh` to help you make sure the goals are accomplished. **Make a write up about your solution below will be a plus point (:**

## Test

For easier testing, you can execute `make test` to run all commands programatically.
`make test` is only a helper command, not a judge.

## Solution

After all the goals are accomplished, before send back to us, you need to compress your solution into `zip/tar` which consists of these files:

- Dockerfile
- Makefile
- post.sh
- pre.sh
- README.md
- test.sh

## Write Up

> Append this documentation on how you fix all the script