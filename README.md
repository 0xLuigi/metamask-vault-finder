# 🦊 MetaMask Vault Finder v1.23

![MetaMask Vault Finder](https://github.com/0xLuigi/metamask-vault-finder/blob/main/images/screenshot.jpg)

A powerful web-based tool designed to help MetaMask users find and analyze vault data from various file types, with intelligent search capabilities and vault reconstruction features.

## 🚀 Features

### File Processing
- **Drag & Drop Interface** - Easy file upload with visual feedback
- **Snappy Decompression** - Decompress Firefox session files 
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

## 🛠️ Technical Stack

- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Styling**: Custom CSS with modern design patterns
- **Crypto**: Web Crypto API, ethers.js for Ethereum functionality
- **File Processing**: FileReader API, custom Snappy decompression

## 📋 Prerequisites

- Modern web browser with JavaScript enabled
- Files containing potential MetaMask vault data
- MetaMask password (for decryption features)

### Usage

#### 1. File Upload
- Drag and drop your file onto the upload area, or click to browse
- Supported file types include text files, browser data, and compressed files
- For compressed Firefox files, use the Snappy Decompression feature (Alt+A shortcut available)

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

## ⚠️ Security Considerations

- **Private Key Safety**: Never share your private keys or seed phrases
- **Local Processing**: All operations are performed locally in your browser
- **No Data Transmission**: No vault data or passwords are sent to external servers
- **Temporary Storage**: Decrypted data is only stored temporarily in browser memory

## 📁 Project Structure

```
metamask-vault-finder/
├── index.html          # Main application file
├── styles.css          # Application styles
├── js/
│   ├── ethers.umd.min.js    # Ethereum library
│   ├── crypto-js.min.js     # Cryptographic functions
│   └── vault-decryptor.js   # Vault decryptor logic
├── images/
│   ├── icon.ico        # Application icon
│   └── Luigi.png       # Author avatar
│   └── screenshot.jpg  # Application screenshot
├── sounds/
│   └── uspech.mp3      # Decompression success notification sound
└── 42                  # The answer to the ultimate question of life, the universe, and everything :D
```
## 📄 Test File
- The project includes a sample Firefox MetaMask wallet file named `42` that you can use to test the functionality of the tool.
- On file 42, you can try Snappy decompression 🗜️. 
- The password for file 42 is: MetaMask

## 👨‍💻 Author

Created with ❤️ for the MetaMask Community by **Luigi**

- **Profile**: [Luigi on MetaMask Community](https://community.metamask.io/u/luigi/summary)
- **Telegram**: [@Luigi_SK](https://t.me/Luigi_SK)

## 💖 Support the Project

If this tool helped you fix your MetaMask wallet, consider supporting the development:

- **Bitcoin (BTC):** `bc1qgug43r48cceja46j9nmj686wps5vad8appytsh`
- **Ethereum (ETH):** `0x8A00f43C099bEB3F5d3C289e8b93c71c32B4d52e`   
