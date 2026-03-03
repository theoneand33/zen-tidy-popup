# Tidy Popup v2

A clean theme for Zen Browser that makes popup panels compact and modern.

## Installation

1. Open `about:config` and accept the warning
2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`
3. Open `about:profiles` and locate your profile folder
4. Copy `chrome.css` from this repository into the `chrome` folder
5. Rename it to `userChrome.css`
6. Restart your browser

The theme will be automatically applied on startup.

## What This Theme Does

- Compact button styling: Smaller, rounded, consistent hit areas
- Enhanced hover effects: Blue hover color that integrates with Zen Browser's primary color
- Modern panel design: Rounded corners, refined borders and shadows
- Better spacing: Optimized padding and margins for a cleaner look
- Tidy extensions panel: Streamlined unified extensions popup with improved layout and spacing
- Fully customizable: Extensive preferences for spacing, radius, shadows, animations, and layout density

## Compatibility

- Zen Browser (tested with version 1.0.0 and above)

## Preferences

Tidy Popup v2 offers extensive customization through the Zen Browser mod settings. All preferences can be adjusted in `about:preferences#zen-mods`.

### Appearance

- **Use Zen Browser primary color for hover effects** (checkbox, default: true)
  - Uses Zen's theme color instead of the default blue
- **Button color when hovered (Light mode)** (string, default: `rgba(80, 80, 250, 0.75)`)
  - Custom CSS color value, only used if Zen primary color is disabled
- **Button color when hovered (Dark mode)** (string, default: `rgba(80, 80, 250, 0.75)`)
  - Custom CSS color value for dark mode, only used if Zen primary color is disabled

### Layout & Spacing

- **Popup padding** (string, default: `6px`)
  - Controls the inner spacing of popup containers. Accepts any CSS unit (px, em, rem, %)
- **Popup border radius** (string, default: `8px`)
  - Controls the roundness of popup container corners
- **Button border radius** (string, default: `8px`)
  - Controls the roundness of buttons and menu items
- **Layout density mode** (dropdown: Compact or Extended, default: Compact)
  - **Compact**: Smaller padding (4px 8px) and tighter margins for space-saving
  - **Extended**: Larger padding (8px 16px) and more spacing for comfortable use
- **Compact mode button margin** (string, default: `var(--arrowpanel-menuitem-margin)`)
  - Custom margin for buttons in compact mode (only visible when Compact mode is selected)
- **Extended mode button margin** (string, default: `4px`)
  - Custom margin for buttons in extended mode (only visible when Extended mode is selected)

### Effects

- **Enable smooth hover animations** (checkbox, default: true)
  - Toggles smooth transition effects on hover
- **Transition duration** (string, default: `0.15s`)
  - Speed of hover animations (e.g., 0.15s, 200ms). Only used when animations are enabled
- **Transition timing function** (dropdown: Ease, Linear, Ease In, Ease Out, Ease In Out, default: Ease)
  - Controls the easing curve of animations. Only used when animations are enabled

### Shadow Customization

- **Popup box-shadow** (string, default: `var(--panel-shadow)`)
  - Custom shadow effect for popup containers. Can use CSS shadow values or browser variables
- **Popup shadow margin** (string, default: `var(--panel-shadow-margin)`)
  - Space between popup and shadow. Accepts any CSS length value

## Tips & Examples

### Using rem units for scalable sizing
Set "Popup padding" to `0.5rem` and "Popup border radius" to `0.5rem` to scale with your browser's base font size.

### Creating a flat design
Set "Popup box-shadow" to `none` and reduce "Popup border radius" to `2px` or `0`.

### Matching your Zen theme
Enable "Use Zen Browser primary color" to automatically match your Zen Browser theme's accent color for hover states.

### Complete flat look with fast transitions
- Popup box-shadow: `none`
- Popup border radius: `2px`
- Enable smooth hover animations: unchecked

### High-DPI displays
If you're on a high-DPI (Retina) display and want crisper borders, you can increase the border radius slightly (e.g., `10px` instead of `8px`) and adjust padding accordingly.

## Troubleshooting

### The theme isn't applying
1. Verify `toolkit.legacyUserProfileCustomizations.stylesheets` is set to `true` in `about:config`
2. Confirm `chrome.css` is in your profile's `chrome` folder and renamed to `userChrome.css`
3. Restart Zen Browser completely (not just reload windows)
4. Check `about:debugging` > "This Firefox" > "Load Temporary Add-on" to see if there are any CSS errors

### Preferences not showing in Zen Mods settings
- Make sure you have the latest version of Zen Browser (the mods system is constantly evolving)
- Check that `preferences.json` is in the same directory as `chrome.css`
- The mod name should be "Tidy Popup v2" in the mods registry

### Popup shadows look weird
Try setting "Popup box-shadow" to `var(--panel-shadow)` (default) or experiment with custom values like `0 4px 12px rgba(0,0,0,0.15)`. If you want no shadow, set it to `none`.

### Hover effects not working
1. Ensure "Enable smooth hover animations" is checked if you want smooth transitions
2. Check that your hover color values are valid CSS colors
3. Verify that the correct color scheme (light/dark) preference values are set

### Buttons look too small/large
Adjust the "Popup padding" and "Layout density mode" preferences. You can also fine-tune compact/extended mode margins separately.

### Conflicts with other mods
If you have other mods that modify popup styling, they may conflict. Try disabling other mods temporarily to identify the culprit. You can also adjust the specificity of selectors if needed.

###Preferences reset after browser update
Your preferences are stored in your Firefox profile and should persist. If they reset, check that your profile is not being overwritten by sync or backup tools.

## Advanced Customization

All preferences are stored as Firefox about:config preferences with the prefix `mod.tidypopupv2.`. You can manually edit them in `about:config` for more control.

For example:
- `mod.tidypopupv2.popupsize` controls the popup padding
- `mod.tidypopupv2.usezenprimarycolor` toggles the Zen color integration

## Credits

Originally forked from [Dinno-DEV/zen-tidy-popup](https://github.com/Dinno-DEV/zen-tidy-popup)  
Then forked from [rasyidrafi/zen-tidy-popup](https://github.com/rasyidrafi/zen-tidy-popup)  
Maintained by [theoneand33](https://github.com/theoneand33)

## Contributing

Found a bug or want to suggest an improvement? Feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/theoneand33/zen-tidy-popup/).

## License

This project is open source and available under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.

## Authors

[Dinno-DEV](https://github.com/Dinno-DEV)  
[rasyidrafi](https://github.com/rasyidrafi)  
[theoneand33](https://github.com/theoneand33)
