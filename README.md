# DevPulse – Internal Tech Issue & Feature Tracker

> A collaborative platform for software teams to report bugs, suggest features, and coordinate resolutions.
**Live URL:** ``
**GitHub:** `https://github.com/Arpitadey88/DevPulse-Assignment-2`

---

## Features

- User registration and authentication with JWT
- Role-based access control (`contributor` and `maintainer`)
- Create, view, update, and delete issues (bugs & feature requests)
- Filter and sort issues by type, status, and date
- Secure password hashing with bcrypt
- Modular, clean TypeScript architecture

---

## Tech Stack

| Technology           | Purpose                                        |
| -------------------- | ---------------------------------------------- |
| Node.js (LTS 24.x)   | Runtime environment                            |
| TypeScript           | Strongly-typed language layer                  |
| Express.js           | Web framework with modular router architecture |
| PostgreSQL           | Relational database                            |
| `pg` (native driver) | Direct database queries via `pool.query()`     |
| `bcrypt`             | Password hashing                               |
| `jsonwebtoken`       | JWT generation and verification                |
| `http-status-codes`  | Consistent HTTP status code references         |

---

## Getting Started

### Prerequisites

- Node.js LTS (24.x or higher)
- PostgreSQL database (local or cloud-hosted)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/FahimFaysalNirjhar/DevPulse-Assignment-2
cd devpulse

# 2. Install dependencies
npm install

# 3. Set up environment variables
cp .env.example .env
# Fill in your values in .env

# 4. Set up the database
psql -U your_user -d your_database -f schema.sql

# 5. Start the development server
npm run dev
```

### Environment Variables

```env
PORT=5000
DATABASE_URL=postgresql://user:password@host:5432/devpulse
JWT_SECRET=your_jwt_secret_here
```

---
