# Valentine Encoder

> Transform your messages into a thousand "I love yous" – because plain text is so last century.

A creative web application that encodes your messages using the phrase "I LOVE YOU" in various capitalizations. Every letter becomes a love note, making your chats more romantic this Valentine's Day.

## ✨ Features

- **🎨 Love-ify Messages**: Convert any text into encoded "I love you" patterns
- **🔓 De-Love-ify**: Decode messages back to their original form
- **🔗 Shareable Links**: Generate compressed shareable links with automatic URL shortening
- **💾 Persistent Storage**: Messages are stored locally so you can decode them anytime
- **📱 Responsive Design**: Beautiful, romantic UI that works on all devices
- **🎭 Privacy-Focused**: All encoding happens in your browser, no server required

## 🚀 Demo

Visit the live application: [Valentine Encoder](https://valentine-encoder.vercel.app/)

## 📖 How It Works

The Valentine Encoder uses a clever binary encoding scheme:

1. **Text to Binary**: Each character is converted to its 8-bit binary representation
2. **Binary to "I LOVE YOU"**: Each bit is mapped to a letter from "I LOVE YOU"
   - `0` = Uppercase letter
   - `1` = Lowercase letter
3. **Formatting**: The 8 letters are formatted as: `I LOVE YOU` (1-4-3 pattern)

### Example

**Original**: `Hi`

**Encoded**:
```
I LOVe yoU
i lOVE You
```

Each line represents one character, with the capitalization pattern encoding the binary value.

## 🎯 Usage

### Encoding a Message

1. Click on the **"Love-ify"** tab
2. Type your message in the "Your Message" textarea
3. The encoded version appears automatically in "Love-ified Output"
4. Click **"Share"** to generate a shareable link

### Decoding a Message

1. Click on the **"De-Love-ify"** tab
2. Paste the encoded message in the input field
3. The original message appears automatically

### Sharing Messages

1. After encoding a message, click the **"Share"** button
2. The app generates a compressed link with TinyURL
3. Share the link with anyone – when they open it, they'll see the decoded message

## 🛠️ Technologies Used

- **HTML5** - Structure and semantics
- **CSS3** - Custom styling with CSS variables and animations
- **Tailwind CSS** - Utility-first CSS framework
- **Vanilla JavaScript** - Core functionality and logic
- **LZ-String** - Compression for shareable links
- **LocalStorage API** - Client-side data persistence
- **TinyURL API** - URL shortening for cleaner sharing

## 🎨 Design Features

- Beautiful gradient backgrounds with Valentine's theme
- Custom fonts: Crimson Pro (serif) and Outfit (sans-serif)
- Smooth animations and transitions
- Heartbeat animation for the heart icon
- Glass morphism effects
- Responsive design for mobile, tablet, and desktop

## 💻 Installation

No installation required! Simply open the HTML file in a modern web browser.

For local development:

```bash
# Clone the repository
git clone https://github.com/tariqulislamrahat/Valentine-Encoder.git

# Navigate to the project directory
cd Valentine-Encoder

# Open in your browser
# Just open index.html or serve with any static server
```

Or use a simple HTTP server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server package)
npx http-server

# Then visit http://localhost:8000
```

## 📁 Project Structure

```
Valentine-Encoder/
│
├── index.html          # Main application file (all-in-one)
├── README.md           # This file
└── LICENSE             # License file (if applicable)
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for Contributions

- Add more encoding schemes (different phrases, emojis)
- Implement dark mode
- Add sound effects
- Create mobile app versions
- Add social media preview cards
- Implement copy-to-clipboard functionality
- Add more Valentine's themes

## 🎓 Credits

This project was brought to life by a collaborative effort:

- **[Tariqul Islam Rahat](https://github.com/tariqulislamrahat)** - Idea & Concept
- **[Grok](https://grok.com/)** - Coding Implementation
- **[Claude Sonnet 4.5](https://claude.ai)** - UI Design

## 📝 Technical Details

### Encoding Algorithm

```javascript
// Character → Binary (8 bits)
"H" → 01001000

// Binary → "I LOVE YOU" pattern
0 1 0 0 1 0 0 0
I L O V E Y O U

// Apply capitalization (0=uppercase, 1=lowercase)
I lOVe yoU
```

### Storage Format

Messages are stored using a short ID system:
- First 2 chars: Initials from the message
- Next 2 chars: Message length (padded)
- Last 2 chars: Hash-based checksum

This allows efficient storage and retrieval of encoded/decoded pairs.

## 🔒 Privacy & Security

- All encoding/decoding happens **client-side**
- No data is sent to any server (except URL shortening)
- Messages are stored in your browser's LocalStorage
- Shareable links contain the encoded message in compressed form

## 🌟 Browser Compatibility

- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Opera 76+

Requires a modern browser with ES6+ support.

## 📄 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 💖 Support

If you like this project, please consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs
- 💡 Suggesting new features
- 🔀 Submitting pull requests

## 📬 Contact

Tariqul Islam Rahat - [@tariqulislamrahat](https://github.com/tariqulislamrahat)

Project Link: [https://github.com/tariqulislamrahat/Valentine-Encoder](https://github.com/tariqulislamrahat/Valentine-Encoder)

---

<div align="center">

**Made with ♥ for Valentine's Day 2026**

*Who needs plain text when your messages can say 'I love you' a thousand times?*

</div>
