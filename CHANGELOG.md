# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- The default copyright note can be overwritten by redefining the command `\copyrightnote`.

### Changed

- If available, use pdfmanagement instead of `\pdfpagesattr` [[#12](https://github.com/adbrucker/llncsconf/issues/12)]
- If `intended` is used, the note is put on each page [[#16](https://github.com/adbrucker/llncsconf/issues/16)]

### Fixed

- Reduzed size of author statement in footnote [[#15](https://github.com/adbrucker/llncsconf/issues/15)]

## [1.1.0] - 2020-05-10

### Added

- Crop area now takes paper format (a4, letter) into account

## 1.0.0 - 2018-02-20

### Added

- Initial version uploaded to CTAN.

[Unreleased]: https://git.logicalhacking.com/adbrucker/llncsconf/compare/v1.1.0...HEAD
[1.1.0]: https://git.logicalhacking.com/adbrucker/llncsconf/compare/v1.0.0...v1.1.0
