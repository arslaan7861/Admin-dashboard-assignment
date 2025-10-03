# 📚 School Management Dashboard

A scalable School Management System built with Next.js that enables admins to manage students, classes, attendance, and subjects seamlessly. This dashboard also supports profile picture uploads using Cloudinary and provides a clean, responsive UI for efficient school data management.

##🚀 Features

Authentication & Admin Dashboard

Secure login with environment-based admin credentials

JWT authentication for API protection

Student Management

Add and update student profiles with photo upload (Cloudinary integration)

Maintain student records across sessions

Class & Subject Management

Create and manage classes for each session

Assign subjects to classes

Attendance Tracking

Mark daily attendance for students

Track class-wise attendance

Scalable Structure

Modular API integration with Next.js API routes

MongoDB database for persistence

Cloudinary for secure file storage

##🛠️ Tech Stack

Frontend & Backend: Next.js (Full-stack)

Database: MongoDB (Mongoose ODM)

Authentication: JWT-based auth

File Uploads: Cloudinary

Styling: Tailwind CSS / ShadCN UI

Password Hashing: bcrypt

##⚙️ Environment Variables

Create a .env.local file in the root directory and configure the following:

ADMIN_PHONENUMBER=1234567890
ADMIN_PASSWORD=password
ADMIN_ID=123123123
ADMIN_NAME=Admin
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_super_secure_secret_key
CLOUDINARY_SECRET=your_cloudinary_secret
CLOUDINARY_KEY=your_cloudinary_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name

##▶️ Getting Started

Clone the repository

git clone https://github.com/your-username/school-management-dashboard.git
cd school-management-dashboard

Install dependencies

npm install

# or

yarn install

Setup environment variables
Create a .env.local file and add the required variables (see above).

Run the development server

npm run dev

# or

yarn dev

Open in browser
Visit http://localhost:3000

📂 Project Structure
school-management-dashboard/
│
├── public/ # Static assets
├── src/ # Source code
│ ├── app/ # Next.js App Router pages
│ ├── components/ # Reusable UI components
│ │ ├── common/ # Shared/common components
│ │ ├── school/ # School-related components
│ │ ├── students/ # Student-related components
│ │ └── ui/ # UI-specific components
│ ├── lib/ # Utility functions
│ │ ├── cloudinary.ts # Cloudinary configuration
│ │ ├── types.ts # Type definitions
│ │ └── utils.ts # Helper utilities
│ └── server/ # Server-side logic
│ ├── actions/ # Business logic/actions
│ ├── DB/ # Database connection/config
│ ├── repository/ # Data access layer (Mongoose ops)
│ └── utils/ # Server utilities
│
├── components.json # shadcn/ui config
├── eslint.config.mjs # ESLint config
├── next-env.d.ts # Next.js TypeScript env
├── next.config.ts # Next.js config
├── package.json # Project dependencies
├── package-lock.json # Dependency lock file
├── postcss.config.mjs # PostCSS config
├── tsconfig.json # TypeScript config
└── README.md # Project documentation

##🔒 Security & Scalability

Environment variables secured in .env.local

JWT authentication for protected APIs

Modular architecture for scaling with more features (fees, exams, parent portal, etc.)

##📜 License

This project is licensed under the MIT License.
