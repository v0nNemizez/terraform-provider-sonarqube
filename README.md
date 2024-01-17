# terraform-provider-sonarqube

Terraform provider for managing Sonarqube configuration
This is a community provider and is not supported by Hashicorp.

## Installation
This provider is a fork of the terraform provider and has been published to the OpenTofu Registry.
See [index.md](docs/index.md) for setup and configuration options

## Developing the Provider

Working on this provider requires the following:

* [Terraform](https://www.terraform.io/downloads.html)
* [Go](http://www.golang.org)
* [Docker Engine](https://docs.docker.com/engine/install/)

You will also need to correctly setup a [GOPATH](http://golang.org/doc/code.html#GOPATH), as well as adding `${GOPATH}/bin` to your `$PATH`.

To compile the provider, run `make`. This will install the provider into your GOPATH.

In order to run the full suite of Acceptance tests, run `make -i testacc`. These tests require Docker to be installed on the machine that runs them, and do not create any remote resources.

```sh
$ make -i testacc
```

## Debugging the Provider

See [debugging.md](docs/debugging.md)
