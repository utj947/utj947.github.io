# Lunar Birthday to Google Calendar

A Chrome extension to add lunar birthdays to Google Calendar as solar date events, with emoji icons for a friendly user experience. Automatically converts lunar dates to solar dates, supports leap months, allows bulk event deletion, and offers donation support via PayPal.

## Quick Start

### Installation
1. **Download the Extension**:
   - Clone the repository or download the ZIP and extract it:
     ```bash
     git clone https://github.com/utj99/Lunar2GoogleCalender.git
     ```

2. **Load in Chrome**:
   - Open Chrome and go to `chrome://extensions/`.
   - Turn on **Developer mode** (top-right toggle).
   - Click **Load unpacked** and select the extension folder.
   - The extension icon should appear in your Chrome toolbar.

3. **Check Emoji Images**:
   - Ensure the `images/` folder contains emoji files (e.g., `moon.png`, `sun.png`, `cake.png`, `calendar.png`, `success.png`, `error.png`).
   - Images should be 24x24px PNGs with transparent backgrounds.

### How to Use
1. **Open the Popup**:
   - Click the extension icon in Chrome's toolbar to open the popup window.

2. **Enter Lunar Birthday Details**:
   - **Lunar Month (1-12)**: Enter the month (e.g., 8 for August) next to the 🌙 emoji.
   - **Lunar Day (1-30)**: Enter the day (e.g., 15) next to the ☀️ emoji.
   - **Leap Month**: Check the "윤달" box if the birthday is in a lunar leap month.
   - **Event Name**: Type the event name (e.g., "My Birthday") next to the 🎂 emoji.
   - **Years to Add (1-50)**: Specify how many years to add events for (e.g., 10) next to the 📅 emoji.
   - **Event Color**: Select a color to distinguish the event in your calendar.

3. **Add to Google Calendar**:
   - Click the **Add to Google Calendar** button.
   - Sign in with Google if prompted (requires a Google account).
   - The extension converts the lunar date to solar dates, accounting for leap months, and adds them as all-day events to your Google Calendar.

4. **Delete Events**:
   - Click the **Event Deletion** button.
   - Enter the event name to delete (e.g., "My Birthday") and click **Confirm**.
   - Confirm the deletion in the dialog to remove all matching events from your calendar.

5. **Support the Developer**:
   - If you find the extension useful, consider donating via PayPal to support development!
   - Click the **Donate** button in the popup to contribute.

6. **Check Results**:
   - A success message with a ✅ emoji shows the solar dates added (e.g., "2025: 2025-09-10").
   - If there’s an error, an ❌ emoji appears with a message (e.g., "Check your internet connection").
   - Open Google Calendar to view the added events.

## Example
- Input:
  - Lunar Month: 8 (🌙)
  - Lunar Day: 15 (☀️)
  - Leap Month: Checked (윤달)
  - Event Name: My Birthday (🎂)
  - Years to Add: 3 (📅)
- Output:
  - Events added for leap month years (e.g., 2033) with corresponding solar dates.
  - Status: "Lunar 8/15 (윤달) added to calendar: 2033: 2033-04-04" with ✅ emoji.
- Deletion:
  - Enter "My Birthday" and confirm to remove all related events.

## Troubleshooting
- **Extension doesn’t load**: Ensure all files (`popup.html`, `popup.js`, `background.js`, `manifest.json`) and the `images/` folder are in the correct folder.
- **Emojis not showing**: Check that image files exist in `images/` and paths match (e.g., `images/moon.png`).
- **Google login fails**: Verify your internet connection and try signing in again.
- **Events not added**: Ensure Google Calendar access and correct permissions.
- **Invalid input**: Enter valid numbers (Month: 1-12, Day: 1-30, Years: 1-50).
- **Leap month issues**: Ensure the leap month checkbox is correctly set for lunar leap years.

## Notes
- The extension uses your Google account to add and delete events securely.
- Emoji icons (🌙, ☀️, 🎂, 📅, ✅, ❌) enhance the interface.
- Cached data ensures faster conversions for repeated dates.
- Supports up to 50 years of events, with leap month calculations for accuracy.
- Donations via PayPal help maintain and improve the extension.

## Support
For issues, suggestions, or to contribute, open an issue on the [GitHub repository](https://github.com/utj99/Lunar2GoogleCalender/issues) or contact [utj947@gmail.com](mailto:utj99@example.com).

If you enjoy this extension, please consider supporting development with a donation:
- [Donate via PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YOUR_BUTTON_ID)