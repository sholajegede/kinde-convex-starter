# Kinde-Convex File Sharing App: Part 1
A fully pre-configured Next.js application to kickstart your development with Kinde and Convex, enabling secure authentication, real-time data syncing, and role-based access control (RBAC). This app serves as a foundational template for building scalable, secure, and user-friendly file-sharing applications.

## 🚀Features
- Passwordless Authentication: Enable seamless logins with Kinde's secure authentication services.
- Social Login Integration: Support for Google, Facebook, and GitHub sign-ins.
- Real-Time Data Management: Powered by Convex, ensuring real-time updates between the frontend and backend.
- Role-Based Access Control (RBAC): Assign and manage roles like Admins and Members to restrict or enable access to features.
- Webhook Integration: Sync user authentication events to your database in real-time.
- Pre-Styled UI Components: Built using Shadcn and TailwindCSS for a responsive and intuitive design.

## 🎓What You'll Learn
This repository demonstrates how to:
- Integrate Kinde into your Next.js project for authentication.
- Configure Convex for database and backend API functions.
- Implement RBAC for secure feature control.
- Use webhooks to synchronize user data and events.
- Protect routes with middleware.
- Fetch and display user data dynamically.

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

## 🛠️ Prerequisites
**Environment Variables**

Update the `.env.local` file with your **Kinde** and **Convex** credentials:
```
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

## 🛡️ Role-Based Access Control (RBAC)
This app demonstrates RBAC with the following roles:
- **Admin**: Full control, including deleting files.
- **Member**: Restricted access, such as uploading files only.
RBAC is configured via Kinde's dashboard, where you can assign roles and permissions to users.

## 🌐 Deploy on Vercel
The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

## 📝 What's Next?
**Part 2: Advanced RBAC Implementation**
In the next installment, learn how to:
- Configure advanced permissions for granular control.
- Implement RBAC checks on API endpoints and the frontend.
- Build a production-grade file-sharing application.

## 💬 Feedback
We’d love to hear from you!
Have thoughts, questions, or suggestions? Drop a comment below or reach out directly on GitHub. Let’s build something amazing together! 🚀


