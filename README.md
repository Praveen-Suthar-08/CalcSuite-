# CalcSuite

CalcSuite is a responsive, frontend-only web application that brings multiple everyday calculators into one interface.

## Features

- **Dashboard** — quick access to every calculator
- **Basic Calculator** — arithmetic operations, keyboard input and calculation history
- **Scientific Calculator** — trigonometric functions, logarithms, square root, powers, factorial, constants and DEG/RAD mode
- **BMI Calculator** — metric and imperial calculations with category indicator
- **Unit Converter** — length, weight, temperature, area, volume, speed, data and time
- **Currency Converter** — common currencies with live-rate attempt and built-in fallback rates
- **Age Calculator** — exact age and next-birthday countdown
- **Date Calculator** — date difference and add/subtract days
- **Dark / Light Mode** — theme preference stored in the browser
- **Local History** — recent calculator results stored with `localStorage`
- **Responsive UI** — desktop, tablet and mobile layouts

## Project Structure

```text
CalcSuite-/
├── index.html
├── index-bundled.html
├── README.md
├── css/
│   └── style.css
├── js/
│   └── app.js
└── assets/
    └── icons/
        └── favicon.svg
```

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Browser LocalStorage
- Public exchange-rate endpoint for optional live currency rates

## How It Works

The project is entirely client-side. The main page provides the application layout, `css/style.css` contains the presentation and responsive styling, and `js/app.js` contains calculator logic and UI interactions.

The currency calculator first attempts to load current rates from the Frankfurter API. When that request is unavailable, the app continues working with bundled reference rates.

## Running Locally

Open `index.html` directly in a browser, or serve the project directory with any static HTTP server.

## Project Notes

- No backend or database is required.
- Calculator history and theme settings remain in the user's browser.
- `index-bundled.html` is a standalone version that keeps the styling and JavaScript inside the HTML file.
