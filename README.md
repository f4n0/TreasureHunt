# Treasure Hunt QR Code Tracker

A simple web-based system for creating and tracking progress in treasure hunts using QR codes. This project consists of two main components: an admin page for generating QR codes and a tracker page for participants to view their progress.

## Features

- **Create QR codes for treasure hunt steps**: Generate unique QR codes for each step in your treasure hunt
- **Multiple treasure hunts**: Organize steps by different treasure hunt titles
- **Mobile-friendly**: Responsive design works on both desktop and mobile devices
- **Local storage**: Progress is saved in the browser's local storage
- **Easy to use**: No server or database required - everything works client-side
- **Customizable**: Add emojis to make each step visually distinctive

## Pages

### 1. Admin Page [Admin Page](https://f4n0.github.io/TreasureHunt/admin.html)

A tool for treasure hunt creators to:
- Define a treasure hunt title
- Create steps with custom names
- Assign unique emojis to each step
- Generate and download QR codes for printing

[Admin Page](https://f4n0.github.io/TreasureHunt/admin.html)

### 2. Tracker Page [Tracker Page](https://f4n0.github.io/TreasureHunt/)

A progress tracker for participants that:
- Displays the steps completed in the current treasure hunt
- Updates automatically when scanning new QR codes
- Shows completion timestamps for each step
- Allows clearing progress for the current hunt

[Tracker Page](https://f4n0.github.io/TreasureHunt/)

## How It Works

1. **Setup**: The admin creates QR codes for each step in the treasure hunt using the admin page
2. **Distribution**: The generated QR codes are printed and placed at appropriate locations
3. **Participation**: Players scan QR codes with their mobile devices as they find them
4. **Tracking**: The index page automatically tracks and displays their progress

## Technical Details

- Built with HTML, CSS, and JavaScript
- Uses the QRCode.js library for generating QR codes
- Uses EmojioneArea for emoji selection in the admin interface
- Stores data in localStorage for persistence
- Responsive design with Bootstrap 5

## QR Code Data Structure

Each QR code contains JSON data encoded in base64 with:
- Treasure hunt title
- Step name
- Associated emoji

## Usage Instructions

### For Administrators:

1. Open [Admin Page](https://f4n0.github.io/TreasureHunt/admin.html) in your browser
2. Enter a title for your treasure hunt
3. Create each step by specifying:
   - Step name
   - Associated emoji
4. Click "Generate QR Code"
5. Click on the generated QR code to download it
6. Print and place QR codes at the appropriate locations

### For Participants:

1. Scan a QR code with your device's camera
2. The browser will open to `index.html` showing your current progress
3. Continue scanning QR codes as you find them
4. Your progress is saved automatically in your browser
5. Use the "Cancel Progress" button to reset if needed

## Browser Compatibility

- Works on modern browsers with localStorage support
- Compatible with Chrome, Firefox, Safari, and Edge
- Requires JavaScript to be enabled

## License

This project is open source and available for personal and educational use.

## Credits

- [QRCode.js](https://github.com/davidshimjs/qrcodejs) for QR code generation
- [Bootstrap](https://getbootstrap.com/) for styling
- [jQuery](https://jquery.com/) for easier DOM manipulation
- [EmojioneArea](https://github.com/mervick/emojionearea) for emoji picker