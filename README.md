# AbZ
unicorn
 
# CommitCircle 🚀

> Stay consistent. Stay accountable. Win together.

CommitCircle is a social accountability platform where friends form groups around a common goal, commit virtual stake points, and stay consistent through daily check-ins. Members who miss their commitments lose points, which are redistributed among those who successfully complete their daily tasks.

This repository contains the MVP (Minimum Viable Product) focused on validating the core idea with manual verification and a simple chat-based interface.

---

## 📖 Problem Statement

Many people start habits such as:

- 🏋️ Going to the gym
- 💻 Coding every day
- 📚 Studying consistently
- 🧘 Meditation
- 🥗 Healthy eating
- 🏃 Running

Most habit-tracking apps fail because there is no real consequence for missing a day.

CommitCircle introduces **social accountability + financial commitment** to motivate users to stay consistent.

---

## 💡 Idea

A group of friends creates a challenge.

Example:

- 30-Day Gym Challenge
- Daily DSA Challenge
- Study Together Challenge

Each member joins with a fixed number of stake points.

Every day:

- Complete the task
- Upload proof
- Other members manually verify it

If a member misses:

- A predefined penalty is deducted from their stake.
- The deducted points are distributed equally among members who completed the task.

At the end of the challenge, users receive their remaining (or increased) balance.

---

# 🎯 MVP Scope

The MVP focuses on validating the concept.

### Authentication

- User Registration
- Login
- JWT Authentication

### Groups

- Create Group
- Join Group
- View Members

### Challenges

- Create Challenge
- Daily Task
- Duration
- Penalty Points

### Daily Check-ins

- Upload Proof
- Submission Status
- View Previous Submissions

### Manual Verification

- Approve Submission
- Reject Submission
- Majority Decision

### Wallet

- Virtual Stake Points
- Automatic Penalty Distribution
- Transaction History

### Chat

- Real-time Group Chat

### Leaderboard

- Current Streak
- Points
- Rank
- Completion Percentage

---

# 🚧 Out of Scope (MVP)

The following features will be added in future versions:

- AI Proof Verification
- UPI Payments
- Wallet Withdrawals
- Push Notifications
- Mobile App
- Admin Dashboard
- Public Challenges
- Third-party Integrations

---

# 🛠 Tech Stack

## Backend

- Python
- Django
- Django REST Framework
- PostgreSQL
- Django Channels
- Redis
- JWT Authentication

## Frontend

- React
- Vite
- Tailwind CSS
- Axios

## Development

- Docker
- Git
- GitHub
- Postman

---

# 📂 Planned Project Structure

```
commit-circle/

├── backend/
├── frontend/
├── docs/
│   ├── PRD.md
│   ├── API.md
│   ├── DATABASE.md
│   └── ROADMAP.md
│
├── README.md
└── .gitignore
```

---

# ⚙️ Planned Development Roadmap

## Phase 0

- Product Design
- User Stories
- Database Design
- API Design

---

## Phase 1

Authentication

- Register
- Login
- JWT

---

## Phase 2

Groups

- Create Group
- Join Group
- Member Management

---

## Phase 3

Challenges

- Create Challenge
- Challenge Rules
- Duration
- Penalty Configuration

---

## Phase 4

Daily Check-ins

- Upload Proof
- Submission Tracking

---

## Phase 5

Manual Verification

- Approve / Reject
- Verification Status

---

## Phase 6

Wallet System

- Stake Points
- Penalty Distribution
- Transaction Logs

---

## Phase 7

Real-time Chat

- WebSockets
- Group Messaging

---

## Phase 8

Leaderboard

- Rankings
- Streaks
- Statistics

---

## Phase 9

Deployment

- Docker
- Backend Deployment
- Frontend Deployment

---

# 📚 Documentation

Project documentation will be maintained inside the `docs/` directory.

- Product Requirements Document (PRD)
- Database Design
- API Documentation
- Development Roadmap

---

# 🎯 Long-Term Vision

Future versions aim to include:

- AI-based proof verification
- Payment gateway integration
- Real money staking
- Google Fit / Apple Health integration
- GitHub verification for coding challenges
- Public communities
- Corporate wellness programs
- College competitions
- Analytics Dashboard

---

# 🤝 Contributing

This project is currently under active development.

Contribution guidelines will be added as the project matures.

---

# 📄 License

This project is licensed under the MIT License.

---

## 🌟 Vision

Build a platform where consistency becomes rewarding, accountability is social, and achieving goals is a shared journey.