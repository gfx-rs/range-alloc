# Changelog

All notable changes to this project will be documented in this file.

The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to cargo's version of [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Per Keep a Changelog there are 6 main categories of changes:
- Added
- Changed
- Deprecated
- Removed
- Fixed
- Security

#### Table of Contents

- [Unreleased](#unreleased)
- [v0.1.5](#v015)
- [v0.1.4](#v014)
- [v0.1.3](#v013)

## Unreleased

- Changed: Switched to `#![no_std]` with `alloc` dependency. @waywardmonkeys
- Changed: Updated MSRV from 1.36 to 1.39 to enable `no_std`.

## v0.1.5

- Added: `allocate_range_aligned` method for aligned sub-range allocation without wasting padding space.
- Added: Documentation comments for all public items.
- Added: README with usage examples, MSRV policy, and license info.
- Added: CI workflow with format, clippy, test, and MSRV jobs.
- Internal: Updated edition from 2015 to 2018.

## v0.1.4

- Fixed: `grow_to` incorrectly assumed the last free range was always at the end of the pool, corrupting the free list when the tail was allocated and an earlier range was free. @dbartussek
- Internal: Clippy lint fixes.

## v0.1.3

Initial release on separate repository (previously part of [gfx-rs](https://github.com/gfx-rs/gfx)).

## Diffs

- [Unreleased](https://github.com/gfx-rs/range-alloc/compare/v0.1.5...HEAD)
- [v0.1.5](https://github.com/gfx-rs/range-alloc/compare/v0.1.4...v0.1.5)
- [v0.1.4](https://github.com/gfx-rs/range-alloc/compare/v0.1.3...v0.1.4)
