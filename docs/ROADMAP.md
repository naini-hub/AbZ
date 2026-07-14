# CommitCircle Development Roadmap (From Scratch)

## Project Goal

Build a social accountability platform where groups of friends create challenges, submit proof of completion, vote on each other's submissions, and give a treat if someone misses too many times.

The goal of the first version is **validation**, not perfection.

---

# Phase 1: Understand the Problem

## Problem Statement

People often make commitments in groups:

* Going to the gym daily
* Solving coding problems every day
* Studying for exams
* Waking up early
* Reading books

Most of these commitments fail within a few days because there is no accountability.

Current habit tracker apps depend on self-reporting, which makes cheating easy.

---

## Proposed Solution

CommitCircle introduces:

* Group accountability
* Photo proof submission
* Peer verification
* Social consequences
* Friendly penalties

The idea is simple:

> It is easier to ignore an app than to disappoint your friends.

---

# Phase 2: Define MVP Features

The first version must contain only the following features.

## User Features

### Authentication

* Register
* Login
* Logout

### Group Management

* Create group
* Join group using invite code
* View group members

### Challenge Management

* Create challenge
* Set challenge goal
* Set miss threshold
* Set treat name

Example:

Goal:

```
Gym Daily
```

Miss Threshold:

```
3 misses
```

Treat:

```
Pizza
```

---

### Daily Submission

Users upload:

* Gym selfie
* Study screenshot
* Running photo
* Any required proof

Only one proof submission per user per day.

---

### Voting System

Each group member can vote:

* Approve
* Reject

Majority decides the result.

---

### Miss Counter

Miss count increases if:

* No submission was uploaded.
* Submission was rejected.

---

### Treat Ledger

When miss threshold is crossed:

Example:

```
Rahul owes Pizza to Gym Squad
```

Miss count resets to zero.

---

### Activity Feed

Display all actions:

```
Rahul uploaded proof.
Priya approved Rahul's proof.
Aman missed today's challenge.
Rohit owes the squad pizza.
```

---

# Phase 3: Learn Required Technologies

## Backend

### Python

Learn:

* Variables
* Functions
* Classes
* Lists
* Dictionaries
* OOP

---

### Django

Learn:

* Projects
* Apps
* Models
* URLs
* Views
* Admin Panel
* Migrations

---

### Django REST Framework

Learn:

* Serializers
* API Views
* ViewSets
* Authentication
* Permissions

---

### PostgreSQL

Learn:

* Tables
* Relationships
* Foreign Keys
* Queries

---

## Frontend

### React

Learn:

* Components
* Props
* State
* Hooks
* Routing
* API Calls

---

### PWA Concepts

Learn:

* Service Workers
* Manifest File
* Installable Applications

---

## Collaboration

Learn Git:

* Clone
* Commit
* Push
* Pull
* Branch
* Pull Request

Never push directly to main branch.

---

# Phase 4: Design Database

## User Table

Fields:

* id
* username
* email
* password
* profile_image
* created_at

---

## Group Table

Fields:

* id
* name
* invite_code
* created_by
* created_at

---

## GroupMember Table

Fields:

* user_id
* group_id
* miss_count
* joined_at

---

## Challenge Table

Fields:

* id
* group_id
* goal
* miss_limit
* treat_name
* start_date
* end_date

---

## Submission Table

Fields:

* id
* user_id
* challenge_id
* image
* status
* submitted_at

Status values:

* Pending
* Approved
* Rejected

---

## Vote Table

Fields:

* id
* submission_id
* voter_id
* vote

---

## TreatLedger Table

Fields:

* id
* user_id
* group_id
* treat_name
* paid
* timestamp

---

# Phase 5: Build Backend APIs

Build APIs in this order.

## Authentication APIs

* Register
* Login
* Logout

---

## Group APIs

* Create Group
* Join Group
* Get Group Details

---

## Challenge APIs

* Create Challenge
* Edit Challenge
* Fetch Challenge

---

## Submission APIs

* Upload Proof
* Fetch Today's Proofs

---

## Voting APIs

* Cast Vote
* Get Vote Count
* Determine Result

---

## Treat APIs

* Fetch Pending Treats
* Mark Treat Paid

---

# Phase 6: Build Frontend

Create pages in this order:

1. Login
2. Register
3. Dashboard
4. Create Group
5. Join Group
6. Challenge Page
7. Upload Proof Page
8. Voting Page
9. Activity Feed
10. Treat Ledger

---

# Phase 7: Add Image Upload

Store images using:

* Local storage during development.
* Cloudinary free tier in production.

---

# Phase 8: Add Real-Time Features

Use:

* Django Channels
* WebSockets

Real-time updates:

* New proof uploaded
* New vote received
* Miss count updated
* Treat triggered

---

# Phase 9: Convert Into PWA

Features:

* Install to Home Screen
* Offline support
* App icon
* Splash screen

---

# Phase 10: Testing

Test:

* Duplicate voting
* Invalid uploads
* Missing submissions
* Simultaneous votes
* Edge cases

---

## Validation Metrics

Track only:

* Day 1 retention
* Day 3 retention
* Day 7 retention

Ignore:

* Revenue
* Funding
* Branding
* Company registration

during the validation stage.

---

# Recommended Folder Structure

## Backend

backend/

* users
* groups
* challenges
* submissions
* votes
* treats
* notifications

## Frontend

frontend/

* pages
* components
* hooks
* services
* assets

---

# Recommended Team Structure

## Backend Engineer

Responsible for:

* APIs
* Database
* Authentication

## Frontend Engineer

Responsible for:

* UI
* API integration
* PWA

## Full Stack Engineer

Responsible for:

* Deployment
* WebSockets
* Production fixes

## Product Lead

Responsible for:

* Testing users
* Collecting feedback
* Measuring retention

---

