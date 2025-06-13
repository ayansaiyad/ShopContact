# MY-SHOP - Restaurant Management System

A modern web application built with Next.js and Firebase for managing restaurants and shops. This application allows users to browse, like, and manage their favorite restaurants with real-time updates.

## Features

- 🔍 Browse restaurants and shops
- ❤️ Like and save favorite restaurants
- 🔐 User authentication with Firebase
- 📱 Responsive design for all devices
- ⚡ Real-time updates with Firebase
- 🎨 Modern and clean UI

## Tech Stack

- **Frontend Framework**: Next.js 14
- **Authentication**: Firebase Authentication
- **Database**: Firebase Firestore
- **Styling**: Tailwind CSS
- **State Management**: React Context API
- **Deployment**: Vercel

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn
- Firebase account

## Getting Started

1. Download the project files
2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Create a Firebase project and add your configuration:
   - Go to Firebase Console
   - Create a new project
   - Add a web app to your project
   - Copy the Firebase configuration
   - Create a `.env.local` file in the root directory and add your Firebase config:
   ```
   NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
   NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
   NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
   NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
   NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
   NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
   ```

4. Run the development server:
```bash
npm run dev
# or
yarn dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## Project Structure

```
MY-SHOP/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   ├── components/        # Reusable components
│   ├── context/          # React context providers
│   ├── hooks/            # Custom React hooks
│   ├── lib/              # Utility functions and Firebase config
│   └── page.tsx          # Main page component
├── public/               # Static assets
├── .env.local           # Environment variables
├── firestore.rules      # Firebase security rules
└── package.json         # Project dependencies
```

## Firebase Security Rules

The application uses Firebase security rules to ensure data security. The rules allow:
- Authenticated users to read and write their own data
- Public read access to restaurant data
- Protected write access to restaurant data

## Deployment

The application is configured for deployment on Vercel. To deploy:

1. Set up your project on Vercel
2. Add your environment variables in Vercel dashboard
3. Deploy!

## Privacy and Security

This is a private project and the code is not publicly available. Please ensure:
- Keep your Firebase configuration secure
- Never commit `.env.local` file to version control
- Regularly update dependencies for security patches
- Follow Firebase security best practices

## License

This is a private project. All rights reserved.

## Support

For support, please contact the development team directly.
