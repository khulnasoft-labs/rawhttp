# rawhttp

[![License](https://img.shields.io/github/license/khulnasoft-lab/rawhttp)](LICENSE.md)
![Go version](https://img.shields.io/github/go-mod/go-version/khulnasoft-lab/rawhttp?filename=go.mod)
[![Release](https://img.shields.io/github/release/khulnasoft-lab/rawhttp)](https://github.com/khulnasoft-lab/rawhttp/releases/)
[![Checks](https://github.com/khulnasoft-lab/rawhttp/actions/workflows/build_test.yaml/badge.svg)](https://github.com/khulnasoft-lab/rawhttp/actions/workflows/build_test.yaml)
[![GoDoc](https://img.shields.io/badge/go-reference-blue)](https://pkg.go.dev/github.com/khulnasoft-lab/rawhttp)

rawhttp is a Go package for making HTTP requests in a raw way.


- Forked and adapted from [https://github.com/gorilla/http](https://github.com/gorilla/http) and [https://github.com/valyala/fasthttp](https://github.com/valyala/fasthttp)
- The original idea is inspired by [@tomnomnom/rawhttp](https://github.com/tomnomnom/rawhttp) work


# Library Usage

A simple example to get started with rawhttp is available at [examples](./example/simple/main.go). For documentation, please refer [godoc](https://pkg.go.dev/github.com/khulnasoft-lab/rawhttp)

## Note

rawhttp internally uses [fastdialer](https://github.com/khulnasoft-lab/fastdialer) to dial connections and fastdialer has a disk cache for DNS lookups. While using rawhttp `.Close()` method should be called at end of the program to remove temporary files created by fastdialer.

# License

rawhttp is distributed under MIT License