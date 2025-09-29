# FPAC Style

A USDA FPAC design system based on [USWDS](https://designsystem.digital.gov/). 
Provides reusable CSS and documentation to style consistent, accessible web experiences.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)
- [Release Notes](#release-notes)

## Overview

**fpac-style**: CSS implementation of USDA's FPAC Design System  
**fpac-design-system**: Documentation website styled with fpac-style

## Installation

```sh
npm install
npm run build
```

## Usage

Add the following to your `package.json` dependencies:

```json
"@fpac/style": "1.0.0-rc.0"
```

Include the compiled CSS in your project:

```html
<link rel="stylesheet" href="dist/fpac-style/styles/fpac-design-system.css">
```

## Folder Structure

- `fpac-style/` – CSS and design tokens
- `fpac-design-system/` – Documentation website

## Contributing

At this time, we are not accepting external contributions.

## License

This project is licensed under the [CC0 1.0 Universal (Public Domain Dedication)](./LICENSE).

## Release Notes

| Version | Date | Notes |
| ------- | ---- | ----- |
| 0.1     | 04/16/2025 | Initial project setup and wiring for @uswds/uswds |
| 1.0     | 09/29/2025 | Initial release to GitHub |

