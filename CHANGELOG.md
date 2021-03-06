# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project mostly adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.1.0] - 2020-05-09

### Added
- Added `line-[style]` and `line-[color]` utilities to go with Tailwind’s text decoration utilities (`underline` and `line-through`); they can be customized with the `textDecorationStyle` and `textDecorationColor` theme keys

### Fixed
- Fixed an issue when using a font size that includes a default line height in a text style (e.g. `['16px', '24px']`), which is supported since Tailwind 1.3

## [3.0.1] - 2020-02-13

### Fixed
- Negative text indent utilities now have the expected class name (`-indent-*` instead of `indent--*`)

## [3.0.0] - 2020-02-05

### Added
- Added kerning utilities, which can be disabled by setting the `kerning` option to `false` (thanks, [@mapgrid](https://github.com/mapgrid)!)
- Added text rendering utilities, which can be customized with the `textRendering` theme object (thanks, [@mapgrid](https://github.com/mapgrid)!)

### Changed
- Changed to use Tailwind 1.2’s new plugin definition syntax
- Font variant utilities (caps, nums, and ligatures) are now generated from the `fontVariantCaps`, `fontVariantNumeric`, and `fontVariantLigatures` theme keys, and their names have changed to include a `caps-`, `nums-`, or `ligatures-` prefix (so `normal-caps` is now `caps-normal`, `no-ligatures` is now `ligatures-none`, etc.)
- The `caps`, `nums`, and `ligatures` variants keys have changed to `fontVariantCaps`, `fontVariantNumeric`, and `fontVariantLigatures`

### Removed
- Removed the `caps`, `nums`, and `ligatures` options

## [2.2.0] - 2019-09-02

### Added
- Added utilities for some OpenType features: caps (alternate glyphs for capital letters), nums (alternate glyphs for numbers, fractions, and ordinal markers), and ligatures
- Added a `no-ellipsis` utility to undo `ellipsis` at breakpoints

## [2.1.1] - 2019-05-27

### Fixed
- Fixed an issue when using an array for a font family in a text style

## [2.1.0] - 2019-05-26

### Added
- Added text style components (see the `textStyles` theme object in the `README` for more info)

## [2.0.0] - 2019-05-13

### Changed since 2.0.0-beta.2
- Added support for global variants thanks to Tailwind’s `variants()` helper function

### Added since 1.x
- Tailwind 1.0.0 compatibility
- Added text unset utilities
- Added boolean options to enable/disable the non-configurable utilities (`ellipsis`, `hyphens`, and `textUnset`)

### Changed since 1.x
- Most of the config options have been moved to the `theme` and `variants` objects in your Tailwind config (see `README` for more info)
- Responsive variants are now generated by default

## [2.0.0-beta.2] - 2019-04-04

### Added
- Added text unset utilities
- Added boolean options to enable/disable the non-configurable utilities (`ellipsis`, `hyphens`, and `textUnset`)

## [2.0.0-beta.1] - 2019-04-04

### Added
- Tailwind 1.0.0 compatibility

### Changed
- Most of the config options have been moved to the `theme` and `variants` objects in your Tailwind config (see `README` for more info)
- Responsive variants are now generated by default

## [1.1.0] - 2019-03-22

### Added
- Added the `hyphens-none` and `hyphens-manual` utilities

### Changed
- Changed the `hyphens` utility to `hyphens-auto`

## [1.0.2] - 2018-11-04

### Added
- Added proper tests with Jest

## [1.0.1] - 2018-08-14

### Fixed
- Fixed escaping in selectors generated by the plugin

## [1.0.0] - 2018-05-06

Initial release

[Unreleased]: https://github.com/benface/tailwindcss-typography/compare/v3.1.0...HEAD
[3.1.0]: https://github.com/benface/tailwindcss-typography/compare/v3.0.1...v3.1.0
[3.0.1]: https://github.com/benface/tailwindcss-typography/compare/v3.0.0...v3.0.1
[3.0.0]: https://github.com/benface/tailwindcss-typography/compare/v2.2.0...v3.0.0
[2.2.0]: https://github.com/benface/tailwindcss-typography/compare/v2.1.1...v2.2.0
[2.1.1]: https://github.com/benface/tailwindcss-typography/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/benface/tailwindcss-typography/compare/v2.0.0...v2.1.0
[2.0.0]: https://github.com/benface/tailwindcss-typography/compare/v2.0.0-beta.2...v2.0.0
[2.0.0-beta.2]: https://github.com/benface/tailwindcss-typography/compare/v2.0.0-beta.1...v2.0.0-beta.2
[2.0.0-beta.1]: https://github.com/benface/tailwindcss-typography/compare/v1.1.0...v2.0.0-beta.1
[1.1.0]: https://github.com/benface/tailwindcss-typography/compare/v1.0.2...v1.1.0
[1.0.2]: https://github.com/benface/tailwindcss-typography/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/benface/tailwindcss-typography/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/benface/tailwindcss-typography/releases/tag/v1.0.0
