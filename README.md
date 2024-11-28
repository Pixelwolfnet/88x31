# 88x31 Button Generator

The **88x31 Button Generator** is a simple tool designed to recreate the nostalgic, old-school buttons that were popular on 90s websites. These tiny, pixel-perfect buttons are perfect for adding a retro aesthetic to your modern projects.

---

## Features

- **Customizable Buttons**: Create buttons with custom text, colors, fonts, and borders.
- **Real-Time Preview**: See your changes instantly in the preview window.
- **Export as GIF**: Generate animated `.gif` files using [gif.js](https://github.com/jnordberg/gif.js) and `worker.gif.js`.
- **Retro Fonts**: Supports classic fonts like `MS Sans Serif` and `Chicago`.
- **Styling Options**: Customize text effects such as blink, rainbow, pulse, fade, flicker, and glow.

---

## Getting Started

### Prerequisites

To run this project, you’ll need:
- A modern browser that supports JavaScript, HTML5, and CSS3.
- A local server or web hosting environment if you plan to modify and test the code.

### Installation

1. Clone or download the project repository:
   ```bash
   git clone https://github.com/Pixelwolfnet/88x31.git
   ```
2. Open `index.html` in your browser.

---

## How to Use

1. **Load the Page**: Open the `index.html` file in a browser.
2. **Customize Your Button**:
   - Enter text in the input field.
   - Adjust colors, border styles, and font using the controls.
   - Select text effects like glow or animations such as pulse and flicker.
3. **Preview**: View your button in the real-time preview section.
4. **Export**: Save your creation as a `.gif` using the export button.

---

## Known Issues

- **Border Export Issues**: `inset` and `outset` borders may not render correctly when exported.
- **Glow Animation**: The glow animation effect is currently not functioning as intended.

We are working to resolve these issues in future updates.

---

## Technologies Used

- **JavaScript**:
  - Handles real-time updates and gif generation using [gif.js](https://github.com/jnordberg/gif.js).
- **HTML/CSS**:
  - Provides the retro-inspired user interface and styling.
- **Fonts**:
  - `MS Sans Serif` and `Chicago` for authentic 90s vibes.

---

## Style Guide

```html
<style>
  /* Retro theme setup */
  body {
    background: #008080;
    font-family: "MS Sans Serif", Arial, sans-serif;
    color: black;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
  }
  .container {
    background: #c0c0c0;
    border: outset 3px #fff;
    padding: 10px;
    max-width: 512px;
  }
  .button-preview {
    width: 88px;
    height: 31px;
    background: black;
    margin: 0 auto;
    border: 1px solid black;
  }
  .glow {
    text-shadow: 0 0 5px currentColor;
  }
  /* Animation styles */
  @keyframes blink {
    0%, 100% { opacity: 1; }
    50% { opacity: 0; }
  }
  .blink {
    animation: blink 1s infinite;
  }
</style>
```

---

## Contributing

We welcome contributions! If you have suggestions, feature requests, or bug fixes, feel free to open an issue or submit a pull request.

---

## License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## Credits

- **Fonts**:
  - `MS Sans Serif` and `Chicago` provided by [Pixelwolf](https://pixelwolf.net/fonts/).
- **GIF Generation**:
  - Powered by [gif.js](https://github.com/jnordberg/gif.js).
