# init.yaktor.io

> NOTE: Please report issues at https://github.com/SciSpike/yaktor-issues/issues.

This repo contains the source content for http://init.yaktor.io, which is intended to provide an easy way for folks to initialize a new Yaktor application with `curl` (or `wget`), piping the output to `sh`.

## Technologies Supported
Currently, this repo only supports our Node.js mapping.

### Node.js
Since Node.js is our first fully-supported technology mapping, you can issue command
```
curl init.yaktor.io | sh
```
You could also issue command
```
curl init.yaktor.io/node | sh
```
to get the same result.

## For Maintainers of This Site
The idea here is that any script will be named for the technology mapping supported.
For example, the technology mapping for Node.js is called `node`, so the init script is placed in a file at the root called `node`.
Any future technology mappings should be named accordingly and placed in this repo's root directory.

> NOTE: Please never change this site to use redirects.
That would complicate the use of `curl` & `wget`, requiring additional flags.
The whole purpose of this site is to make it as brain-dead easy to remember and to execute.
Redirects would complicate the invocation & be more to remember.
