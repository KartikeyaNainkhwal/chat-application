

---

### Author Information

**Name:** Kartikeya Nainkhwal  
**University:** Indian Institute of Technology Bhilai (IIT Bhilai)  
**Department:** Computer Science Eng. (CSE)  

---

If you provide your department name, I can include it in the description.


```markdown
# Chat Application

## Overview

This chat application is a real-time messaging platform built with Next.js, MongoDB, Pusher, Cloudinary, and OAuth authentication using GitHub and Google. It supports user authentication, real-time messaging, and media file uploads.

## Features

- **User Authentication**: Sign in using GitHub or Google.
- **Real-Time Messaging**: Powered by Pusher.
- **Media Uploads**: Integrates with Cloudinary for handling images.
- **Responsive Design**: Built with Next.js and Tailwind CSS.

## Tech Stack

- **Frontend**: Next.js, React, Tailwind CSS
- **Backend**: Node.js, MongoDB, Pusher
- **Authentication**: NextAuth.js, OAuth (GitHub & Google)
- **Media Storage**: Cloudinary

## Prerequisites

- [Node.js](https://nodejs.org/en/download/) (version 14.x or higher)
- MongoDB Atlas account or local MongoDB setup
- GitHub and Google developer accounts for OAuth setup
- Cloudinary account for media uploads
- Pusher account for real-time functionality

## Getting Started

### 1. Clone the Repository

Clone the project repository to your local machine:

```bash
git clone https://github.com/your-username/chat-application.git
cd chat-application
```

### 2. Install Dependencies

Install all necessary dependencies:

```bash
npm install
# or
yarn install
```

### 3. Setup Environment Variables

Create a `.env` file in the root directory of the project. Copy and paste the environment variables below into the `.env` file, replacing placeholders with your actual credentials.

```bash
# MongoDB URL
DATABASE_URL="mongodb+srv://<username>:<db_password>@cluster0.iqybizk.mongodb.net/<databaseName>?retryWrites=true&w=majority"

# NextAuth URL
NEXTAUTH_URL=http://localhost:3003

# NextAuth secret (generate a random string)
NEXTAUTH_SECRET="your-random-secret"

# GitHub OAuth credentials
GITHUB_CLIENT_ID=<your-github-client-id>
GITHUB_CLIENT_SECRET=<your-github-client-secret>

# Google OAuth credentials
GOOGLE_CLIENT_ID=<your-google-client-id>
GOOGLE_CLIENT_SECRET=<your-google-client-secret>

# Cloudinary credentials
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=<your-cloudinary-cloud-name>
NEXT_PUBLIC_CLOUDINARY_CLOUD_PRESET=<your-cloudinary-cloud-preset>

# Pusher credentials
PUSHER_APP_ID=<your-pusher-app-id>
PUSHER_APP_SECRET=<your-pusher-app-secret>
NEXT_PUBLIC_PUSHER_APP_KEY=<your-pusher-app-key>
NEXT_PUBLIC_PUSHER_APP_CLUSTER=<your-pusher-app-cluster>
```

### 4. Run the Application Locally

Start the application in development mode:

```bash
npm run dev
# or
yarn dev
```

The application will be available at [http://localhost:3003](http://localhost:3003).

### 5. OAuth Configuration

#### GitHub OAuth

1. Go to your [GitHub Developer Settings](https://github.com/settings/developers) and create a new OAuth app.
2. Set the callback URL to `http://localhost:3003/api/auth/callback/github`.
3. Update `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` in your `.env` file with the credentials obtained.

#### Google OAuth

