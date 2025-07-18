# 🚀 Prisma TypeScript Starter

This project demonstrates how to use **Prisma ORM** with **TypeScript** and a PostgreSQL database.

---

## 📂 Project Structure

.
├── prisma/
│ ├── schema.prisma
│ └── migrations/
├── src/
│ ├── create.ts
│ ├── read.ts
│ ├── update.ts
├── .env
├── package.json
├── tsconfig.json
└── README.md

---

## 🔧 Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [PostgreSQL](https://www.postgresql.org/) running locally or remotely

---

## 💾 Clone the repository

```bash
git clone https://github.com/tejashirve01/Prisma.git
cd Prisma
📦 Install dependencies

npm install
⚙️ Configure your environment variables
Create a .env file in the root of the project:


touch .env
Add your PostgreSQL connection string:


DATABASE_URL="postgresql://<username>:<password>@<host>:<port>/<database>"
Example for local Postgres:

DATABASE_URL="postgresql://postgres:password@localhost:5432/mydb"
🗃️ Run Prisma migrations
This sets up your database schema.

⚠️ WARNING: This will drop your dev database if it exists!

npx prisma migrate reset
If you only want to run pending migrations without dropping data:


npx prisma migrate deploy
🔄 Generate Prisma Client
After changing the schema, run:

npx prisma generate
✨ Run the code
Run your TypeScript scripts directly using ts-node:


npx ts-node src/create.ts
npx ts-node src/read.ts
npx ts-node src/update.ts
Or build the project and run the compiled JavaScript:


npm run build
node dist/create.js
🚀 Useful Scripts
View Prisma Studio (DB GUI):

npx prisma studio



