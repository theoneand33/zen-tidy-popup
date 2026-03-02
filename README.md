# Zen Tidy Popup

A clean, standalone theme for Zen Browser and Firefox that modifies popup panels with compact buttons, modern hover colors, and a tidier interface.

## Features

- 🎨 **Clean Popup Design** - Rounded corners, refined borders, and smooth shadows
- 📏 **Compact Buttons** - Makes popup buttons more compact and visually appealing
- 🌈 **Custom Hover Colors** - Beautiful blue hover effect that works in both light and dark themes
- 🎯 **Zen Primary Color Integration** - Automatically uses Zen Browser's primary color for hover states
- 🔧 **Universal Compatibility** - Works with both Zen Browser and Firefox - no mod manager required!
- 📚 **Tidy Extension Panel** - Cleans up the unified extensions popup for a more organized look
- ⚡ **Lightweight** - Simple CSS with no dependencies or configuration needed

## Installation

### Method 1: Using a UserChrome.css (Recommended)

1. Locate your browser profile folder
2. Create a folder called `chrome` in your profile directory if it doesn't exist
3. Copy `chrome.css` from this repository into the `chrome` folder
4. Restart your browser

The theme will be automatically applied on startup.

### Method 2: As a Simple Extension

For a more flexible installation:

1. Create a new folder for the extension
2. Add a `manifest.json` file pointing to `chrome.css` as a user stylesheet
3. Load the extension in your browser via `about:debugging`

## Customization

The theme uses Zen Browser's primary color for hover effects by default. To customize the color, edit the `chrome.css` file and modify the CSS variables:

```css
:root {
  --mod-forkedtidypopup-hovercolor-light-final: rgba(80, 80, 250, 0.75);
  --mod-forkedtidypopup-hovercolor-dark-final: rgba(80, 80, 250, 0.75);
}
```

Replace the rgba values with your preferred colors.

## What This Theme Does

- Compact button styling: Smaller, rounded, consistent hit areas
- Enhanced hover effects: Blue hover color that integrates with Zen Browser's primary color
- Modern panel design: Rounded corners, refined borders and shadows
- Better spacing: Optimized padding and margins for a cleaner look
- Tidy extensions panel: Streamlined unified extensions popup with improved layout and spacing

## How it works

The theme applies CSS styling directly to Firefox/Zen Browser UI elements:
- All features are enabled by default (no configuration needed)
- Hover colors use Zen Browser's primary color when available, with a fallback to the default blue
- Light/Dark hover colors automatically follow your system color scheme
- Simply place `chrome.css` in your profile's `chrome/` folder and restart

## Compatibility

- ✅ Zen Browser
- ✅ Firefox

## Credits

Originally forked from [Dinno-DEV/zen-tidy-popup](https://github.com/Dinno-DEV/zen-tidy-popup)

Enhanced with additional customization options and improved styling.

## Contributing

Found a bug or want to suggest an improvement? Feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/rasyidrafi/zen-tidy-popup/).

## License

This project is open source and available under standard open source terms.

## Author

Modified and enhanced by [rasyidrafi](https://github.com/rasyidrafi)

---