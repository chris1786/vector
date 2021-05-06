---
title: Internal logs
description: Expose all log and trace messages emitted by the running Vector instance
kind: source
---

## Requirements

{{< component/requirements >}}

## Configuration

{{< component/config >}}

## Output

{{< component/output >}}

## Telemetry

{{< component/telemetry >}}

## How it works

### Context

{{< snippet "context" >}}

### Logs are limited by startup options

At startup, the selection of log messages generated by Vector is set by a combination of the `LOG` environment variable and the `--quiet` and `--verbose` command-line
options. The `internal_logs` source only receives logs that are generated by these options.

### State

{{< snippet "stateless" >}}