# Time

A lightweight single-page web app for viewing the current time across multiple time zones.

## Features
- Real-time local clock with DST status and countdown to the next daylight saving change.
- Searchable world clock cards with automatic persistence in `localStorage`.
- Quick toggles for 12/24-hour display and resetting to the default city list.
- Accessible, responsive layout with dark and light mode support.

## Getting Started
Open `index.html` directly in any modern browser. No build tools or dependencies are required.

1. Clone or download this repository.
2. Open the `index.html` file in your browser.
3. Add or remove cities using the form to customize your world clock grid.

## Development Notes
- The app relies on the browser's `Intl.DateTimeFormat` APIs and geolocation. Location lookups gracefully fall back to IP-based search if geolocation permissions are denied.
- Time zone cards are persisted via `localStorage`; clearing browser storage resets the grid to defaults.

## License
This project is provided as-is without warranty.
