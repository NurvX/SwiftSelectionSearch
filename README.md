
# Swift Selection Search

A browser extension that automatically displays search engine icons when you select text, allowing for quick and convenient searches across multiple engines.

## Features

- **Text Selection Detection**: Automatically shows search icons when text is selected on any webpage
- **Multiple Search Engines**: Quick access to popular search engines like Google, Bing, DuckDuckGo, etc.
- **Customizable Options**: Configure which search engines to display and their order
  - Per-engine pop-up and context menu toggles
  - Global disable options for all pop-ups and context menus
- **Clipboard Integration**: Copy selected text to clipboard for easy pasting
- **Context Menu Support**: Right-click selected text to access search engines via context menu
- **Import/Export Settings**: Backup and restore your search engine configurations
- **Manifest V3 Compatible**: Built with the latest Chrome extension standards for better performance and security

## Installation

### From Source

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd swift-selection-search
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Build the extension:
   ```bash
   npm run build
   ```

4. Load in your browser:
   - **Chrome/Edge**: Open `chrome://extensions/`, enable "Developer mode", click "Load unpacked", and select the `dist/` folder
   - **Firefox**: Open `about:debugging`, click "This Firefox", click "Load Temporary Add-on", and select `manifest.json` from the `dist/` folder

## Development

- `npm run dev` - Start the development server with hot reload
- `npm run build` - Build the extension for production
- `npm run test` - Run tests (currently not implemented)

## Project Structure

- `src/` - Source TypeScript files
  - `content.ts` - Content script for text selection handling
  - `background.ts` - Background service worker
  - `options.ts` - Options page logic
  - `types.ts` - TypeScript type definitions
- `dist/` - Built extension files (generated)
- `manifest.json` - Extension manifest
- `vite.config.ts` - Vite build configuration

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## Privacy Policy

See [PRIVACY.md](PRIVACY.md) for our privacy policy.

## License

This project is licensed under the ISC License - see the package.json file for details.

## Changelog

See [changelog.md](changelog.md) for version history and updates.