# Users and Authentication Example App
This example demonstrates how to add users and authentication to a basic file sharing application. It uses [Kinde](https://kinde.com) for authentication.

Users are initially presented with **Get started** and **Log in** buttons. After user's sign up, their information is sent through a webhook and persisted to a `users` table on Convex. Users can also sign up and log in with passwordless authentication, social logins and have access to role-based access control.

## 🛠️ Prerequisites
Before you begin, ensure you have the following:
- Node.js installed on your computer.
- Familiarity with TypeScript, React, and Next.js.
- Free accounts on [Kinde](https://kinde.com) and [Convex](https://www.convex.dev).

## 🔧 Getting Started
1. Clone the Repository
```bash
git clone https://github.com/sholajegede/kinde-convex-starter.git
cd kinde-convex-starter
```
2. Install Dependencies
```bash
npm install
# or
yarn install
# or
bun install
```
3. Run the Development Server
```bash
npm run dev
# or
yarn dev
# or
bun run dev
```
Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

## 🛠️ Setting up your own Kinde instance
Follow the instructions in [https://docs.convex.dev/auth/kinde#get-started](https://docs.convex.dev/auth/kinde#get-started) to obtain your **Kinde** and **Convex** credentials.

Update the `.env.local` file with your obtained credentials:
```
# Deployment used by `npx convex dev`
CONVEX_DEPLOYMENT=your_convex_deployment
NEXT_PUBLIC_CONVEX_URL=https://your_convex_deployment.convex.cloud
NEXT_PUBLIC_CONVEX_HTTP_URL=https://your_convex_deployment.convex.site

KINDE_CLIENT_ID=your_kinde_client_id
KINDE_CLIENT_SECRET=your_kinde_client_secret
KINDE_ISSUER_URL=https://your_kinde_subdomain.kinde.com
KINDE_SITE_URL=http://localhost:3000
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_POST_LOGIN_REDIRECT_URL=http://localhost:3000/dashboard

NEXT_PUBLIC_CONVEX_URL=your_convex_public_url
NEXT_PUBLIC_CONVEX_HTTP_URL=your_convex_http_url
```
**Database Schema**

The schema is pre-configured to store user data, including email, roles, and preferences.

## 📂 Project Structure
- **/app**: Next.js application files.
- **/convex**: Backend functions, schema, and API handlers for Convex.
- **/providers**: Custom providers for Kinde and Convex integration.
- **/components**: Reusable UI components styled with TailwindCSS and Shadcn.
- **middleware.ts**: Middleware to protect routes.

## 💬 Feedback
We’d love to hear from you!
Have thoughts, questions, or suggestions? Drop a comment below or reach out directly on GitHub. Let’s build something amazing together! 🚀


