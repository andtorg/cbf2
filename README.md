CBF 2
====

This is an helper file to build a pentaho system (server + solution). It's largely derived from [CBF](https://github.com/webdetails/cbf) tool already available to Pentaho community.

It features an easier logic to build server (a fewer number of alternative, indeed) and embeds the major plugins setup, via property setting.

The main goal is to let Ant do all the job with no need for other script geekery, being bash or whatever. One script, one language to look for bugs.


To build the server, invoke
`ant -Dproject=yourProject -Denv=yourEnv`

The default `all` target will build from source and apply the patches.

To install all plugins, invoke the `install-plugins` target. It will download and install the components.
