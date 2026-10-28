# Changelog

## [v1.1.2] - 2026-10-28

### Changed

* ShellSpec will now use `$RUNNER_TEMP` for its temporary directory

## [v1.1.1] - 2026-10-28

### Fixed

* Failure when called with `shell: zsh` and `kcov: true`

## [v1.1.0] - 2026-10-27

### Added

* `shellspec-shell` option to select the shell used to run ShellSpec

### Changed

* `project-root` default value is now `.` instead of the empty string

## [v1.0.1] - 2026-10-27

### Fixed

* Exit code 100 on ubuntu-24.04
* Report and coverage output not uploaded as artifacts on Windows
  runners

## v1.0.0 - 2026-10-18

* Initial release

[v1.1.2]: https://github.com/jefferyto/shellspec-action/compare/v1.1.1...v1.1.2
[v1.1.1]: https://github.com/jefferyto/shellspec-action/compare/v1.1.0...v1.1.1
[v1.1.0]: https://github.com/jefferyto/shellspec-action/compare/v1.0.1...v1.1.0
[v1.0.1]: https://github.com/jefferyto/shellspec-action/compare/v1.0.0...v1.0.1
