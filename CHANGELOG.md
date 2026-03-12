# Changelog

All notable changes to the `quantum-chemistry-bonn` LaTeX package will be
documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

## [0.2.0] - 2026-03-12

### Added

- New dependency: `acronym` package (loaded with `[nolist]` option).
- Reference shortcut macros: `\figref`, `\tabref`, `\eqeqref`, and `\siref` for
  convenient cross-referencing.
- New unit declaration `\atm` for atmosphere.
- New unit macro `\logunits` rendering "log units" via `siunitx`.
- New quantity macros: `\logkow` (octanol/water), `\logkaw` (air/water), and
  `\logkab` (α/β partition coefficients).
- New QC method: ωB97M-V (aliases `wb97mv`, `wb97m-v`).
- Over 80 predefined acronyms for common quantum-chemistry terminology via
  `\acrodef` (e.g., DFT, BSSE, CC, SCF, GGA, NMR, and many more).

### Changed

- Corrected `\dgsolv` to render as ΔsolvG (was previously using δGsolv).
- Updated `\logkow` subscript from "ow" to "o/w" for clarity.
- Updated `\logpl` spacing (thin space instead of `~`).
- Renamed `src/` directory to `tex/` following CTAN conventions for runtime
  files.

### Fixed

- Corrected date mismatch between `\ProvidesPackage`, `\date`, and the
  documentation abstract (all now consistently use the same date).

## [0.1.0] - 2025-06-04

### Added

- Initial release.
- Color definitions: `bonnblue`, `bonnred`, `bonnyellow`, `bonngrey`/`bonngray`,
  `bonngreen`, plus utility colors (`newaccent`, `black`, `highlightgreen`,
  `white`, `StdBody`).
- Shortcut color macros: `\colb`, `\coly`, `\colr`, `\colg`.
- Program name macros: `\orca`, `\censo`, `\draco`, `\crest`, `\xtb`, `\tblite`.
- Abbreviation macros: `\etal`, `\ie`, `\eg`.
- Unit macros: `\kcalpmol`, `\kjpmol` (via `siunitx`).
- Quantity macros: `\pka`, `\logkow`, `\logpl`, `\dgsolv`.
- `\method{<key>}` lookup macro with case-insensitive matching.
- `\DeclareMethod` and `\DeclareMethods` for registering QC methods with
  aliases.
- Predeclared methods: r²SCAN-3c, ωr²SCAN-D4, ωPr²SCAN50-D4.
- Full documentation and example file.

[unreleased]: https://github.com/chselz/quantum-chemistry-bonn/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/chselz/quantum-chemistry-bonn/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/chselz/quantum-chemistry-bonn/releases/tag/v0.1.0
