# JamShoot

We build private, offline-first apps for iPhone, iPad and Mac.
And we open-source the tools we use to ship them.

## Open source

### [JamShoot Design](https://github.com/jamshoot-apps/jamshoot-design)

A design system for static sites. Components are plain JavaScript functions that render HTML at build time. There is no client framework and there are no npm dependencies.

- Component options are validated at build time, and a bad option stops the build with a clear error
- Theming uses twelve color roles, with light and dark palettes and a theme control
- `jamshoot-lint` checks contrast, focus styles, tap target size, reduced motion and more
- API tables are generated from code, and README examples run as tests
- The CLI includes `jamshoot-build`, `jamshoot-dev` with live reload, and `jamshoot-og-image`

Node.js 22+ · `npm install @jamshoot-apps/design` · [Documentation](https://jamshoot-apps.github.io/jamshoot-design/)

### [JamShoot Studio](https://github.com/jamshoot-apps/jamshoot-studio)

Composes App Store screenshots from app screenshots, localized text and a portable JSON project. Use the local browser editor, or the CLI in CI pipelines and LLM agents.

- 62 built-in App Store sizes for iPhone, iPhone Duo, iPad and Mac, plus custom sizes
- Text per language, and variants of the whole set such as light and dark
- The CLI validates, plans and renders, with JSON output and exit codes for CI
- A single Pillow renderer handles preview and export, and writes a SHA-256 manifest for every PNG
- Runs locally and offline, with no Node.js or headless browser

Python 3.11+ · [Documentation](https://jamshoot-apps.github.io/jamshoot-studio/)

## Used in production

Every JamShoot app website is built with JamShoot Design. Every App Store screenshot we ship is rendered with JamShoot Studio.

- [CullBit](https://cullbit.jamshoot.net/) — photo culling for iPhone, iPad and Mac
- [YellChef](https://yellchef.jamshoot.net/) — hands-free cooking for iPhone and iPad
- [WireTrap](https://wiretrap.jamshoot.net/) — mic and camera activity for Mac

## Principles

- **Few dependencies.** We use the standard library first, and add a dependency only when it earns its place.
- **Local and offline.** No account and no network required.
- **Fail early.** Errors surface at build or validation time, not in production.
- **Automation-friendly.** Machine-readable output, stable exit codes, and docs that work for people and coding agents.
- **Docs that stay true.** Examples are tested, and reference docs are generated from source.

## Contributing

Issues and pull requests are welcome. Each repository has its own `CONTRIBUTING.md`. Report security issues privately as described in `SECURITY.md`, not in public issues.

## License

Open-source projects are licensed under [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0). The JamShoot name, logo and brand artwork are excluded. See `NOTICE` in each repository. The apps are proprietary.

[jamshoot.net](https://jamshoot.net/)
