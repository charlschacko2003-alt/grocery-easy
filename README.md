# Grocery Shared Website with Login and Shared Database

This is a Vite + React + Firebase website.

It has:
- Email/password sign up and login
- Shared Firestore database
- Real-time updates for all users
- Shared grocery products and prices
- Shared house checklist: Home / Buy
- Shared buying checklist and quantities
- Add, edit and delete grocery items

## Setup

1. Install Node.js.
2. Create a Firebase project.
3. Enable Authentication → Sign-in method → Email/Password.
4. Create Firestore Database.
5. Create a Firebase Web App and copy the config values.
6. Copy `.env.example` to `.env.local` and fill your Firebase values.
7. Add the rules from `firestore.rules` to Firebase Firestore Rules.
8. Run:

```bash
npm install
npm run dev
```

## First use

1. Open the website.
2. Sign up.
3. Click **Create starter database**.
4. Share the deployed website link with others.
5. Everyone who logs in sees and edits the same data.

## Deploy

### Vercel
- Upload this folder to GitHub.
- Import the repository in Vercel.
- Add the same environment variables from `.env.local` in Vercel settings.
- Deploy.

### Netlify
- Build command: `npm run build`
- Publish directory: `dist`
- Add the Firebase environment variables.

## Note about live supermarket prices

This website stores shared manual prices. Automatic real-time Lidl/Netto/Aldi/REWE website scraping needs a separate backend/API and must follow each website's terms and technical restrictions.
