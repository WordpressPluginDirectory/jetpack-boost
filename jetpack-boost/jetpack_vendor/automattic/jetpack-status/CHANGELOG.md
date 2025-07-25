# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [6.0.0] - 2025-07-21
### Removed
- Remove host guess based on DNS. [#44325]

## [5.4.0] - 2025-07-08
### Changed
- VIP: Change hosting check method back now that constant is reliable. [#44223]

## [5.3.1] - 2025-06-27
### Changed
- Internal updates.

## [5.3.0] - 2025-06-23
### Changed
- VIP: Change hosting check method. [#44059]

## [5.2.1] - 2025-06-19
### Changed
- Internal updates.

## [5.2.0] - 2025-06-10
### Added
- Request: Add new class used to classify requests on a site. [#43843]

## [5.1.4] - 2025-04-28
### Changed
- Internal updates.

## [5.1.3] - 2025-04-21
### Fixed
- Module Activation: Use require_once to avoid potential redeclaration errors. [#43120]

## [5.1.2] - 2025-04-14
### Changed
- Internal updates.

## [5.1.1] - 2025-03-31
### Changed
- Internal updates.

## [5.1.0] - 2025-03-26
### Added
- Add database option to enable Offline Mode. [#42630]

## [5.0.10] - 2025-03-21
### Changed
- Internal updates.

## [5.0.9] - 2025-03-18
### Changed
- Internal updates.

## [5.0.8] - 2025-03-17
### Changed
- Internal updates.

## [5.0.7] - 2025-03-12
### Changed
- Internal updates.

## [5.0.6] - 2025-03-05
### Changed
- Internal updates.

## [5.0.5] - 2025-03-03
### Fixed
- Hosting provider checks: Avoid PHP warnings in local environments. [#41994]

## [5.0.4] - 2025-02-24
### Changed
- Host detection: Look for specific external hosting provider only when required. [#41890]

## [5.0.3] - 2025-02-03
### Fixed
- Code: Remove extra params on function calls. [#41263]

## [5.0.2] - 2025-01-20
### Changed
- Code: Use function-style exit() and die() with a default status code of 0. [#41167]

## [5.0.1] - 2024-11-25
### Changed
- Updated package dependencies. [#40258]

## [5.0.0] - 2024-11-14
### Removed
- General: Update minimum PHP version to 7.2. [#40147]

## [4.0.3] - 2024-11-04
### Added
- Enable test coverage. [#39961]

## [4.0.2] - 2024-09-23
### Changed
- Update dependencies.

## [4.0.1] - 2024-09-06
### Removed
- Removed usage of _deprecated_function when deprecating Status::is_onboarding [#39272]

## [4.0.0] - 2024-09-05
### Deprecated
- Deprecated Jetpack Onboarding system. [#39229]

## [3.3.4] - 2024-08-23
### Changed
- Updated package dependencies. [#39004]

## [3.3.3] - 2024-08-19
### Changed
- Internal updates.

## [3.3.2] - 2024-06-24
### Changed
- Internal updates.

## [3.3.1] - 2024-06-21
### Added
- Check for active modules among the unavailable ones. [#37358]

## [3.3.0] - 2024-06-10
### Deprecated
- Deprecated is_staging_site [#37023]

## [3.2.3] - 2024-06-03
### Removed
- Remove the Identity Crisis dev dependency. [#37654]

## [3.2.2] - 2024-05-29
### Changed
- Phab baseline file update. [#36968]

## [3.2.1] - 2024-05-28
### Changed
- Internal updates.

## [3.2.0] - 2024-05-22
### Deprecated
- Jetpack: Deprecated Errors class. [#37451]

## [3.1.0] - 2024-05-20
### Added
- Add the 'is_current_request_activating_plugin_from_plugins_screen' method extracted from the Plugin Install package. [#37430]

## [3.0.3] - 2024-05-08
### Fixed
- Status: Added check for compatibility reasons [#37256]

## [3.0.2] - 2024-05-06
### Added
- Add new method used to track allowed domains for API access. [#36924]

## [3.0.1] - 2024-04-30
### Changed
- Internal updates.

## [3.0.0] - 2024-04-25
### Added
- Add is_automattician_feature_flags_only on Jetpack sites as an alternative to is_automattician present on simple sites. [#34798]

### Removed
- Remove methods deprecated long ago. [#36985]

## [2.2.2] - 2024-04-22
### Changed
- Internal updates.

## [2.2.1] - 2024-04-08
### Changed
- Internal updates.

## [2.2.0] - 2024-03-22
### Added
- Add support for A8C for Agencies source parameter. [#36491]

## [2.1.3] - 2024-03-20
### Changed
- Internal updates.

## [2.1.2] - 2024-03-12
### Changed
- Internal updates.

## [2.1.1] - 2024-03-01
### Fixed
- Avoid issues when the dns_get_record function is not defined [#36019]

## [2.1.0] - 2024-01-18
### Added
- Add hosting provider check. [#34864]

## [2.0.2] - 2023-12-03
### Fixed
- Module active checks should always be true on WordPress.com simple sites. [#34248]

## [2.0.1] - 2023-11-21
### Changed
- Added a note of non-usage of PHP8+ functions yet. [#34137]
- Replaced usage of substr() with str_starts_with() and str_ends_with(). [#34207]

## [2.0.0] - 2023-11-20
### Changed
- Updated required PHP version to >= 7.0. [#34192]

## [1.19.0] - 2023-11-13
### Added
- Added Host::get_source_query() to return the 'source' query param from the current URL. [#33984]

## [1.18.5] - 2023-09-25
### Changed
- Add 127.0.0.1 into the list of known local domains. [#32898]
- WP.com Compatibility: Abort out early checking if Protect is active. WP.com's protection is not site option based. [#33196]

## [1.18.4] - 2023-09-19

- Minor internal updates.

## [1.18.3] - 2023-09-11
### Changed
- General: remove backwards-compatibility function checks now that the package supports WP 6.2. [#32772]

## [1.18.2] - 2023-09-04
### Fixed
- Exclude domains starting with live from known Pantheon staging domains [#32789]

## [1.18.1] - 2023-08-23
### Changed
- Updated package dependencies. [#32605]

## [1.18.0] - 2023-07-18
### Added
- Transferred 'get_calypso_env()' method from Jetpack plugin. [#31906]

## [1.17.2] - 2023-06-19
### Changed
- Use Plans package to detect feature support. [#31213]

## [1.17.1] - 2023-05-11
### Changed
- PHP 8.1 compatibility updates [#30517]

## [1.17.0] - 2023-04-17
### Changed
- When Jetpack is available, `Modules::get()` no longer translates `module_tags`. Use Jetpack's `jetpack_get_module_i18n_tag()` function if you need translations. [#30067]

## [1.16.4] - 2023-04-10
### Added
- Add Jetpack Autoloader package suggestion. [#29988]

## [1.16.3] - 2023-03-28
### Changed
- Move brute force protection into WAF package. [#28401]

## [1.16.2] - 2023-02-20
### Changed
- Minor internal updates.

## [1.16.1] - 2023-01-23
### Added
- Add new filters for the latest status methods [#28328]

## [1.16.0] - 2023-01-16
### Added
- Add 2 new methods to detect whether a site is private or not. [#28322]

## [1.15.4] - 2023-01-11
### Changed
- Modules: Allow for deactivating multiple plugins when activating a module. [#28181]

## [1.15.3] - 2022-12-19
### Changed
- Updated package dependencies.

## [1.15.2] - 2022-12-02
### Changed
- Updated package dependencies. [#27688]

## [1.15.1] - 2022-11-22
### Changed
- Updated package dependencies. [#27043]

## [1.15.0] - 2022-11-07
### Added
- WordPress.com: add checks for Simple or either Simple/WoA. [#27278]

## [1.14.3] - 2022-07-26
### Changed
- Updated package dependencies. [#25158]

## [1.14.2] - 2022-07-19
### Changed
- Update logic in `is_woa_site` function for host changes [#25067]

## [1.14.1] - 2022-06-21
### Changed
- Renaming master to trunk.

## [1.14.0] - 2022-06-14
### Fixed
- Moved the connection_url_redirect action handling to the connection package. [#24529]

## [1.13.6] - 2022-05-24
### Added
- Allow plugins to filter the list of available modules. Only activate and consider active modules that are available [#24454]

## [1.13.5] - 2022-05-20
### Changed
- Modules: Make activate() method Jetpack plugin agnostic. Allowing standalone plugins to use it without Jetpack.

## [1.13.4] - 2022-05-19
### Added
- PHPCS updates. [#24418]

## [1.13.3] - 2022-05-10

## [1.13.2] - 2022-04-26
### Changed
- Updated package dependencies.

## [1.13.1] - 2022-04-19
### Changed
- PHPCS: Fix `WordPress.Security.ValidatedSanitizedInput`

## [1.13.0] - 2022-04-05
### Added
- Created Modules and File modules for managing those resources

## [1.12.0] - 2022-03-02
### Added
- Cache return values (per blog) from various status methods.

## [1.11.2] - 2022-02-28
### Fixed
- Re-doing 1.11.1 to fixup a bad release.

## [1.11.1] - 2022-02-28
### Fixed
- Remove trailing semicolor form site suffix.

## [1.11.0] - 2022-02-22
### Added
- Add methods to distinguish Newspack and VIP sites.

## [1.10.0] - 2022-01-25
### Added
- Added Visitor class for status regarding the site visitor.

## [1.9.5] - 2022-01-04
### Changed
- Switch to pcov for code coverage.
- Updated package dependencies

## [1.9.4] - 2021-12-14
### Changed
- Updated package dependencies.

## [1.9.3] - 2021-11-22
### Changed
- Updated package dependencies

## [1.9.2] - 2021-11-16
### Changed
- Add a function_exists check before calling wp_get_environment_type

## [1.9.1] - 2021-11-02
### Changed
- Set `convertDeprecationsToExceptions` true in PHPUnit config.
- Update PHPUnit configs to include just what needs coverage rather than include everything then try to exclude stuff that doesn't.

## [1.9.0] - 2021-10-26
### Added
- Added Host class for reporting known hosting environment information.

## [1.8.4] - 2021-10-13
### Changed
- Updated package dependencies.

## [1.8.3] - 2021-10-12
### Changed
- Updated package dependencies

## [1.8.2] - 2021-09-28
### Changed
- Updated package dependencies.

## [1.8.1] - 2021-08-30
### Changed
- Run composer update on test-php command instead of phpunit
- Tests: update PHPUnit polyfills dependency (yoast/phpunit-polyfills).
- update annotations versions

## [1.8.0] - 2021-06-15
### Changed
- Update callback to Jetpack to new Identity_Crisis class.

## [1.7.6] - 2021-05-25
### Changed
- Updated package dependencies.

## [1.7.5] - 2021-04-27
### Deprecated
- Deprecates is_no_user_testing_mode

## [1.7.4] - 2021-04-08
### Changed
- Packaging and build changes, no change to the package itself.

## [1.7.3] - 2021-03-30
### Added
- Composer alias for dev-master, to improve dependencies

### Changed
- Update package dependencies.

### Fixed
- Use `composer update` rather than `install` in scripts, as composer.lock isn't checked in.

## [1.7.2] - 2021-02-05

- CI: Make tests more generic

## [1.7.1] - 2021-01-20

- Add mirror-repo information to all current composer packages
- Monorepo: Reorganize all projects

## [1.7.0] - 2020-12-14

- Update dependency brain/monkey to v2.6.0
- Pin dependencies
- Packages: Update for PHP 8 testing

## [1.6.0] - 2020-11-23

- Status: Introduce get_site_suffix method
- Status: Fix test failure
- Status: Improve the staging site detection
- General: update minimum required version to WordPress 5.5
- Add the no_user_testing mode
- Status: Add a couple of test cases for staging site detection
- Update dependency brain/monkey to v2.5.0
- Updated PHPCS: Packages and Debugger

## [1.5.0] - 2020-10-13

- Also use Core `wp_get_environment_type` for local

## [1.4.0] - 2020-08-13

- CI: Try collect js coverage

## [1.3.0] - 2020-07-28

- Core Compat: Site Environment

## [1.2.0] - 2020-06-22

- PHPCS: Clean up the packages
- Staging Sites: add newspack staging to the list of known providers

## [1.1.1] - 2020-01-27

- Pin dependency brain/monkey to 2.4.0

## [1.1.0] - 2020-01-14

- Packages: Various improvements for wp.com or self-contained consumers

## [1.0.4] - 2019-11-08

- Packages: Use classmap instead of PSR-4

## [1.0.3] - 2019-10-28

- Packages: Add gitattributes files to all packages that need th…

## [1.0.2] - 2019-10-23

- Use spread operator instead of func_get_args

## [1.0.1] - 2019-09-20

- Docs: Unify usage of @package phpdoc tags

## 1.0.0 - 2019-09-14

- Packages: Introduce a status package

[6.0.0]: https://github.com/Automattic/jetpack-status/compare/v5.4.0...v6.0.0
[5.4.0]: https://github.com/Automattic/jetpack-status/compare/v5.3.1...v5.4.0
[5.3.1]: https://github.com/Automattic/jetpack-status/compare/v5.3.0...v5.3.1
[5.3.0]: https://github.com/Automattic/jetpack-status/compare/v5.2.1...v5.3.0
[5.2.1]: https://github.com/Automattic/jetpack-status/compare/v5.2.0...v5.2.1
[5.2.0]: https://github.com/Automattic/jetpack-status/compare/v5.1.4...v5.2.0
[5.1.4]: https://github.com/Automattic/jetpack-status/compare/v5.1.3...v5.1.4
[5.1.3]: https://github.com/Automattic/jetpack-status/compare/v5.1.2...v5.1.3
[5.1.2]: https://github.com/Automattic/jetpack-status/compare/v5.1.1...v5.1.2
[5.1.1]: https://github.com/Automattic/jetpack-status/compare/v5.1.0...v5.1.1
[5.1.0]: https://github.com/Automattic/jetpack-status/compare/v5.0.10...v5.1.0
[5.0.10]: https://github.com/Automattic/jetpack-status/compare/v5.0.9...v5.0.10
[5.0.9]: https://github.com/Automattic/jetpack-status/compare/v5.0.8...v5.0.9
[5.0.8]: https://github.com/Automattic/jetpack-status/compare/v5.0.7...v5.0.8
[5.0.7]: https://github.com/Automattic/jetpack-status/compare/v5.0.6...v5.0.7
[5.0.6]: https://github.com/Automattic/jetpack-status/compare/v5.0.5...v5.0.6
[5.0.5]: https://github.com/Automattic/jetpack-status/compare/v5.0.4...v5.0.5
[5.0.4]: https://github.com/Automattic/jetpack-status/compare/v5.0.3...v5.0.4
[5.0.3]: https://github.com/Automattic/jetpack-status/compare/v5.0.2...v5.0.3
[5.0.2]: https://github.com/Automattic/jetpack-status/compare/v5.0.1...v5.0.2
[5.0.1]: https://github.com/Automattic/jetpack-status/compare/v5.0.0...v5.0.1
[5.0.0]: https://github.com/Automattic/jetpack-status/compare/v4.0.3...v5.0.0
[4.0.3]: https://github.com/Automattic/jetpack-status/compare/v4.0.2...v4.0.3
[4.0.2]: https://github.com/Automattic/jetpack-status/compare/v4.0.1...v4.0.2
[4.0.1]: https://github.com/Automattic/jetpack-status/compare/v4.0.0...v4.0.1
[4.0.0]: https://github.com/Automattic/jetpack-status/compare/v3.3.4...v4.0.0
[3.3.4]: https://github.com/Automattic/jetpack-status/compare/v3.3.3...v3.3.4
[3.3.3]: https://github.com/Automattic/jetpack-status/compare/v3.3.2...v3.3.3
[3.3.2]: https://github.com/Automattic/jetpack-status/compare/v3.3.1...v3.3.2
[3.3.1]: https://github.com/Automattic/jetpack-status/compare/v3.3.0...v3.3.1
[3.3.0]: https://github.com/Automattic/jetpack-status/compare/v3.2.3...v3.3.0
[3.2.3]: https://github.com/Automattic/jetpack-status/compare/v3.2.2...v3.2.3
[3.2.2]: https://github.com/Automattic/jetpack-status/compare/v3.2.1...v3.2.2
[3.2.1]: https://github.com/Automattic/jetpack-status/compare/v3.2.0...v3.2.1
[3.2.0]: https://github.com/Automattic/jetpack-status/compare/v3.1.0...v3.2.0
[3.1.0]: https://github.com/Automattic/jetpack-status/compare/v3.0.3...v3.1.0
[3.0.3]: https://github.com/Automattic/jetpack-status/compare/v3.0.2...v3.0.3
[3.0.2]: https://github.com/Automattic/jetpack-status/compare/v3.0.1...v3.0.2
[3.0.1]: https://github.com/Automattic/jetpack-status/compare/v3.0.0...v3.0.1
[3.0.0]: https://github.com/Automattic/jetpack-status/compare/v2.2.2...v3.0.0
[2.2.2]: https://github.com/Automattic/jetpack-status/compare/v2.2.1...v2.2.2
[2.2.1]: https://github.com/Automattic/jetpack-status/compare/v2.2.0...v2.2.1
[2.2.0]: https://github.com/Automattic/jetpack-status/compare/v2.1.3...v2.2.0
[2.1.3]: https://github.com/Automattic/jetpack-status/compare/v2.1.2...v2.1.3
[2.1.2]: https://github.com/Automattic/jetpack-status/compare/v2.1.1...v2.1.2
[2.1.1]: https://github.com/Automattic/jetpack-status/compare/v2.1.0...v2.1.1
[2.1.0]: https://github.com/Automattic/jetpack-status/compare/v2.0.2...v2.1.0
[2.0.2]: https://github.com/Automattic/jetpack-status/compare/v2.0.1...v2.0.2
[2.0.1]: https://github.com/Automattic/jetpack-status/compare/v2.0.0...v2.0.1
[2.0.0]: https://github.com/Automattic/jetpack-status/compare/v1.19.0...v2.0.0
[1.19.0]: https://github.com/Automattic/jetpack-status/compare/v1.18.5...v1.19.0
[1.18.5]: https://github.com/Automattic/jetpack-status/compare/v1.18.4...v1.18.5
[1.18.4]: https://github.com/Automattic/jetpack-status/compare/v1.18.3...v1.18.4
[1.18.3]: https://github.com/Automattic/jetpack-status/compare/v1.18.2...v1.18.3
[1.18.2]: https://github.com/Automattic/jetpack-status/compare/v1.18.1...v1.18.2
[1.18.1]: https://github.com/Automattic/jetpack-status/compare/v1.18.0...v1.18.1
[1.18.0]: https://github.com/Automattic/jetpack-status/compare/v1.17.2...v1.18.0
[1.17.2]: https://github.com/Automattic/jetpack-status/compare/v1.17.1...v1.17.2
[1.17.1]: https://github.com/Automattic/jetpack-status/compare/v1.17.0...v1.17.1
[1.17.0]: https://github.com/Automattic/jetpack-status/compare/v1.16.4...v1.17.0
[1.16.4]: https://github.com/Automattic/jetpack-status/compare/v1.16.3...v1.16.4
[1.16.3]: https://github.com/Automattic/jetpack-status/compare/v1.16.2...v1.16.3
[1.16.2]: https://github.com/Automattic/jetpack-status/compare/v1.16.1...v1.16.2
[1.16.1]: https://github.com/Automattic/jetpack-status/compare/v1.16.0...v1.16.1
[1.16.0]: https://github.com/Automattic/jetpack-status/compare/v1.15.4...v1.16.0
[1.15.4]: https://github.com/Automattic/jetpack-status/compare/v1.15.3...v1.15.4
[1.15.3]: https://github.com/Automattic/jetpack-status/compare/v1.15.2...v1.15.3
[1.15.2]: https://github.com/Automattic/jetpack-status/compare/v1.15.1...v1.15.2
[1.15.1]: https://github.com/Automattic/jetpack-status/compare/v1.15.0...v1.15.1
[1.15.0]: https://github.com/Automattic/jetpack-status/compare/v1.14.3...v1.15.0
[1.14.3]: https://github.com/Automattic/jetpack-status/compare/v1.14.2...v1.14.3
[1.14.2]: https://github.com/Automattic/jetpack-status/compare/v1.14.1...v1.14.2
[1.14.1]: https://github.com/Automattic/jetpack-status/compare/v1.14.0...v1.14.1
[1.14.0]: https://github.com/Automattic/jetpack-status/compare/v1.13.6...v1.14.0
[1.13.6]: https://github.com/Automattic/jetpack-status/compare/v1.13.5...v1.13.6
[1.13.5]: https://github.com/Automattic/jetpack-status/compare/v1.13.4...v1.13.5
[1.13.4]: https://github.com/Automattic/jetpack-status/compare/v1.13.3...v1.13.4
[1.13.3]: https://github.com/Automattic/jetpack-status/compare/v1.13.2...v1.13.3
[1.13.2]: https://github.com/Automattic/jetpack-status/compare/v1.13.1...v1.13.2
[1.13.1]: https://github.com/Automattic/jetpack-status/compare/v1.13.0...v1.13.1
[1.13.0]: https://github.com/Automattic/jetpack-status/compare/v1.12.0...v1.13.0
[1.12.0]: https://github.com/Automattic/jetpack-status/compare/v1.11.2...v1.12.0
[1.11.2]: https://github.com/Automattic/jetpack-status/compare/v1.11.1...v1.11.2
[1.11.1]: https://github.com/Automattic/jetpack-status/compare/v1.11.0...v1.11.1
[1.11.0]: https://github.com/Automattic/jetpack-status/compare/v1.10.0...v1.11.0
[1.10.0]: https://github.com/Automattic/jetpack-status/compare/v1.9.5...v1.10.0
[1.9.5]: https://github.com/Automattic/jetpack-status/compare/v1.9.4...v1.9.5
[1.9.4]: https://github.com/Automattic/jetpack-status/compare/v1.9.3...v1.9.4
[1.9.3]: https://github.com/Automattic/jetpack-status/compare/v1.9.2...v1.9.3
[1.9.2]: https://github.com/Automattic/jetpack-status/compare/v1.9.1...v1.9.2
[1.9.1]: https://github.com/Automattic/jetpack-status/compare/v1.9.0...v1.9.1
[1.9.0]: https://github.com/Automattic/jetpack-status/compare/v1.8.4...v1.9.0
[1.8.4]: https://github.com/Automattic/jetpack-status/compare/v1.8.3...v1.8.4
[1.8.3]: https://github.com/Automattic/jetpack-status/compare/v1.8.2...v1.8.3
[1.8.2]: https://github.com/Automattic/jetpack-status/compare/v1.8.1...v1.8.2
[1.8.1]: https://github.com/Automattic/jetpack-status/compare/v1.8.0...v1.8.1
[1.8.0]: https://github.com/Automattic/jetpack-status/compare/v1.7.6...v1.8.0
[1.7.6]: https://github.com/Automattic/jetpack-status/compare/v1.7.5...v1.7.6
[1.7.5]: https://github.com/Automattic/jetpack-status/compare/v1.7.4...v1.7.5
[1.7.4]: https://github.com/Automattic/jetpack-status/compare/v1.7.3...v1.7.4
[1.7.3]: https://github.com/Automattic/jetpack-status/compare/v1.7.2...v1.7.3
[1.7.2]: https://github.com/Automattic/jetpack-status/compare/v1.7.1...v1.7.2
[1.7.1]: https://github.com/Automattic/jetpack-status/compare/v1.7.0...v1.7.1
[1.7.0]: https://github.com/Automattic/jetpack-status/compare/v1.6.0...v1.7.0
[1.6.0]: https://github.com/Automattic/jetpack-status/compare/v1.5.0...v1.6.0
[1.5.0]: https://github.com/Automattic/jetpack-status/compare/v1.4.0...v1.5.0
[1.4.0]: https://github.com/Automattic/jetpack-status/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/Automattic/jetpack-status/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/Automattic/jetpack-status/compare/v1.1.1...v1.2.0
[1.1.1]: https://github.com/Automattic/jetpack-status/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/Automattic/jetpack-status/compare/v1.0.4...v1.1.0
[1.0.4]: https://github.com/Automattic/jetpack-status/compare/v1.0.3...v1.0.4
[1.0.3]: https://github.com/Automattic/jetpack-status/compare/v1.0.2...v1.0.3
[1.0.2]: https://github.com/Automattic/jetpack-status/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/Automattic/jetpack-status/compare/v1.0.0...v1.0.1
