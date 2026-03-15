# StellarTrack-Frontend

StellerTrack is a **transparent, milestone-based donation platform** built on the Stellar ecosystem. This frontend application provides donors, charities, and validators with a **clear and intuitive interface to track donations, monitor project milestones, and verify real-world impact in real time**.

The platform ensures that **donations are not blindly transferred to charities**, but instead **secured in smart contracts and released only when predefined milestones are completed and verified** using Soroban.

The CharityTrack frontend allows users to:

* Discover and donate to charity campaigns
* Monitor milestone progress
* Verify project impact
* Track donation history
* Interact with decentralized smart contracts through non-custodial wallets

By combining **blockchain transparency, milestone-based funding, and intuitive UI design**, CharityTrack transforms charitable giving into a **fully transparent and verifiable process**.

---

# ✨ Key Features

### 🌍 Campaign Discovery

Browse verified charity campaigns across multiple categories such as:

* Education
* Healthcare
* Water & sanitation
* Climate initiatives
* Disaster relief

Each campaign displays funding progress, milestone completion, and impact statistics.

---

### 💰 Transparent Donation System

Donations are sent directly to **smart contract escrow**, ensuring:

* Funds cannot be misused
* Donations are publicly verifiable
* Milestone-based release guarantees accountability

---

### 📊 Milestone Progress Tracking

Every campaign includes clearly defined milestones such as:

* Planning
* Resource procurement
* Project implementation
* Impact verification

Users can see milestone status in real time.

Example:

```
Milestone 1 – Project Planning ✅
Milestone 2 – Materials Procurement ⏳
Milestone 3 – Installation 🔒
Milestone 4 – Community Verification 🔒
```

---

### 📈 Impact Dashboard

The platform provides a visual overview of:

* Funds raised
* Funds released
* Beneficiaries impacted
* Project completion progress

This ensures donors **see the real-world impact of their contributions**.

---

### 🔐 Wallet-Based Authentication

Users interact with the platform using **non-custodial wallets**.

Supported wallet integrations include:

* Freighter
* Albedo
* Stellar Wallet Kit

Users maintain **full control of their funds and identity**.

---

### 🏛 Charity Profiles

Each verified organization has a public profile containing:

* Organization description
* Campaign history
* Completion rate
* Trust score

This improves donor confidence and accountability.

---

### 📱 Responsive User Experience

The frontend is designed to be:

* Fully responsive across devices
* Accessible and inclusive
* Fast and lightweight

Ensuring seamless use on **desktop, tablet, and mobile devices**.

---

# 🧑‍💻 Tech Stack

### Framework

Next.js (App Router)

### Language

TypeScript

### Styling

Tailwind CSS

### State Management

React Hooks

### Blockchain Integration

Stellar wallet integrations

### Smart Contract Interaction

Soroban RPC

### Deployment

Vercel

---

# 📁 Project Structure

```
.
├── public/                # Static assets
│   ├── images/
│   └── icons/
│
├── src/
│
│   ├── app/               # Next.js App Router pages
│   │   ├── campaigns/
│   │   ├── dashboard/
│   │   ├── donate/
│   │   └── profile/
│
│   ├── components/        # Reusable UI components
│   │   ├── CampaignCard
│   │   ├── DonationModal
│   │   ├── MilestoneTracker
│   │   ├── WalletConnect
│   │   └── ImpactChart
│
│   ├── hooks/             # Custom React hooks
│   │   ├── useWallet.ts
│   │   ├── useCampaigns.ts
│   │   └── useDonations.ts
│
│   ├── lib/               # Utility functions
│   │   ├── stellar.ts
│   │   ├── api.ts
│   │   └── formatters.ts
│
│   ├── services/          # API and blockchain services
│   │   ├── backend.service.ts
│   │   └── contract.service.ts
│
│   ├── styles/            # Global and modular styles
│   │   └── globals.css
│
│   ├── types/             # Shared TypeScript interfaces
│   │   ├── campaign.ts
│   │   ├── milestone.ts
│   │   └── donation.ts
│
│   └── data/              # Static and mock data
│
├── middleware.ts
├── .gitignore
├── CONTRIBUTING.md
├── README.md
├── components.json
├── eslint.config.mjs
├── next.config.ts
├── package-lock.json
```

---

# 📦 Installation & Setup

## Prerequisites

Before running the project locally, ensure the following are installed:

* Node.js 18+
* npm or yarn
* A supported Stellar wallet

---

## Local Development

### Install dependencies

```
npm install
```

---

### Start development server

```
npm run dev
```

The application will be available at:

```
http://localhost:3000
```

---

# 🌐 Environment Variables

Create a `.env.local` file in the project root.

```
NEXT_PUBLIC_API_BASE_URL=http://localhost:4000
NEXT_PUBLIC_STELLAR_NETWORK=testnet
NEXT_PUBLIC_SOROBAN_RPC_URL=https://soroban-testnet.stellar.org
NEXT_PUBLIC_CONTRACT_ID=your_contract_address
```

---

# 🧪 Testing

CharityTrack frontend includes **comprehensive testing coverage** to ensure reliability and maintainability.

### Run all tests

```
npm test
```

---

### Run tests with coverage

```
npm run test:coverage
```

---

### Run tests in watch mode

```
npm run test:watch
```

---

### Test Coverage Goals

Target coverage: **80%+**

Coverage includes:

* Unit tests for UI components
* Integration tests for donation flows
* Wallet connection testing
* Campaign browsing flows

The CI/CD pipeline automatically verifies coverage thresholds.

---

# 🚀 CI/CD Pipeline

This project uses **GitHub Actions** to automate testing, linting, and deployment.

---

## Workflows

### Continuous Integration (CI)

Runs on all pull requests and includes:

* Linting checks
* Unit and integration tests
* Build verification

---

### Deploy to Staging

Automatically deploys the **develop branch** to the staging environment.

---

### Deploy to Production

Automatically deploys the **main branch** to production using Vercel.

---

## Quick Setup

Install dependencies including Git hooks.

```
npm install
npm run prepare
```

Run CI checks locally:

```
npm run lint
npm run test
npm run build
```

Detailed documentation:

```
.github/CICD.md
```

Quick reference guide:

```
.github/QUICK_REFERENCE.md
```

---

# 🔗 Useful Links

Stellar Developer Docs
[https://developers.stellar.org](https://developers.stellar.org)

Soroban Smart Contracts
[https://soroban.stellar.org/docs](https://soroban.stellar.org/docs)

Next.js Documentation
[https://nextjs.org/docs](https://nextjs.org/docs)

Tailwind CSS
[https://tailwindcss.com/docs](https://tailwindcss.com/docs)

---

# 🤝 Contributing

Contributions are welcome 🚀

To contribute:

1. Fork the repository
2. Create a feature branch
3. Write clear and descriptive commit messages
4. Submit a pull request

All contributions are reviewed before merging.

---

# 📜 License

MIT License


