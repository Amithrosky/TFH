# TFH (Temporary File Holder) v2.1

A lightweight, secure, and ephemeral file-sharing utility designed for browser-based transient data management.

## 🚀 Features

- **30-Minute Self-Destruct**: Automatically purges uploaded files after 30 minutes of retention.
- **P2P Direct Share**: Leverages WebRTC for direct peer-to-peer file transfers, ensuring files never touch a central server.
- **Browser Storage Integration**: Employs IndexedDB (`C:/TFH/Temp_files/` virtual path) for local temporary holding.
- **Real-Time Terminal Log**: Built-in system console for live monitoring of network events and storage states.
- **Client-Side Encryption**: Ensures transient files remain protected during the holding period.

## ⚡ Quick Start

1. **Access**: Visit TFH (https://amithrosky.github.io/TFH/)
2. **Hold or Share**:
   - **Virtual Hold**: Drag and drop files to hold them in browser memory for up to 30 minutes.
   - **P2P Share**: Generate a direct WebRTC connection link to transfer files directly to another device.
3. **Purge**: Clear all active holding files instantly using the manual system wipe option.

## 🔒 Security & Retention Protocol

| Component | Implementation Details |
| :--- | :--- |
| **Retention Limit** | 30 Minutes (Automated purge protocol) |
| **Storage Engine** | Browser IndexedDB (Client-side virtual node) |
| **P2P Engine** | WebRTC DataChannels (No server-side storage) |

> **Note**: For WebRTC P2P transfers, ensure the host browser tab remains open until the receiving peer completes the file extraction.

---

Developed by [Amith Rosky](https://github.com/amithrosky).
