# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Fixed
- Issue #1 - nestjs support

### Added
- added new package scripts `test` and `test:coverage`
- [Volta](https://volta.sh/) to pin packages

### Changes
- coveralls and istanbul pinned at latest versions
- oauth moved to peer dependecies 
- package name, links, README updates
- verify callback: first argument is now an object to pick properties (fixes )

### Removed
- Removed support for versions of node under 18, although 16 should still work.
- Makefiles
- Travis 

## [1.6.1] - 2021-09-24
### Fixed
- Error in cases where the authorization server returns a successful access
token response which is missing an `access_token` parameter.

## [1.6.0] - 2021-07-01
### Added

- Support for `store: true` option to `Strategy` constructor, which initializes
a state store capable of storing application-level state.
- Support for `state` object passed as option to `authenticate`, which will be
persisted in the session by state store.
- `callbackURL` property added to metadata passed to state store.
