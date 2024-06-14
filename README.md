# Airbnb Clone

![Airbnb Clone](https://via.placeholder.com/728x90.png?text=Airbnb+Clone)

A feature-rich Airbnb clone built with Next.js, Prisma, and other modern web technologies.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Scripts](#scripts)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication with NextAuth.js
- Database integration with Prisma
- Cloud image upload with Next Cloudinary
- Interactive date picker with React Date Range
- Map integration with React Leaflet
- State management with Zustand
- Form handling with React Hook Form
- Responsive design with TailwindCSS

## Tech Stack

- **Frontend:** React, Next.js, TailwindCSS
- **Backend:** Next.js API Routes, Prisma, NextAuth.js
- **Database:** Prisma Client
- **Other:** Axios, Bcrypt, Date-fns, Query-string, React Icons, React Spinners, World Countries

## Getting Started

Follow these steps to get the project up and running locally.

### Prerequisites

- Node.js and npm installed on your machine
- A PostgreSQL database (or another database supported by Prisma)
- A Cloudinary account for image uploads

### Installation

#### 1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/airbnb-clone.git
   cd airbnb-clone
   ```

#### 2. Install the dependencies:

   ```sh
   npm install
   ```

#### 3. Set up environment variables:

   Create a `.env` file in the root directory and add your environment variables. Here's an example:

   ```env
   DATABASE_URL="postgresql://user:password@localhost:5432/mydb"
   NEXTAUTH_URL="http://localhost:3000"
   NEXTAUTH_SECRET="yoursecret"
   CLOUDINARY_URL="cloudinary://apikey:apisecret@cloudname"
   ```

#### 4. Run database migrations:

   ```sh
   npx prisma migrate dev
   ```

#### 5. Start the development server:

   ```sh
   npm run dev
   ```

## Scripts

- `npm run dev`: Starts the development server.
- `npm run build`: Builds the application for production.
- `npm run start`: Starts the production server.
- `npm run lint`: Runs ESLint to check for linting errors.

## Configuration

### Prisma

Prisma is used for database interactions. To configure Prisma, modify the `prisma/schema.prisma` file according to your database schema and run the following command to generate the Prisma client:

```sh  
npx prisma generate
```

### NextAuth.js

NextAuth.js handles user authentication. Configure your providers and session settings in the `[...nextauth].js` file located in the `pages/api/auth` directory.

### TailwindCSS

TailwindCSS is used for styling. You can customize the TailwindCSS configuration in the `tailwind.config.js` file.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch:

   ```sh
   git checkout -b feature/YourFeature
   ```

3. Commit your changes:

   ```sh
   git commit -m 'Add some feature'
   ```

4. Push to the branch:

   ```sh
   git push origin feature/YourFeature
   ```

5. Open a pull request.

## License

This project is licensed under the MIT License.
