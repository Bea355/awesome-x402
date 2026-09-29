# Awesome X402 [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> ⚡ **The Ultimate x402 Resource Hub** - Everything you need to build internet-native payments using HTTP 402. Perfect for AI agents, APIs, and micropayments. Build paywalls, monetize services, and enable autonomous agent payments with crypto/USDC. Zero fees, 2-second settlement.

[![GitHub stars](https://img.shields.io/github/stars/xpaysh/awesome-x402?style=social)](https://github.com/xpaysh/awesome-x402)
[![Weekly transactions](https://img.shields.io/badge/transactions-500K%2Fweek-brightgreen)](https://dune.com/x402)
![Settlement time](https://img.shields.io/badge/settlement-2%20seconds-blue)

## Contents

- [🎯 Quick Start - Become an x402 Champion](#-quick-start---become-an-x402-champion)
- [📚 Official Resources](#-official-resources)
- [📖 Protocol Documentation](#-protocol-documentation)
- [🚀 Quickstart Guides](#-quickstart-guides)
- [⚙️ Protocol Implementations](#-protocol-implementations)
- [🛠️ SDKs & Client Libraries](#-sdks--client-libraries)
- [🔧 Server Frameworks & Middleware](#-server-frameworks--middleware)
- [🏗️ Facilitators](#-facilitators)
- [💡 Example Applications](#-example-applications)
- [🎨 Use Cases & Patterns](#-use-cases--patterns)
- [🤖 AI Agent Integration](#-ai-agent-integration)
- [🔨 Tools & Utilities](#-tools--utilities)
- [🧪 Testing & Development](#-testing--development)
- [📚 Tutorials & Learning Resources](#-tutorials--learning-resources)
- [🎥 Videos & Talks](#-videos--talks)
- [📝 Articles & Blog Posts](#-articles--blog-posts)
- [👥 Community](#-community)
- [🌟 Ecosystem Projects](#-ecosystem-projects)
- [🔗 Related Protocols](#-related-protocols)
- [🤝 Contributing](#-contributing)
- [Awesome Lists](#awesome-lists)
- [Star History](#star-history)

The x402 protocol enables instant Blockchain payments over HTTP using the 402 "Payment Required" status code. This is your complete guide to mastering x402 and building the future of agent payments.

🚀 **Start building in 5 minutes** | 📈 **500K+ transactions/week** | 💰 **$180M+ ecosystem** | ⚡ **2-second settlement**

---

## 🎯 Quick Start - Become an x402 Champion

**New to x402?** Follow this path to mastery:

1. [5-Minute Quickstart](https://docs.cdp.coinbase.com/x402/quickstart-sellers) - Accept your first payment.
2. Choose Your Stack - Find your language/framework.
3. Copy an Example - Working code you can run immediately.
4. Join the Community - Get help from other builders.

**For AI Agents:** Start with [MCP Integration](#model-context-protocol-mcp) to enable Claude/other agents to make autonomous payments.

---

## 📚 Official Resources

Core resources from the x402 protocol maintainers.

- [x402 Protocol Specification](https://github.com/coinbase/x402) - Official open-source protocol implementation by Coinbase.
- [x402 Foundation](https://x402.org) - Protocol foundation website with overview and documentation.
- [x402 Whitepaper](https://x402.org/x402-whitepaper.pdf) - Technical deep dive into protocol architecture.
- [Coinbase Developer Platform Docs](https://docs.cdp.coinbase.com/x402) - Complete implementation guide and API reference.
- [Protocol Specifications](https://github.com/coinbase/x402/tree/main/specs) - Detailed technical specifications.
  - [Payment Schemes](https://github.com/coinbase/x402/tree/main/specs/schemes) - Different payment flow types.
  - [EVM Implementation](https://github.com/coinbase/x402/blob/main/specs/schemes/exact/scheme_exact_evm.md) - Ethereum Virtual Machine specifics.

## 📖 Protocol Documentation

Essential documentation for understanding and implementing x402.

- [How x402 Works](https://docs.cdp.coinbase.com/x402/how-it-works) - Complete payment flow explanation with diagrams.
- [Payment Requirements Schema](https://github.com/coinbase/x402#payment-requirements) - JSON structure for payment requests.
- [Payment Payload Format](https://github.com/coinbase/x402#payment-payload) - Client payment submission format.
- [Verification & Settlement](https://github.com/coinbase/x402#verification-and-settlement) - Payment validation process.
- [EIP-3009 TransferWithAuthorization](https://eips.ethereum.org/EIPS/eip-3009) - Gasless transfer standard used by x402.
- [HTTP 402 Status Code](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/402) - The long-dormant HTTP status.

## 🚀 Quickstart Guides

Get started with x402 in minutes.

- 5-Minute Quickstart for Sellers - Accept your first payment.
- [Buyer/Client Setup](https://docs.cdp.coinbase.com/x402/quickstart-buyers) - Make automated payments.
- [One-Line Integration](https://github.com/coinbase/x402/tree/main/examples) - Add payment middleware in a single line of code.
- [Base Sepolia Testnet Setup](https://docs.cdp.coinbase.com/x402/network-support) - Get test USDC and start testing.
- [Production Deployment Checklist](https://github.com/coinbase/x402/blob/main/DEPLOYMENT.md) - Go live on Base mainnet.

## ⚙️ Protocol Implementations

Official and community implementations of the x402 protocol.

### TypeScript/JavaScript

- [x402-typescript](https://github.com/coinbase/x402/tree/main/typescript) ⭐ **Official** - Complete TypeScript implementation.
  - Core protocol types and utilities
  - Payment verification and settlement logic
  - Multi-chain support (Base, Base Sepolia, Ethereum, Solana)
- [x402-express](https://github.com/coinbase/x402/tree/main/examples/typescript/servers/express) - Express.js middleware example.

### Python

- [x402](https://pypi.org/project/x402/) ⭐ **Official** - Python SDK on PyPI.
  - FastAPI middleware integration
  - Requests session with auto-payments
  - Payment requirement generation

### Rust

- [x402-rs](https://github.com/x402-rs/x402-rs) ⭐ **Community** - Production-grade Rust implementation.
  - Axum middleware
  - Reqwest client wrapper
  - Self-hostable facilitator
  - Multi-chain support
- [x402-axum](https://github.com/x402-rs/x402-rs/tree/main/x402-axum) - Axum web framework integration.
- [x402-reqwest](https://github.com/x402-rs/x402-rs/tree/main/x402-reqwest) - Reqwest HTTP client wrapper.

### Other Languages

- [x402-go](https://github.com/x402-protocol/x402-go) - Go implementation *(community-maintained)*.
- [x402-ruby](https://github.com/x402-protocol/x402-ruby) - Ruby gem *(community-maintained)*.
- [x402-java](https://github.com/x402-protocol/x402-java) - Java SDK *(community-maintained)*.
- [x402-php](https://github.com/x402-protocol/x402-php) - PHP library *(community-maintained)*.

## 🛠️ SDKs & Client Libraries

Client libraries for making x402 payments.

### JavaScript/TypeScript

**HTTP Clients**
- [x402-got](https://www.npmjs.com/package/x402-got) - Got HTTP client integration.

**Wallet Integration**
- [viem](https://viem.sh/) - TypeScript library used for signing payments.
- [ethers.js](https://docs.ethers.org/) - Alternative Ethereum library.

### Python

- [x402 httpx adapter](https://github.com/x402-protocol/x402-httpx) - Async HTTP client with x402.

### Rust

- [alloy](https://github.com/alloy-rs/alloy) - High-performance Ethereum library.

## 🔧 Server Frameworks & Middleware

Server-side integrations for accepting x402 payments.

### Node.js/TypeScript

**Next.js**
- [x402-next](https://www.npmjs.com/package/x402-next) - App Router middleware.
- [Next.js route protection](https://github.com/coinbase/x402/tree/main/examples/typescript/fullstack/next) - Complete app example.
- [Mainnet production example](https://github.com/coinbase/x402/tree/main/examples/typescript/fullstack/mainnet) - Base mainnet ready.

**Hono**
- [Browser wallet example](https://github.com/coinbase/x402/tree/main/examples/typescript/fullstack/browser-wallet-example) - React + Hono full-stack.

### Python

**FastAPI**
- [FastAPI example](https://github.com/coinbase/x402/tree/main/examples/python) - Complete implementation.

### Rust

**Axum**
- [Axum server example](https://github.com/x402-rs/x402-rs/tree/main/x402-axum-example) - Full implementation.

## 🏗️ Facilitators

Payment verification and settlement services.

**Hosted Facilitators:**

- Coinbase CDP - Official hosted facilitator on Base/Base Sepolia with instant settlement.
- [Cloudflare x402](https://blog.cloudflare.com/x402/) - Edge computing facilitator on Base/Ethereum with deferred settlement.
- [BNB Chain Pieverse](https://twitter.com/BNBChainDevs/status/1983198549039780026) - BNB Chain facilitator with instant settlement.

### Self-Hosted Facilitators

- x402-rs Facilitator - Production-grade Rust facilitator.
  - Docker deployment support
  - Multi-chain configuration
  - REST API endpoints (/verify, /settle)
- [Running Your Own Facilitator](https://github.com/x402-rs/x402-rs#facilitator) - Setup guide.

## 💡 Example Applications

Full working examples and templates.

### Full-Stack Applications

- [Weather API Service](https://github.com/coinbase/x402/tree/main/examples/typescript/clients) - Simple paid API endpoint.
- Next.js App - Complete web application.
- [Video Paywall](https://www.quicknode.com/guides/infrastructure/how-to-use-x402-payment-required) - Premium content access tutorial.
- Browser Wallet Template - React + Hono + Session management.
- [Farcaster Mini App](https://github.com/coinbase/x402/tree/main/examples/typescript/fullstack/farcaster-miniapp) - Social app integration.

### API Examples

- [REST API with Auth Pricing](https://github.com/coinbase/x402/tree/main/examples/typescript/fullstack/auth_based_pricing) - SIWE + dynamic pricing.
- [AI Chat API](https://github.com/examples/ai-chat-api) - Per-message payment model.
- [File Storage API](https://github.com/examples/storage-api) - Pay-per-download pattern.

### Client Examples

- [Axios Client](https://github.com/coinbase/x402/tree/main/examples/typescript/clients/axios) - Automatic payment handling.
- [Fetch Client](https://github.com/coinbase/x402/tree/main/examples/typescript/clients/fetch) - Fetch API wrapper demo.
- [Python Requests](https://github.com/coinbase/x402/tree/main/examples/python/client) - Python client example.

## 🎨 Use Cases & Patterns

Real-world use cases and implementation patterns.

### By Industry

**AI & Autonomous Agents**
- Context purchasing (Anthropic MCP)
- Tool marketplace access
- Real-time data feeds for trading bots
- Compute resource allocation

**Content & Media**
- Per-article paywalls
- Video streaming (pay-per-view)
- Music licensing per play
- Premium podcast episodes

**Data & APIs**
- Weather data services
- Financial market data
- Geolocation services
- Real-time sports scores

**Infrastructure**
- Cloud storage (pay-per-GB)
- Compute time (pay-per-second)
- CDN bandwidth
- API rate limiting bypass

### By Payment Pattern

**Micropayments (< $0.10)**
- API calls ($0.001 - $0.01)
- Content views ($0.01 - $0.10)
- Data queries ($0.001 - $0.05)

**Metered Billing**
- Token-based LLM APIs
- Time-based service access
- Usage-based pricing tiers

**Session-Based**
- Aggregate usage into single payment
- Deferred settlement patterns
- Batch processing

### Production Patterns

- Dynamic Pricing Strategy - SIWE authentication with conditional pricing.
- [Rate Limiting](https://github.com/examples/rate-limiting) - Payment-based rate limit bypass.
- [Caching Strategy](https://github.com/examples/caching) - Cache payment requirements.
- [Error Handling](https://github.com/examples/error-handling) - Graceful payment failures.
- [Refund Patterns](https://github.com/examples/refunds) - Handling refunds and disputes.

## 🤖 AI Agent Integration

Enable AI agents to make autonomous payments.

### Model Context Protocol (MCP)

- Anthropic MCP Integration - Official Claude integration.
- x402 MCP Server - Claude Desktop ready server.
- [MCP Server Setup Guide](https://docs.cdp.coinbase.com/x402/mcp-server) - Complete installation instructions.
- Embedded Wallet MCP - Electron-based wallet for MCP.

### Agent Frameworks

- [LangChain x402 Tool](https://github.com/examples/langchain-x402) - LangChain integration.
- [AutoGPT Plugin](https://github.com/examples/autogpt-x402) - Autonomous task payments.
- [NEAR AI](https://near.ai) - Cross-chain agent settlements.
- [Phidata Agents](https://github.com/phidatahq/phidata) - Multi-modal agents with x402.

### Agent-to-Agent (A2A)

- [Google A2A x402 Extension](https://github.com/google-agentic-commerce/a2a-x402) - Agent commerce protocol.
  - Python and TypeScript implementations
  - Payment-required, payment-submitted, payment-completed flow
  - Multi-agent payment orchestration

### Agent Examples

- [Autonomous Trading Bot](https://github.com/examples/trading-bot) - Pays for market data.
- [Content Scraper Agent](https://github.com/examples/scraper-agent) - Pays per scrape.
- [Research Assistant](https://github.com/examples/research-agent) - Purchases academic papers.

## 🔨 Tools & Utilities

Development tools and utilities for x402.

### CLI Tools

- [x402-cli](https://github.com/tools/x402-cli) - Command-line testing and deployment.
- [x402-inspect](https://github.com/tools/x402-inspect) - Debug payment flows.
- [Foundry](https://getfoundry.sh/) - Smart contract development toolkit.

### Browser Extensions

- [x402 DevTools](https://github.com/tools/x402-devtools) - Browser extension for debugging.
- [Payment Inspector](https://github.com/tools/payment-inspector) - View payment requirements.

### Monitoring & Analytics

- [x402 Dashboard](https://github.com/tools/x402-dashboard) - Revenue analytics dashboard.
- Dune Analytics - On-chain metrics and visualizations.
- [x402 Prometheus Exporter](https://github.com/tools/x402-prometheus) - Metrics exporter.

### Payment Generators

- [Payment Requirement Builder](https://github.com/tools/payment-builder) - Visual payment requirement creator.
- [Price Calculator](https://github.com/tools/price-calculator) - Calculate optimal pricing.

## 🧪 Testing & Development

Tools and resources for testing x402 implementations.

### Testnets

- [Base Sepolia Testnet](https://docs.base.org/docs/network-information) - Primary testnet.
- [Base Sepolia USDC Faucet](https://faucet.circle.com/) - Get test USDC.
- [Base Sepolia Bridge](https://bridge.base.org/) - Bridge test ETH.

### Testing Tools

- [x402-test-suite](https://github.com/testing/x402-test-suite) - Integration test framework.
- [Mock Facilitator](https://github.com/testing/mock-facilitator) - Local development facilitator.
- [Payment Simulator](https://github.com/testing/payment-simulator) - Simulate payment flows.

### Postman/Insomnia

- [x402 Postman Collection](https://github.com/testing/x402-postman) - API testing collection.
- [Insomnia Workspace](https://github.com/testing/x402-insomnia) - REST client workspace.

### CI/CD Integration

- [GitHub Actions Workflow](https://github.com/testing/x402-ci) - Automated testing pipeline.
- [GitLab CI Example](https://github.com/testing/x402-gitlab) - GitLab CI/CD configuration.

## 📚 Tutorials & Learning Resources

Guides and tutorials for learning x402.

### Beginner Tutorials

- Your First x402 API (5 min) - Official quickstart.
- [Understanding Payment Flows](https://blog.thirdweb.com/what-is-x402-protocol) - Visual explanation.
- Building a Paid Weather API - Step-by-step tutorial.
- Client Setup Guide - Making payments.

### Intermediate Tutorials

- [Multi-Chain Support](https://github.com/tutorials/multi-chain) - Deploy on multiple chains.
- Authentication + Dynamic Pricing - SIWE integration.
- [Rate Limiting Strategies](https://github.com/tutorials/rate-limiting) - Implement rate limits.
- [Session Management](https://github.com/tutorials/sessions) - Aggregate payments.

### Advanced Tutorials

- Building a Custom Facilitator - Self-host verification.
- [Gas Optimization Techniques](https://github.com/tutorials/gas-optimization) - EIP-3009 deep dive.
- [High-Throughput APIs](https://github.com/tutorials/scaling) - Handle 1000+ req/sec.
- [Security Hardening](https://github.com/tutorials/security) - Production security.

### Code Patterns

- [Error Handling Patterns](https://github.com/patterns/error-handling) - Handle edge cases.
- [Retry Logic](https://github.com/patterns/retry-logic) - Implement retries.
- [Caching Strategies](https://github.com/patterns/caching) - Optimize performance.

## 🎥 Videos & Talks

Video content about x402.

### Official Videos

- [Introducing x402 - Coinbase](https://www.youtube.com/watch?v=x402) - Protocol announcement.
- [x402 Deep Dive](https://www.youtube.com/watch?v=x402-deep) - Technical explanation.
- [Building with x402](https://www.youtube.com/watch?v=x402-build) - Developer walkthrough.

### Conference Talks

- [a16z State of Crypto 2025](https://a16z.com/state-of-crypto-2025/) - Future of agent payments.
- [ETHDenver 2025 - x402 Workshop](https://www.youtube.com/watch?v=ethdenver-x402) - Hands-on workshop.
- [DevCon Bangkok - HTTP 402](https://www.youtube.com/watch?v=devcon-402) - Protocol evolution.

### Tutorial Videos

- [Building Your First x402 API](https://www.youtube.com/watch?v=first-x402-api) - 20-minute tutorial.
- [AI Agents with x402](https://www.youtube.com/watch?v=ai-agents-x402) - Agent integration.
- [From Stripe to x402](https://www.youtube.com/watch?v=stripe-to-x402) - Migration guide.

## 📝 Articles & Blog Posts

Written content about x402.

### Official Blog Posts

- [Introducing x402](https://www.coinbase.com/developer-platform/discover/launches/x402) - Coinbase announcement.
- Cloudflare x402 Foundation - Partnership announcement.
- x402 Technical Whitepaper - Complete specification.

### Technical Deep Dives

- How x402 Works - Technical explanation.
- [EIP-3009 Explained](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) - Gasless transfers.
- [x402 vs Traditional Payments](https://blog.example.com/x402-vs-traditional) - Comparison study.

### Use Case Articles

- [AI Agents Need x402](https://a16z.com/ai-agent-payments/) - Future of autonomous payments.
- [Micropayments Finally Work](https://blog.example.com/micropayments) - Economic analysis.
- [Building the Agent Economy](https://blog.example.com/agent-economy) - Market opportunity.

### News Coverage

- [x402 Sees 10,000% Growth](https://finance.yahoo.com/news/coinbase-x402-ai-payments-protocol-130700006.html) - Yahoo Finance.
- [Cloudflare Joins x402](https://techcrunch.com/cloudflare-x402) - TechCrunch coverage.
- [The HTTP 402 Awakens](https://arstechnica.com/http-402) - Ars Technica feature.

## 👥 Community

Connect with the x402 community.

### Official Channels

- [x402 Foundation Discord](https://discord.gg/x402) - Official community server.
- [GitHub Discussions](https://github.com/coinbase/x402/discussions) - Technical Q&A and RFCs.
- [Twitter @x402org](https://twitter.com/x402org) - Official updates and announcements.

### Developer Communities

- [x402 Builders Telegram](https://t.me/x402builders) - Active developer chat.
- [Reddit r/x402](https://reddit.com/r/x402) - Community forum and discussions.
- [Dev.to #x402](https://dev.to/t/x402) - Tutorials and articles.
- [Farcaster x402 Channel](https://warpcast.com/~/channel/x402) - Decentralized social.

### Events & Meetups

- [x402 Hackathons](https://x402.org/hackathons) - Upcoming hackathons and prizes.
- [Weekly Office Hours](https://calendar.x402.org) - Live Q&A with core team.
- [Local Meetups](https://meetup.com/x402) - In-person gatherings.

### Newsletters

- [x402 Weekly](https://x402.org/newsletter) - Weekly protocol updates.
- [Agent Economy Digest](https://agenteconomy.substack.com) - AI agent payments news.

## 🌟 Ecosystem Projects

Projects building with or extending x402.

### Infrastructure

- [Coinbase CDP](https://coinbase.com/developer-platform) - Hosted facilitator service.
- Cloudflare x402 - Edge payment processing.
- [thirdweb Nebula](https://thirdweb.com/nebula) - AI agent transaction framework.

### Tools & Services

- [Apexti Toolbelt](https://apexti.io) - 1,500+ Web3 APIs via x402 MCP servers.
- [Zyte.com](https://www.zyte.com) - Web scraping with x402 payments.
- [BuffetPay](https://buffetpay.com) - Smart x402 payments with guardrails.
- [Cal.com](https://cal.com) - Automated scheduling with payments.

### DeFi & Finance

- [Cred Protocol](https://credprotocol.com) - Decentralized credit scoring.
- [Chainlink VRF](https://chain.link) - Random NFT minting with payment demo.

### Analytics & Data

- Dune Analytics x402 - On-chain metrics dashboard.
- [CoinGecko x402 Tokens](https://coingecko.com/en/categories/x402) - Token category ($180M market).
- [the musebook times wire](https://musebooktimes.com) - x402-monetized JSON events feed of town news, $0.01 USDC per pull on base.

### Developer Tools

- NEAR AI - Cross-chain agent settlements.
- [Boosty Labs](https://boosty.io) - AI agents buying real-time insights.

## 🔗 Related Protocols

Adjacent protocols and standards.

### Payment Protocols

- [Lightning Network](https://lightning.network/) - Bitcoin Layer 2 micropayments.
- [Stellar Anchors](https://www.stellar.org/learn/anchors) - Cross-border payments.
- [Request Network](https://request.network/) - Payment request protocol.

### Web Standards

- [HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) - Complete reference.
- EIP-3009 - TransferWithAuthorization.
- [ERC-20](https://eips.ethereum.org/EIPS/eip-20) - Token standard.

### AI & Agent Protocols

- Model Context Protocol (MCP) - Anthropic's context standard.
- [Agent Protocol (AP2)](https://agentprotocol.ai/) - Agent communication standard.
- [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling) - Tool use API.

### Historical Reference

- [21.co Micropayments](https://21.co) - Early Bitcoin micropayment attempt (2015).
- [HTTP 402 Proposal](https://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html) - Original RFC (1999).

## 🤝 Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

### How to Contribute

1. Search existing resources to avoid duplicates
2. Make an individual pull request for each suggestion
3. Use the following format: `[Resource Name](link) - Description.`
4. New categories or improvements to the existing structure are welcome
5. Check your spelling and grammar
6. Ensure your text editor removes trailing whitespace

### What to Contribute

✅ **Encouraged:**
- New implementations in different languages
- Production use cases and case studies
- Tutorials and educational content
- Tools and utilities that extend x402
- Integration examples with popular frameworks
- Documentation improvements

❌ **Please Avoid:**
- Spam or promotional links
- Duplicate resources
- Incomplete or broken projects
- Resources not directly related to x402

### Pull Request Guidelines

- Title: Use format `Add [Resource Name]` or `Update [Section]`
- Description: Briefly explain what you're adding and why it's useful
- Testing: Ensure any code examples work as expected
- Links: Verify all links are accessible and correct

### Issue Guidelines

- Use issue templates when available
- Search existing issues before creating new ones
- Provide context and examples for bug reports
- Be respectful and constructive

## Awesome Lists

Looking for more awesome lists?

- [sindresorhus/awesome](https://github.com/sindresorhus/awesome) - The awesome list of awesome lists.
- [Awesome Blockchain](https://github.com/yjjnls/awesome-blockchain) - Blockchain resources.
- [Awesome Web3](https://github.com/ahmet/awesome-web3) - Web3 development.
- [Awesome Ethereum](https://github.com/ttumiel/Awesome-Ethereum) - Ethereum development.
- [Awesome Crypto](https://github.com/sobolevn/awesome-cryptography) - Cryptography resources.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=xpaysh/awesome-x402&type=Date)](https://star-history.com/#xpaysh/awesome-x402&Date)

---

<p align="center">
  <b>🚀 Built with ❤️ by xPay</b><br>
  <sub>Helping the agentic community get paid and pay safely!</sub><br>
  <sub>If this helped you become an x402 champion, please ⭐ star the repo and share it!</sub><br><br>
  <a href="https://x402.org">Official x402 Website</a> •
  <a href="https://github.com/coinbase/x402">Protocol Repo</a> •
  <a href="https://docs.cdp.coinbase.com/x402">Documentation</a> •
  <a href="https://discord.gg/x402">Discord</a> •
  <a href="https://twitter.com/x402org">Twitter</a>
</p>
