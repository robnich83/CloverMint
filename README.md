# 🎟️ NFT Ticket Collectible DApp

## Overview
This project introduces a blockchain-based event ticketing system where tickets are issued as **Semi-Fungible Tokens (SFTs)** for easy sale and distribution — and later **converted into collectible NFTs** after the event concludes.  

This solves two major issues in the live events industry:
1. **Ticket Scalping / Price Inflation** — by restricting resale prices before the event.
2. **Lost Value After Events** — by turning used tickets into collectible NFTs with future rewards.

---

## 🔑 Core Features

### 1. Pre-Event (SFT Tickets)
- Event tickets are minted as ERC-1155 SFTs.
- Can be sold or transferred only within approved price limits.
- Acts as proof of purchase for entry.

### 2. Event Access
- Wallet or QR-based entry validation.
- Ticket marked as “used” on-chain once scanned.

### 3. Post-Event (NFT Collectible)
- Each used SFT converts into a **unique ERC-721 NFT**.
- Metadata updated with event artwork, details, and rewards.
- NFT acts as a digital collectible or proof of attendance.

---

## 🧠 Smart Contract Logic

Contract: EventTicketManager

mintTicketSFT(eventId, seatType, price, buyer)
-> Mints SFT (ERC-1155)
-> Restricts resale price

validateTicket(eventId, tokenId)
-> Marks ticket as used (on-chain)

convertToNFT(eventId)
-> Converts used SFTs into unique ERC-721 NFTs
-> Adds collectible metadata + rewards


---

## ⚙️ Tech Stack

| Layer | Tools |
|-------|-------|
| Blockchain | Ethereum / Polygon / Base |
| Smart Contracts | Solidity (ERC-1155 + ERC-721) |
| Frontend | React + Ethers.js |
| Storage | IPFS / Pinata |
| Wallet | MetaMask / Coinbase Wallet |

---

## 💰 Benefits
- Eliminates ticket scalping
- Enhances fan engagement via collectibles
- Opens new monetization for artists & organizers
- Establishes transparent resale markets

---

## 🧩 Future Add-ons
- Loyalty tiers based on owned NFTs  
- Token-gated early access for superfans  
- NFT-based voting for event experiences  

---

## 📄 License
MIT License


