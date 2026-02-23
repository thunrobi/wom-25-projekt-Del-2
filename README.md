# wom-25-projekt-Del-2
# wom-25-projekt-Del-2

A full-stack web application built with Node.js, Prisma, and a vanilla JavaScript/CSS/HTML frontend. The project is containerized with Docker for easy setup and deployment.

## Tech Stack

- **Backend:** Node.js (`src/`)
- **Database ORM:** Prisma (`prisma/`)
- **Frontend:** HTML, CSS, JavaScript (`frontend/`)
- **Containerization:** Docker & Docker Compose
- **Testing:** Test suite in `test/`

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [Docker](https://www.docker.com/) and Docker Compose
- A compatible database (configured via Prisma — see `prisma/schema.prisma`)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/thunrobi/wom-25-projekt-Del-2.git
   cd wom-25-projekt-Del-2
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root directory and configure your database connection:

   ```env
   DATABASE_URL="your-database-connection-string"
   ```

4. **Run Prisma migrations:**

   ```bash
   npx prisma migrate dev
   ```

5. **Start the development server:**

   ```bash
   npm start
   ```

### Running with Docker

To spin up the full application stack using Docker Compose:

```bash
docker-compose up --build
```

This will build and start all services defined in `docker-compose.yml`.

## Project Structure

```
wom-25-projekt-Del-2/
├── frontend/        # Static frontend (HTML, CSS, JS)
├── prisma/          # Prisma schema and migrations
├── src/             # Backend application source code
├── test/            # Test files
├── Dockerfile       # Docker image configuration
├── docker-compose.yml
└── package.json
```

## Running Tests

```bash
npm test
```

## License

This project is for educational purposes as part of the WOM-25 course.
