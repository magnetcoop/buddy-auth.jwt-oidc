# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).

## [Unreleased]

## [0.6.0] - 2019-06-18

### Changed
- Fixed installation instructions in README.md

### Added
- This CHANGELOG
- Implemented JWKS keys retrieval retries with [diehard](https://github.com/sunng87/diehard)
- You can now provide a configuration key that implements the `duct.logger/Logger` protocol and the the library will log any relevant issues that may prevent tokens from being validated (e.g., inability to get the JWKS URL, getting invalid keys in the JWKS body, etc.)

## [0.5.0] - 2019-02-21

### Changed
- Added composed cache to set token storage limit. This was previously disabled (even if it was documented as working in the README), as composition with `ttlcache` didn't seem to work. 
- Bumped CIDER version dependency (devel profile only)

## [0.4.0] - 2019-01-20

### Added
- Updated Clojure version to 1.10.0
- Added deploy config

## [0.3.0] - 2019-01-28
- Initial commit (previous versions were not publicly released)

[UNRELEASED]:  https://github.com/magnetcoop/buddy-auth.jwt-oidc/compare/v0.6.0...HEAD
[0.6.0]: https://github.com/magnetcoop/buddy-auth.jwt-oidc/releases/tag/v0.6.0
[0.5.0]: https://github.com/magnetcoop/buddy-auth.jwt-oidc/releases/tag/v0.5.0
[0.4.0]: https://github.com/magnetcoop/buddy-auth.jwt-oidc/releases/tag/v0.4.0
