# Zion: Blockchain-Based Resume IP Marketplace

![Zion Logo](https://github.com/team-zion/.github/blob/main/assets/logo.png?raw=true)

## 📖 Description

Zion is a blockchain-powered marketplace that transforms text-based intellectual property, specifically resumes and cover letters, into valuable digital assets while preserving privacy and ensuring fair compensation for original creators.

### Integration with Story Protocol

Zion leverages Story Protocol to register cover letters as IP assets with unique identifiers (DIDs/CIDs) on the blockchain. When a user's resume is utilized by AI to help another user create a new cover letter, the original author receives compensation through Story Protocol's automated reward system. The integration includes:

- **IP Asset Registration**: Converting text documents into blockchain assets
- **License Management**: Establishing usage rights for registered documents
- **Royalty Distribution**: Automating payments to original authors when their work is referenced

### About Team Zion

We are Team Zion, named after a sanctuary for humanity. Our team also operates RocketPunch, a Web 2.0-based business networking platform with over 600,000 users. This background has fueled our interest in discovering real-world use cases for blockchain technology that create tangible impact in professional settings.

While many solutions in the Story Protocol ecosystem focus on tokenizing visual creative works like images, characters, and videos, we identified an untapped opportunity in text-based IP containing valuable personal information. Zion enables the monetization of content that users cannot publicly share but holds significant value when utilized securely by AI systems.

## 🐤 Demo

- [View Demo Video](https://youtu.be/dn4ji28ofEE)
- [View Presentation Slides](https://github.com/team-zion/.github/blob/main/assets/Zion%20Revolutionizing%20Text%20IP%20Management%20with%20Story%20Protocol.pdf)

## ⭐ Main Features

### Resume & Cover Letter IP Registration
- Upload and register your resume/cover letter as a blockchain asset
- Securely store your document with privacy protection
- Maintain ownership rights through Story Protocol's IP registry

### AI-Powered Cover Letter Generation
- Create personalized cover letters tailored to specific job applications
- Leverage AI to improve writing quality and match job descriptions
- Reference high-quality registered documents for better results

### Transparent Reward System
- Track when your documents are referenced by others
- Automatically receive compensation based on contribution value
- View detailed usage history of your intellectual property

## 🔧 Tech Stack

### Frontend & Backend
- **Next.js**: Full-stack React framework for server-side rendering and API routes
- **TypeScript**: Strongly typed programming language that builds on JavaScript
- **Python**: Backend language for AI and data processing

### Authentication & Wallet
- **Auth.js**: User authentication and session management
- **Privy SDK**: Seamless wallet creation and management for blockchain interactions

### Blockchain Integration
- **Story Protocol SDK**: IP registry, licensing, and royalty distribution
- **EVM (Ethereum Virtual Machine)**: Execution environment for smart contracts

### Data Storage
- **PostgreSQL**: Primary database for user accounts and document metadata
- **Pinecone Vector DB**: Vector database for text similarity search and semantic matching
- **Vercel Storage**: Document file storage for PDFs and associated files

### AI & Natural Language Processing
- **Claude API**: AI model for text analysis and generation of cover letters
- **RAG Agent**: Retrieval-Augmented Generation system that combines document retrieval with AI generation for context-aware cover letter creation

## 📊 Architecture Overview

Our architecture consists of three main components that work together to create a seamless experience:

### Upload Flow
- Users upload cover letters via the Next.js frontend
- Privy SDK creates and manages user wallets
- Documents are stored in Vercel Storage
- Metadata is saved in PostgreSQL
- Story Protocol registers the IP on-chain

### Generation Flow
- User requests a cover letter generation
- The system extracts data from registered IPs using Pinecone Vector DB
- Claude API generates personalized content
- Story Protocol tracks usage and distributes rewards
- The new document is saved and registered as a derivative work

## 📂 Component Breakdown

### 1. Application
The user-facing frontend/backend that handles cover letter management and creation.

**Key Features**
- **Resume Upload**: Users can register their existing resumes
- **Create Resume**: Users can initiate personalized cover letter generation using AI
- **Dashboard**: Track uploaded documents and earned rewards

### 2. Story Protocol (Web3 Layer)
Handles on-chain IP registration of cover letters and reward distribution whenever a cover letter is referenced or reused.

**Key Features**
- **IP Registration**: Cover letters are registered as IP using DIDs/CIDs or NFTs
- **Usage Tracking**: Each instance of resume reuse is recorded
- **Reward Distribution**: Automatic tokenized rewards for original authors

### 3. AI Agent
Uses IP-registered resumes to generate tailored cover letters based on job context and user background.

**Key Features**
- **Cover letter Analysis**: Extracts experience, skills, and structure from the IP cover letter
- **Context-Aware Generation**: Combines resume data with job description to create a personalized cover letter
- **Usage Reporting**: Logs which IP assets were used and notifies Story Protocol for reward processing



## 💬 Feedback on Building with Story Protocol

Integrating with Story Protocol was generally a positive experience that enabled us to build a robust IP management system. The modular approach of separating IP assets, licensing, and royalty functions provided flexibility in implementation.

However, we encountered a challenge during the process of registering derivatives. The documentation and sample code omitted the critical step of transferring License Token authorization to Story's smart contract, which made issue tracing difficult when problems arose. We resolved this by implementing the authorization transfer functionality ourselves.

Despite this hurdle, Story Protocol's approach to IP management aligns perfectly with our vision for text-based asset monetization, and we're excited to continue building on this foundation.

## 👨‍💻 Role & Contribution

Our cross-functional team leveraged diverse expertise to bring Zion to life:

### Product & Design
- Product strategy and market research
- UX/UI design for seamless user experience

### Frontend Development
- Next.js application development
- Integration with Privy for wallet management

### Blockchain Integration
- Story Protocol SDK implementation
- Smart contract interaction and testing

### AI & Backend Development
- Claude API integration for cover letter generation
- Vector database setup for text similarity
- Auth.js implementation for secure authentication

## 📌 Future Roadmap

- **Private Document Sharing**: Enhanced privacy features for selective sharing
- **Expansion of use cases**: Creation of investment portfolio documents
- **Cover Letter Templates**: Pre-designed templates optimized for different industries
- **Advanced Analytics**: Insights into document performance and usage
- **Expanded IP Types**: Support for additional text-based IP beyond resumes
- **Mobile Application**: Native mobile experience for on-the-go users

---

Made with ❤️ by Team Zion | [GitHub](https://github.com/team-zion)
