<div align="center">

# ⌨️ TECHFEST TYPING ENGINE
### **Precision. Speed. Zero Latency.**

A high-performance, real-time typing competition orchestrator designed for competitive tech environments. Built to handle intense traffic with sub-millisecond synchronization.

[![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.dot-io&logoColor=white)](https://socket.io/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![NodeJS](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Anti-Cheat](https://img.shields.io/badge/Anti--Cheat-Active-red?style=for-the-badge&logo=securityscorecard&logoColor=white)](#)

---

[🎮 Live Demo](#) • [🛠️ Architecture](#-system-architecture) • [🚀 Deploy](#-installation) • [🔒 Security](#-anti-cheat-measures)

</div>

---

## 🔥 The Core Engine

This isn't just a typing site; it's an **event-driven battleground**. Designed specifically for TechFests, it replaces unreliable manual scoring with a robust, automated pipeline.

### 🏗️ System Architecture

The platform follows a **Real-Time Event-Driven** pattern to ensure every keystroke counts.

```text
TypingEngine (Core Orchestrator)
┃
┣━━ 📡 Real-Time Layer (Socket.io)
┃   ┣━━ ⚡ Low-Latency Sync ....... [Room-based Scaling]
┃   ┣━━ ⏱️ NTP Time Sync ........... [Clock Drift Correction]
┃   ┗━━ 📊 Live Leaderboard ........ [Broadcast Updates]
┃
┣━━ 🛡️ Security & Integrity
┃   ┣━━ 🚫 Anti-Cheat Engine ....... [WPM/Input Anomalies]
┃   ┣━━ 🔒 JWT Authentication ...... [Identity Security]
┃   ┗━━ 🚦 Rate Limiter ............ [DDoS Protection]
┃
┣━━ 📦 Persistence Layer
┃   ┣━━ 🍃 MongoDB ................. [Result History]
┃   ┗━━ 📋 Match Logging ........... [Audit Trails]
┃
┗━━ 📊 Observability
    ┗━━ 📝 Structured Logger ....... [Match Analytics]
✨ Features That Win
⚡ Real-time Synchronization: Every competitor sees their opponents' progress in real-time without refreshing.

🛡️ Hardened Anti-Cheat: Intelligent logic to detect copy-pasting, script-injection, and impossible WPM spikes.

📊 Live Dashboards: Large-screen optimized views for event halls, showing the top 10 rankings dynamically.

📱 Ultra-Responsive: Built with Vanilla JS for maximum performance and minimal client-side overhead.

🚀 Quick Deployment
Bash

# Clone the repository
git clone [https://github.com/your-username/techfest-typing.git](https://github.com/your-username/techfest-typing.git) && cd techfest-typing

# Configure environment
echo "PORT=3000\nMONGO_URI=your_uri\nJWT_SECRET=your_secret" > .env

<div align="center">

View Full API Documentation →

</div>
## 📖 Documentation Structure

This documentation is organized into modular files for better navigation. See the [docs](./docs/) folder for complete documentation:

- **[FEATURES.md](./docs/FEATURES.md)** - Complete feature list and capabilities
- **[SETUP.md](./docs/SETUP.md)** - Installation and configuration guide
- **[QUICKSTART.md](./docs/QUICKSTART.md)** - Quick start guide for organizers and participants
- **[ARCHITECTURE.md](./docs/ARCHITECTURE.md)** - Project structure and tech stack
- **[SOCKET_API.md](./docs/SOCKET_API.md)** - WebSocket events and communication protocol
- **[DATABASE.md](./docs/DATABASE.md)** - MongoDB schema and data structure
- **[DESIGN_SYSTEM.md](./docs/DESIGN_SYSTEM.md)** - Color tokens, typography, spacing, animations
- **[REST_API.md](./docs/REST_API.md)** - REST API endpoints and responses
- **[DEPLOYMENT.md](./docs/DEPLOYMENT.md)** - Deployment guides for Render and Railway
- **[TESTING.md](./docs/TESTING.md)** - Testing checklist and edge cases
- **[CONFIG.md](./docs/CONFIG.md)** - Configuration and customization options
- **[TROUBLESHOOTING.md](./docs/TROUBLESHOOTING.md)** - Common issues and solutions
- **[PERFORMANCE.md](./docs/PERFORMANCE.md)** - Performance metrics and optimization
- **[CONTRIBUTING.md](./docs/CONTRIBUTING.md)** - Contribution guidelines

## 🐳 Run with Docker (Recommended)

You can run the entire application stack (App + MongoDB) with a single command. No need to install Node.js or MongoDB locally.

1.  **Start the Platform**
    ```bash
    docker-compose up --build
    ```

2.  **Access Application**
    - Organizer: `http://localhost:3000/organizer`
    - Participant: `http://localhost:3000/`

---

## 🚀 Manual Quick Start

1. **Clone & Install**
   ```bash
   git clone <repository-url>
   cd typing-platform
   npm install
   ```

2. **Configure Database**
   ```bash
   # Create .env file
   MONGODB_URI=mongodb://localhost:27017/typing-platform
   PORT=3000
   NODE_ENV=development
   ```

3. **Start Server**
   ```bash
   npm start
   ```

4. **Access Application**
   - Organizer: `http://localhost:3000/organizer`
   - Participant: `http://localhost:3000/`

**Made with ❤️ for techfest typing competitions**

**Last Updated**: January 4, 2026  
**Version**: 1.0.0
