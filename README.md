# MetaMask Vault Finder v1.23

![MetaMask Vault Finder](https://github.com/0xLuigi/metamask-vault-finder/blob/main/images/screenshot.jpg)

A powerful web-based tool designed to help MetaMask users find and analyze vault data from various file types, with intelligent search capabilities and vault reconstruction features.

## 🚀 Features

### File Processing
- **Drag & Drop Interface** - Easy file upload with visual feedback
- **Snappy Decompression** - Decompress Firefox session files and other compressed formats
- **Smart File Analysis** - Automatically detects and processes various file types
- **Large File Support** - Optimized for handling large files with progress indicators

### Intelligent Search
- **Keyword-Based Search** - Pre-configured with MetaMask-specific keywords
- **Customizable Keywords** - Add or remove search terms as needed
- **Flexible Matching** - Configure minimum keyword match requirements
- **Real-time Results** - Instant search results with highlighted matches

### Vault Data Management
- **Data Compiler** - Manually reconstruct MetaMask vault data
- **Field Validation** - Automatic validation of IV and salt fields
- **Quick Templates** - Pre-configured keyMetadata for different MetaMask versions
- **Export Options** - Copy to clipboard or save as text file

### Vault Decryption
- **Password-based Decryption** - Decrypt vault data using your MetaMask password
- **Multiple Keyring Support** - Handle HD wallets, simple key pairs, and Snap keyrings
- **Address Generation** - Automatically generate Ethereum addresses from private keys
- **Security Warnings** - Built-in reminders about private key security

## 🛠️ Technical Stack

- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Styling**: Custom CSS with modern design patterns
- **Crypto**: Web Crypto API, ethers.js for Ethereum functionality
- **File Processing**: FileReader API, custom Snappy decompression

## 📋 Prerequisites

- Modern web browser with JavaScript enabled
- Files containing potential MetaMask vault data
- MetaMask password (for decryption features)

## 🚀 Getting Started

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/metamask-vault-finder.git
cd metamask-vault-finder
```

2. Open `index.html` in your web browser or serve it through a local web server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server
```

3. Navigate to `http://localhost:8000` in your browser

### Usage

#### 1. File Upload
- Drag and drop your file onto the upload area, or click to browse
- Supported file types include text files, browser data, and compressed files
- For compressed files, use the Snappy Decompression feature (Alt+A shortcut available)

#### 2. Configure Search
- Review and modify search keywords as needed
- Set minimum keyword match count (default: 4)
- Click "Search Vault Data" to analyze the file

#### 3. Analyze Results
- View found data with highlighted keywords
- Click "View full file" to examine complete file content
- Use the find function to locate specific text within files

#### 4. Compile Vault Data
- Fill in the vault data fields (data, iv, keyMetadata, salt)
- Use quick buttons for common keyMetadata configurations
- Copy or save the compiled JSON

#### 5. Decrypt Vault (Optional)
- Paste your vault JSON data
- Enter your MetaMask password
- View decrypted wallet information including seed phrases and private keys

## 🔍 Default Search Keywords

The tool searches for these MetaMask-related terms by default:
- `{` - JSON structure indicators
- `data` - Encrypted vault data
- `iv` - Initialization vector
- `keyMetadata` - Encryption metadata
- `PBKDF2` - Key derivation algorithm
- `params` - Algorithm parameters
- `iterations` - PBKDF2 iterations
- `salt` - Cryptographic salt

## ⚠️ Security Considerations

- **Private Key Safety**: Never share your private keys or seed phrases
- **Local Processing**: All operations are performed locally in your browser
- **No Data Transmission**: No vault data or passwords are sent to external servers
- **Temporary Storage**: Decrypted data is only stored temporarily in browser memory

## 🔧 Configuration Options

### KeyMetadata Templates
- **New MetaMask (600,000 iterations)**: For recent MetaMask versions
- **Old MetaMask (10,000 iterations)**: For older MetaMask versions
- **Custom**: Manual entry for specific configurations

### Field Validation
- **IV**: Must be 24 base64 characters
- **Salt**: Must be 44 base64 characters
- **Data**: Encrypted vault data (variable length)

## 📁 Project Structure

```
metamask-vault-finder/
├── index.html          # Main application file
├── styles.css          # Application styles
├── js/
│   ├── ethers.umd.min.js    # Ethereum library
│   └── crypto-js.min.js     # Cryptographic functions
├── images/
│   ├── icon.ico        # Application icon
│   └── Luigi.png       # Author avatar
└── sounds/
    └── uspech.mp3      # Success notification sound
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Guidelines
- Follow existing code style and structure
- Test thoroughly with various file types
- Ensure security best practices are maintained
- Update documentation for new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

Created with ❤️ for the MetaMask Community by **Luigi**

- **MetaMask Community**: [MetaMask Guides](https://community.metamask.io/g/Guides)
- **Profile**: [Luigi on MetaMask Community](https://community.metamask.io/u/luigi/summary)
- **Telegram**: [@Luigi_SK](https://t.me/Luigi_SK)

## 💰 Support

If you found this tool helpful, consider supporting the development:

**Ethereum (ETH/ERC-20)**:
```
0x8A00f43C099bEB3F5d3C289e8b93c71c32B4d52e
```

**Bitcoin (BTC)**:
```
bc1qgug43r48cceja46j9nmj686wps5vad8appytsh
```

**Dogecoin (DOGE)**:
```
DH5CjTzDPmrSgPqiKnpKurUmeVvU7w5C5P
```

## 📋 Changelog

### Version 1.23
- Enhanced Snappy decompression functionality
- Improved file processing with progress indicators
- Added keyboard shortcuts (Alt+A for Snappy decompression)
- Enhanced vault decryption with multiple keyring support
- Improved UI with better error handling and validation

## ⚠️ Disclaimer

This tool is provided as-is for educational and recovery purposes. Always keep your MetaMask data secure and backed up. The author is not responsible for any loss of funds or data. For critical recovery operations, consider using the official [MetaMask Vault Decryptor](https://github.com/MetaMask/vault-decryptor).

## 🔗 Related Projects

- [MetaMask Vault Decryptor](https://github.com/MetaMask/vault-decryptor) - Official MetaMask vault decryption tool
- [MetaMask Extension](https://github.com/MetaMask/metamask-extension) - MetaMask browser extension

---

**Note**: This is an independent community project and is not officially affiliated with MetaMask or ConsenSys.
