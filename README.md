# Better Firefox

A collection of Firefox vertical tabs configuration flags and CSS customizations to enhance your browsing experience with improved UI and functionality.

![image](https://github.com/user-attachments/assets/ef19e084-7e4a-4f5f-ba16-c95fa2495a6c)

## Features

- 🎨 Custom CSS styling support
- 🛠️ Browser toolbox debugging capabilities
- 📌 Enhanced pinned tab management
- 🏗️ Floating browser container
- 📋 Horizontal sidebar layout
- ⚡ Optimized startup performance

## Installation

### Step 1: Enable Custom CSS

1. Open Firefox and type `about:config` in the address bar
2. Click "Accept the Risk and Continue"
3. Search for each configuration flag listed below and set the values accordingly

### Step 2: Browser Configuration

Set these flags in `about:config`:

| Flag | Value | Purpose |
|------|-------|---------|
| `toolkit.legacyUserProfileCustomizations.stylesheets` | `true` | Enable custom CSS |
| `devtools.debugger.remote-enabled` | `true` | Enable browser toolbox |
| `devtools.chrome.enabled` | `true` | Enable browser toolbox shortcut |
| `browser.sessionstore.restore_pinned_tabs_on_demand` | `true` | Disable auto load pinned bookmarks on startup |
| `browser.tabs.loadBookmarksInTabs` | `true` | Open bookmarks in new tab |
| `browser.tabs.closeWindowWithLastTab` | `false` | Prevent browser close when closing last tab |

### Step 3: User Customization Flags

Create and configure these custom flags in `about:config`:

| Flag | Value | Feature |
|------|-------|---------|
| `user.floating-browser-container` | `true` | Floating browser container |
| `user.increase-pinned-tab-height` | `true` | Increase pinned tab height |
| `user.add-pinned-separator` | `true` | Add pinned tab separator |
| `user.disable-status-bar` | `true` | Disable status bar |
| `user.horizontal-sidebar` | `true` | Enable horizontal sidebar |
| `user.horizontal-sidebar.hide-extensions` | `true` | Hide sidebar extensions |
| `user.horizontal-sidebar.hide-specific-extension` | `true` | Hide specific extensions |

### Step 4: Apply CSS Files

1. Find your Firefox profile folder:
   - Type `about:profiles` in the address bar
   - Look for "Profile: default" and click "Open Directory" under the 'Root Directory' section.

2. Create a new folder named `chrome` in your profile directory (if it doesn't already exist).

3. Place the CSS files from this repository into the `chrome` folder

4. Restart Firefox to apply changes

## Troubleshooting

**CSS not loading?**
- Ensure `toolkit.legacyUserProfileCustomizations.stylesheets` is set to `true`
- Verify CSS files are in the correct `chrome` folder
- Restart Firefox after making changes

**Flags not working?**
- Double-check flag names are spelled exactly as shown
- Ensure values are set correctly (true/false)

**Want to revert changes?**
- Set flags back to `false` or delete custom flags
- Remove CSS files from the `chrome` folder
- Restart Firefox

## License

This project is open source and available under the [MIT License](LICENSE).
