# YouTube Sync P2P 🔄

A Chrome extension that allows users to synchronize YouTube video playback across multiple devices using peer-to-peer connections.

![YouTube Sync P2P Logo](images/icon128.png)

## ✨ Features

- **🔄 Real-time Synchronization**: Automatically keeps video playback in sync across multiple devices
- **🔌 Peer-to-Peer Architecture**: Direct connection between devices without requiring a server
- **🚪 Simple Room-based System**: Easy to create and join rooms with shareable codes
- **⏯️ Play/Pause Syncing**: When the host plays or pauses, all connected viewers follow
- **⏩ Seek Position Syncing**: When the host seeks to a different position, all viewers' videos update
- **📊 Status Indicators**: Clear visual feedback about connection status
- **👥 Multiple Viewer Support**: Host can have multiple viewers connected simultaneously

## 📥 Installation

### From Chrome Web Store
*(Coming Soon)*

### Manual Installation
1. Download or clone this repository
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" (toggle in the top-right corner)
4. Click "Load unpacked" and select the extension directory
5. The extension icon should appear in your browser toolbar

## 📝 How to Use

### Hosting a Session
1. Navigate to any YouTube video
2. Click the YouTube Sync P2P extension icon in your toolbar
3. Select the "Host" tab (if not already selected)
4. Click "Create Room"
5. Share the generated room code with friends who want to join your session
6. Control the video playback as usual - all connected viewers will stay in sync

### Joining a Session
1. Get a room code from someone hosting a YouTube Sync session
2. Navigate to the same YouTube video (or any YouTube video - the host's video will load)
3. Click the YouTube Sync P2P extension icon
4. Select the "Join" tab
5. Enter the room code
6. Click "Connect to Room"
7. The video will now stay synchronized with the host's playback

### Leaving a Session
1. Click the YouTube Sync P2P extension icon
2. Click "Leave Room"

## ❓ Troubleshooting

### Common Issues
- **Can't create/join room**: Make sure you're on a YouTube video page
- **Synchronization issues**: Check your internet connection
- **Video not loading**: Ensure you're on the same video as the host
- **Connection lost**: The host may have closed their session or browser

### Debugging
If you encounter issues:
1. Open Chrome DevTools (F12 or Ctrl+Shift+I)
2. Check the console for error messages
3. Try refreshing the page and reconnecting

## 🔒 Privacy and Security

- All connections are peer-to-peer
- No data is stored on external servers
- Room codes are randomly generated and temporary
- Only basic video playback information is shared between peers

## 💻 Technical Details

- Built with JavaScript
- Uses PeerJS for WebRTC peer-to-peer connections
- Chrome storage API for session persistence
- Supports modern YouTube SPA navigation

## 🛠️ Development

### Project Structure
- `manifest.json`: Extension configuration
- `popup.html` & `popup.js`: Extension popup interface
- `content.js`: Content script that interacts with YouTube
- `background.js`: Background service worker
- `peerjs.min.js`: PeerJS library for WebRTC connections

### Building from Source
1. Clone the repository
2. Make your changes
3. Load the extension in Chrome using Developer mode

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👏 Acknowledgments

- [PeerJS](https://peerjs.com/) for WebRTC simplification
- [Font Awesome](https://fontawesome.com/) for icons

## 🔮 Future Plans

- Firefox support
- Video queue synchronization
- Chat functionality between viewers
- Custom room names
