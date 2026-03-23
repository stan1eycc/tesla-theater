# Tesla Theater ⚡

A minimal, zero-dependency fullscreen streaming launcher for Tesla's in-car browser.

## How It Works

Tesla's browser grants fullscreen privileges to YouTube. This project leverages YouTube's redirect endpoint (`youtube.com/redirect?q=<url>`) to open any streaming service in fullscreen mode — creating a seamless, TV-like experience.

## Usage

1. Open the GitHub Pages URL in your Tesla's browser
2. Tap **Launch Fullscreen** to enter fullscreen mode
3. Select a streaming service from the dashboard

## Features

- **Single-file** — pure HTML/CSS/JS, no frameworks or build tools
- **4 categories** — Video, Music, Tools, Kids
- **Dark theme** — optimized for in-car displays
- **Tab navigation** — quick switching between categories
- **Easy to customize** — edit `index.html` to add/remove services

## Customization

Each service is a `<a class="card">` element in `index.html`. To add a new one:

1. Add an SVG icon to `icons/`
2. Add a card entry in the appropriate tab section:

```html
<a class="card" href="#" data-url="https://example.com">
  <img src="icons/example.svg" alt="Example">
  <span>Example</span>
</a>
```

## Notes

- Fullscreen does not work when the car is in Park with hazard lights flashing
- A valid subscription is required for each streaming platform

## License

MIT
