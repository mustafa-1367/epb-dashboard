# e-Participatory Budgeting (e-PB) Dashboard

A blockchain-powered citizen participatory budgeting platform for Estonian municipalities. Built as a single-page application that simulates on-chain governance with full transparency, role-based access control, and a complete 7-phase budgeting lifecycle.

## Live Demo

Open `governance-dashboard.html` directly in any modern browser — no server or build tools required.

## Features

### 7-Phase e-PB Lifecycle

| Phase | Name | Description |
|-------|------|-------------|
| 1 | **Budget Determination** | Government sets total participatory budget on-chain |
| 2 | **Idea Submission** | Citizens (age 14+) submit proposals with optional anonymization |
| 3 | **Public Discussion** | Citizens like, comment, and discuss proposals |
| 4 | **Expert Evaluation** | Verified experts approve/reject with feasibility scores |
| 5 | **Citizen Voting** | One-user-one-vote with anonymized demographics |
| 6 | **Implementation** | City council approval, milestone tracking, fund disbursement |
| 7 | **Feedback Gathering** | Post-implementation 1-5 star ratings and comments |

### Smart Contract Simulation

- Simulated Polygon PoS blockchain with live block counter
- Unique transaction hashes for every on-chain action
- Immutable audit trail for all decisions, votes, and fund movements
- On-chain record verification by transaction hash

### Role-Based Access Control (RBAC)

| Role | Capabilities |
|------|-------------|
| **Citizen** | Submit proposals, vote, comment, like, provide feedback |
| **Government** | Set budget, approve implementation, all citizen actions |
| **Expert** | Evaluate proposals (approve/reject/revision), all citizen actions |

### Additional Features

- **Voter Anonymization**: Voter identity hidden while preserving demographic data for statistics
- **One-User-One-Vote**: Smart contract enforces single vote per citizen per proposal
- **Age Eligibility**: Minimum age 14 for idea submission (Estonian e-PB rules)
- **15 Estonian Counties**: Full maakond (county) coverage with participation tracking
- **Demographics Dashboard**: Gender distribution (donut chart), age distribution, population pyramid, participation rates by gender/age, county-level breakdown
- **Budget Allocation**: Interactive sliders for category-based budget preference voting
- **Real-time Statistics**: Dynamic stats that update as citizens interact
- **Dark Theme UI**: Modern dark interface with responsive design

## Project Structure

```
epb-dashboard/
├── governance-dashboard.html   # Complete application (HTML + CSS + JS)
├── README.md                   # Project documentation
├── LICENSE                     # MIT License
└── .gitignore                  # Git ignore rules
```

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/mustafa-1367/epb-dashboard.git
   cd epb-dashboard
   ```

2. **Open in browser**
   ```bash
   open governance-dashboard.html
   ```
   Or simply double-click the file.

3. **Connect Wallet** — Click "Connect Wallet" in the header to start interacting.

4. **Switch Roles** — After connecting, use the role selector (Citizen / Gov / Expert) to test different access levels.

## How to Use

### As a Citizen
1. Connect wallet
2. Navigate to **Submit Proposal** tab
3. Fill in proposal details (title, category, district, budget, age)
4. Submit — your proposal enters the Discussion phase
5. Visit **Discussion** tab to comment on and like proposals
6. Vote on proposals in the **Vote & Allocate** tab
7. Rate completed projects in the **Feedback** tab

### As Government
1. Connect wallet and switch role to **Gov**
2. Set the participatory budget in the **Dashboard** tab
3. Monitor proposals, votes, and fund allocation
4. Approve implementations in the **Implementation** tab

### As Expert
1. Connect wallet and switch role to **Expert**
2. Navigate to **Expert Review** tab
3. Evaluate proposals with feasibility scores and justification
4. Approved proposals automatically move to the Voting phase

## Technology

- **HTML5** — Semantic markup, forms, tables
- **CSS3** — Custom properties, `conic-gradient` charts, flexbox, grid, animations
- **Vanilla JavaScript (ES6+)** — Classes, template literals, Sets, array methods
- **No external dependencies** — Zero frameworks, zero libraries, zero build tools

## Estonian Administrative Structure

The platform covers all 15 Estonian counties (maakond):

Harju, Hiiu, Ida-Viru, Jogeva, Jarva, Laane, Laane-Viru, Polva, Parnu, Rapla, Saare, Tartu, Valga, Viljandi, Voru

## Screenshots

> Open `governance-dashboard.html` in your browser to see the full dashboard.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
