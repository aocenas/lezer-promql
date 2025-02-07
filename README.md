# lezer-promql

[![CircleCI](https://circleci.com/gh/prometheus/lezer-promql.svg?style=shield)](https://circleci.com/gh/prometheus/lezer-promql) [![NPM version](https://img.shields.io/npm/v/lezer-promql.svg)](https://www.npmjs.org/package/lezer-promql)

## Where does it come from?

The authoritative copy of this code lives in `prometheus/prometheus` and is synced to
`prometheus/lezer-promql` on a regular basis by a bot. Please contribute any code changes to the code
in https://github.com/prometheus/prometheus/tree/main/web/ui/module/codemirror-promql/src/grammar.

## Overview

This is a PromQL grammar for the [lezer](https://lezer.codemirror.net/) parser system. It is inspired by the initial
grammar coming from [Prometheus](https://github.com/prometheus/prometheus/blob/master/promql/parser/generated_parser.y)
written in yacc.

This library is stable but doesn't provide any guideline of how to use it as it has been integrated
into [codemirror-promql](https://github.com/prometheus/codemirror-promql). If you want to use this library,
you perhaps want to actually use **codemirror-promql** instead.

**Note**: This library is following the changes of the upstream grammar (i.e. coming from Prometheus) as closed as possible

## Installation

This package is available as an npm package:

```bash
npm install --save lezer-promql
```

**Note**: you will have to manually install the dependency `lezer` as it is a peer dependency to this package.

```bash
npm install --save lezer
```

## Development

### Building

    npm i
    npm run build

### Testing

    npm run test

## License

The code is licensed under an [Apache 2.0](./LICENSE) license.