1. Go to the [Google Cloud Console](https://console.cloud.google.com/), create a new project, and configure the OAuth consent screen.
2. Create OAuth credentials with the redirect URI `http://localhost:3003/api/auth/callback/google`.
3. Update `GOOGLE_CLIENT_ID` and `GOOGLE_CLIENT_SECRET` in your `.env` file with the credentials obtained.

### 6. Deploying to Production

When deploying to a cloud service like [Vercel](https://vercel.com/), ensure you update `NEXTAUTH_URL` in your `.env` file to your production URL.

Example:

```bash
NEXTAUTH_URL=https://your-production-url.com
```

### 7. Optional Steps for Cloudinary & Pusher

#### Cloudinary

- Sign up for a Cloudinary account [here](https://cloudinary.com/).
- Retrieve your cloud name and preset from the Cloudinary dashboard.
- Update `NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME` and `NEXT_PUBLIC_CLOUDINARY_CLOUD_PRESET` in your `.env` file.

#### Pusher

- Sign up for a Pusher account [here](https://pusher.com/).
- Create a new app and obtain the app ID, secret, key, and cluster.
- Update `PUSHER_APP_ID`, `PUSHER_APP_SECRET`, `NEXT_PUBLIC_PUSHER_APP_KEY`, and `NEXT_PUBLIC_PUSHER_APP_CLUSTER` in your `.env` file.

### 8. MongoDB Setup

1. Set up a MongoDB Atlas cluster or install MongoDB locally.
2. Replace `<db_password>` and `<databaseName>` in `DATABASE_URL` with your MongoDB credentials.
3. Whitelist your IP address on MongoDB Atlas under "Network Access."

### 9. Available Scripts

- **`npm run dev`**: Starts the development server.
- **`npm run build`**: Builds the application for production.
- **`npm start`**: Starts the production server after build.

## Contributing

Contributions are welcome! Please submit issues, bugs, or feature requests. Pull requests are also appreciated.

## License

This project is licensed under the [MIT License](LICENSE).

## Additional Resources

- **[Next.js Documentation](https://nextjs.org/docs)**: Explore the power of Next.js for building your web applications. Learn about its file-based routing, API routes, and optimized performance features.
- **[NextAuth.js Documentation](https://next-auth.js.org/getting-started/introduction)**: Learn more about authentication in Next.js using NextAuth.js. Understand how to implement session management, secure your APIs, and support multiple providers.
- **[Tailwind CSS Documentation](https://tailwindcss.com/docs)**: Dive into the documentation for Tailwind CSS, a utility-first CSS framework. Discover how to rapidly build custom designs with a low-level utility approach.
- **[Pusher Documentation](https://pusher.com/docs)**: Explore Pusher for adding real-time functionality to your applications. Learn how to integrate real-time notifications, chat functionality, and presence channels.
- **[React Icons Documentation](https://react-icons.github.io/react-icons/)**: Find and customize high-quality SVG icons for your React applications. Utilize a large collection of icons from popular libraries like FontAwesome and Material Design.
- **[React Select Documentation](https://react-select.com/home)**: Get to know more about React Select, a flexible and customizable select component. Learn how to handle complex form inputs with ease.
- **[React Hook Form Documentation](https://react-hook-form.com/get-started)**: Learn about React Hook Form for efficient form management in React. Understand how to build performant forms with minimal re-renders.
- **[Next Cloudinary Documentation](https://cloudinary.com/documentation/nextjs_image_and_video)**: Understand how to integrate Cloudinary for image and video management. Explore features like optimization, transformations, and responsive image delivery.
- **[Prisma Documentation](https://www.prisma.io/docs/)**: Explore Prisma for database access in TypeScript and JavaScript. Learn about its ORM capabilities, schema modeling, and database migrations.
- **[Axios Documentation](https://axios-http.com/docs/intro)**: Find information on how to use Axios for making HTTP requests. Learn how to handle requests, responses, and error handling with ease.
- **[Zustand Documentation](https://github.com/pmndrs/zustand)**: Learn about Zustand, a small and fast state management library. Discover how to manage application state with a minimal API and improved performance.
- **[React Hot Toast Documentation](https://react-hot-toast.com/docs)**: Understand how to use React Hot Toast for toast notifications in React applications. Explore its features for displaying notifications with various styles and positions.
- **[Headless UI Documentation](https://headlessui.dev/)**: Explore Headless UI, a set of completely unstyled UI components. Learn how to build accessible and customizable components without sacrificing functionality.

> **Note:** Please keep your API keys and configuration values secure and do not expose them publicly.
```

This version includes detailed features for each additional resource, making the `README.md` more informative and useful for anyone setting up or working with your project.
