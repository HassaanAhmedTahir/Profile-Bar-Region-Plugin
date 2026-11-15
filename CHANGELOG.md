# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project follows [Semantic Versioning](https://semver.org/).

## [1.3.0] - 2026-11-15

### Fixed
- Dropdown links and the Logout Target now resolve substitution strings (`&APP_ID.`, `&SESSION.`, `&DEBUG.`, page items) before `apex_util.prepare_url`. Previously links such as `f?p=&APP_ID.:10:&SESSION.` were output literally and didn't navigate correctly.
- Hovered menu text was always white, which made it invisible on the default light hover color (`#F3F4F6`). The hover text color is now chosen automatically from the hover background.
- A literal *Image MIME Type* (e.g. `image/jpeg`) was ignored. It's now used, and invalid values fall back to `image/png`.
- With *Logout Position = Inside* and the dropdown disabled, the logout button disappeared. It now falls back to the outside button.
- The dropdown's right edge was offset by the scrollbar width on scrolling pages.
- The fallback logout icon is now `fa-sign-out` (available in Font APEX and matching the attribute default).

### Changed
- Docs: *Show Status* depends on *Show Image*, since the status dot sits on the avatar.

## [1.2.0]

### Added
- Version published in the original blog post.
