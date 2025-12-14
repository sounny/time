# Time

A lightweight single-page web app for viewing the current time across multiple time zones. Everything runs in the browser—no builds or dependencies required.

## Features
- Real-time hero clock with daylight saving status and a countdown to the next DST change for the pinned zone.
- Pin any time zone to make it the main clock while keeping the local zone visible.
- Searchable, sortable world clock cards with drag-and-drop reordering and per-card offset labels.
- Add new IANA time zones, remove cards, or reset back to the default list; preferences persist in `localStorage`.
- Quick toggle between 12/24-hour formats plus accessible, responsive layout with light and dark mode support.

## Getting Started
Open `index.html` directly in any modern browser.

1. Clone or download this repository.
2. Open the `index.html` file in your browser (no server needed).
3. Add or remove cities using the form, drag cards to reorder, and pin a zone to set the primary clock.

## Development Notes
- The app uses the browser's `Intl.DateTimeFormat` APIs for formatting and validates time zones via the same interface.
- Supported zones populate the add form's datalist (falling back to a curated list where necessary).
- Time zone list, main clock pin, and 12/24-hour preference are saved in `localStorage`; clearing storage resets to defaults.
- Location messaging prefers the device's time zone and attempts a quick IP-based lookup for a friendlier label.

## License
This project is provided as-is without warranty.
