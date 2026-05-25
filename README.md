# Star Generator

A simple, browser-based star rating code generator that lets you build customizable HTML star-rating snippets in seconds.

![Star Generator Screenshot](https://raw.githubusercontent.com/jsammarco/Star_Generator/refs/heads/main/screenshots/screenshot.PNG)

## Overview

Star Generator is a lightweight single-page tool for creating star-rating HTML with a live preview. It is designed for quick visual customization without any build step, dependencies, or server setup.

You can adjust:

- Rating value
- Maximum number of stars
- Star size
- Star spacing
- Base image URL path
- Optional text before or after the stars
- Output tag style (`span`, `h1`, `h2`, `h3`, or `h4`)

## Features

- Live preview as you edit settings
- Generated HTML ready to copy into a webpage or template
- Support for full, half, and empty star states
- Download links for the star image assets
- Cookie-based setting persistence in the browser
- Standalone `index.html` with no install process

## Files

- `index.html` - the complete app UI, styles, and generator logic
- `star.png` - full star image
- `half_star.png` - half star image
- `no_star.png` - empty star image
- `screenshots/screenshot.PNG` - project screenshot

## Getting Started

1. Clone or download this repository.
2. Open `index.html` in any modern web browser.
3. Adjust the controls to match your desired rating output.
4. Copy the generated HTML from the output box.
5. Use the included image assets or point the base URL to your hosted copies.

## How It Works

The generator builds a sequence of `<img>` tags based on the selected rating and maximum star count. For each position, it chooses one of these images:

- `star.png` for a full star
- `half_star.png` for a half star
- `no_star.png` for an empty star

It then wraps the output in the selected heading tag, or leaves it inline when `span` is selected.

## Example Output

```html
<h3>
<img src="https://example.com/star.png" width="32" style="vertical-align:middle; margin-right:-5px;">
<img src="https://example.com/star.png" width="32" style="vertical-align:middle; margin-right:-5px;">
<img src="https://example.com/half_star.png" width="32" style="vertical-align:middle; margin-right:-5px;">
<img src="https://example.com/no_star.png" width="32" style="vertical-align:middle; margin-right:-5px;">
</h3>
```

## Use Cases

- Product ratings
- Review summaries
- Landing pages
- CMS content blocks
- Simple embedded widgets

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
