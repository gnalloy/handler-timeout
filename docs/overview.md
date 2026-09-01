# Overview

[简体中文](overview.zh-CN.md) | [Docs Index](README.md)

## Purpose

Timeout and idle-state handlers for Gnalloy channels, backed by the core hashed wheel timer.

This module provides Pipeline handlers. A handler observes, transforms, rejects, delays, records, or protects messages after a Channel already exists. It does not own listening sockets or application protocols unless explicitly named.

## Repository Identity

- Module path: `gnalloy.org/handler-timeout`
- GitHub repository: `github.com/gnalloy/handler-timeout`
- Default branch: `dev`
- License: Apache-2.0

## Package Map
- `gnalloy.org/handler-timeout` (`timeout`)

## Direct Gnalloy Dependencies

- `gnalloy.org/gnalloy`

## Direct Dependents in the Current Repository Set

- `gnalloy.org/codec-websocket`

## Architecture Position

Gnalloy keeps the core small and dependency-light. This repository is a replaceable module around one responsibility, connected through explicit Go packages instead of runtime discovery.

## Compatibility

The public import path is `gnalloy.org/handler-timeout`. Until the first stable tag is published, use `@dev` or an explicit pseudo-version selected by your dependency policy.
