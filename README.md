# Whisper

> **Confidential messaging platform powered by Zama FHEVM**

Whisper enables private message communication using Zama's Fully Homomorphic Encryption Virtual Machine. Your messages remain encrypted during transmission, storage, and processing—complete privacy protection.

---

## The Communication Privacy Problem

Traditional messaging platforms decrypt your messages for processing, exposing sensitive content to the system.

**Whisper solves this** by processing encrypted messages directly using Zama FHEVM, ensuring your communications stay private at all times.

---

## Zama FHEVM for Private Messaging

### Why FHE Matters in Messaging

**FHEVM** (Fully Homomorphic Encryption Virtual Machine) enables message processing, routing, and delivery while your content remains encrypted. No decryption required.

### How Whisper Protects Messages

```
┌──────────────┐
│ User Message │
│ Input        │
└──────┬───────┘
       │
       ▼ FHE Encryption
┌──────────────┐
│ Encrypted    │
│ Message      │
└──────┬───────┘
       │
       ▼
┌──────────────────────┐
│  FHEVM Message       │
│  Contract            │
│  (Whisper)           │
│  ┌──────────────┐    │
│  │ Route        │    │ ← Encrypted routing
│  │ Encrypted    │    │
│  │ Message      │    │
│  │ Deliver      │    │
│  └──────────────┘    │
└──────┬───────────────┘
       │
       ▼
┌──────────────────────┐
│ Zama FHE Runtime     │
│ Message Processing   │
│ & Routing            │
└──────┬───────────────┘
       │
       ▼
┌──────────────┐
│ Encrypted    │
│ Delivery     │
│ (Only        │
│  recipient   │
│  can decrypt)│
└──────────────┘
```

### Core Privacy Features

- 🔐 **End-to-End Encryption**: Messages encrypted with FHE before sending
- 🔒 **Processing Privacy**: Message routing without decryption
- ✅ **Storage Security**: Encrypted message storage on blockchain
- 🌐 **Decentralized**: No single point of message interception

---

## Quick Start

```bash
# Clone repository
git clone https://github.com/flowersonthefloor/Whisper
cd Whisper

# Install dependencies
npm install

# Setup environment
cp .env.example .env.local
# Configure your settings

# Deploy contracts
npm run deploy:sepolia

# Start application
npm run dev
```

**Requirements**: MetaMask, Sepolia ETH, Node.js 18+

---

## How Private Messaging Works

### Message Flow

1. **Encrypt Message**: Your message encrypted with FHE before sending
2. **Submit Encrypted**: Encrypted message submitted to blockchain
3. **FHEVM Routing**: Smart contract routes message without decryption
4. **Encrypted Storage**: Message stored encrypted on blockchain
5. **Private Delivery**: Only recipient can decrypt message
6. **Verifiable**: Message delivery verifiable without revealing content

### Privacy Comparison

| Aspect | Traditional Messaging | Whisper |
|-------|---------------------|---------|
| **Transmission** | Encrypted in transit | Encrypted at all stages |
| **Storage** | Plaintext on servers | Encrypted on blockchain |
| **Processing** | Decrypted for routing | Encrypted routing |
| **Access** | Server can read | Only recipient reads |
| **Audit** | Centralized logs | Transparent blockchain |

---

## Technology Architecture

### Core Stack

| Component | Technology | Purpose |
|-----------|-----------|---------|
| **Encryption** | Zama FHE | Fully homomorphic encryption |
| **Blockchain** | Ethereum Sepolia | Decentralized message storage |
| **Smart Contracts** | Solidity + FHEVM | Encrypted message routing |
| **Frontend** | React + TypeScript | Messaging interface |
| **Build Tool** | Hardhat | Development environment |

### Zama FHEVM Integration

- **Message Encryption**: FHE encryption before sending
- **Encrypted Routing**: Route messages without decryption
- **Privacy-Preserving**: No message content visibility
- **Verifiable Delivery**: Transparent delivery confirmation

---

## Use Cases

### Private Communication

- Confidential business messaging
- Secure personal communication
- Private team collaboration
- Encrypted group chats

### Professional Privacy

- Secure client communication
- Confidential document sharing
- Private business discussions
- Encrypted professional networking

### Personal Privacy

- Private family messaging
- Secure personal notes
- Confidential diary entries
- Encrypted personal communication

---

## Development

### Building

```bash
npm run build:contracts    # Build smart contracts
npm run build:frontend     # Build frontend
npm run build              # Build all components
```

### Testing

```bash
npm test                   # Run all tests
npm run test:contracts     # Contract tests only
npm run test:frontend      # Frontend tests only
```

### Deployment

```bash
npm run deploy:sepolia     # Deploy to Sepolia testnet
npm run deploy:local       # Deploy to local network
```

---

## Security & Privacy

### Privacy Guarantees

- 🔐 **Message Content**: Always encrypted, never decrypted by system
- 🔒 **Metadata Protection**: Minimal metadata exposure
- ✅ **Delivery Verification**: Verifiable without revealing content
- 🌐 **Decentralized Storage**: No centralized message storage

### Security Features

- **FHE Encryption**: Military-grade encryption for all messages
- **Zero-Knowledge Routing**: Message routing without content access
- **Blockchain Immutability**: Messages cannot be altered
- **Transparent Audit**: Message delivery logs without content

### Best Practices

- 🔒 Use Sepolia testnet for development
- 🔒 Never commit private keys
- 🔒 Verify contract addresses before sending
- 🔒 Use hardware wallets for production
- 🔒 Understand gas costs for FHE operations

---

## Contributing

Contributions welcome! Priority areas:

- 🔬 FHE performance optimization for messaging
- 🛡️ Security audits for communication protocols
- 📖 Documentation improvements
- 🎨 UI/UX for messaging interface
- 🌐 Internationalization

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## Resources

- **Zama**: [zama.ai](https://www.zama.ai/)
- **FHEVM Documentation**: [docs.zama.ai/fhevm](https://docs.zama.ai/fhevm)
- **Ethereum Sepolia**: [sepolia.etherscan.io](https://sepolia.etherscan.io/)

---

## License

MIT License - See [LICENSE](LICENSE) file for details.

---

## Acknowledgments

Built with [Zama FHEVM](https://github.com/zama-ai/fhevm) - Privacy-preserving messaging on blockchain.

---

**Repository**: https://github.com/flowersonthefloor/Whisper  
**Issues**: https://github.com/flowersonthefloor/Whisper/issues  
**Discussions**: https://github.com/flowersonthefloor/Whisper/discussions

---

_Powered by Zama FHEVM | Private Messages | Decentralized Communication_
