# Tonicue 瞳休

Tonicue 瞳休 is a cute desktop break reminder for screen-heavy work. It runs quietly in the background, tracks active screen time locally, and pops a small always-on-top reminder when it is time to rest your eyes, drink water, stretch your neck, or stand up.

The project is currently an early desktop MVP for Windows and macOS Apple Silicon.

## Features

- Active screen-time tracking, with idle, lock, and sleep handling
- Windows tray and macOS menu bar background mode
- Small right-bottom reminder popup
- Eye rest, water, neck stretch, and stand-up reminders
- Guided rest steps for each reminder type
- 20-second countdown for eye-rest reminders
- Snooze for 1 or 5 minutes
- Focus pause for 30 minutes
- Local daily stats and rhythm feedback
- Local-only settings storage

## Install Preview Builds

Built packages are generated in `dist/`.

Windows:

```text
dist/Tonicue 瞳休 Setup 0.1.5.exe
```

macOS Apple Silicon:

```text
dist/Tonicue 瞳休-0.1.5-arm64.dmg
```

These preview builds are not code-signed yet, so Windows and macOS may show unknown-developer warnings. See [INSTALL.md](INSTALL.md) for friendlier installation steps.

## Development

Requirements:

- Node.js
- npm

Install dependencies:

```bash
npm install
```

Run the app in development:

```bash
npm run dev
```

Run the project structure check:

```bash
npm run lint
```

## Build

Build Windows x64 installer:

```bash
npm run build:win
```

Build macOS Apple Silicon package:

```bash
npm run build:mac
```

Build both:

```bash
npm run build:all
```

## Privacy

Tonicue does not require an account and does not upload usage data. Screen-time stats, reminder settings, and daily state are stored locally through Electron's app data directory.

See [PRIVACY.md](PRIVACY.md) for details.

## Roadmap

- Add screenshots and short demo GIFs
- Split the main process into smaller modules
- Add unit tests for timing and reminder scheduling
- Add ESLint and Prettier
- Add GitHub Actions for lint and build checks
- Add signed installers for public distribution
- Improve brand icon and visual polish

## Contributing

Issues, feature suggestions, and UX feedback are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT. See [LICENSE](LICENSE).
