# TicketHub — React + Vite

A student demonstration project for online movie and event ticket booking. Built with React functional components, Vite, and browser Local Storage.

## Modules
- **Authentication module** (`src/modules/Auth.jsx`): user signup/login, validation, persistent session.
- **User module** (`src/modules/User.jsx`): browse/filter movies and events, view own bookings/tickets.
- **Admin module** (`src/modules/Admin.jsx`): dashboard metrics, add/edit/delete events, view bookings.
- **Booking module** (`src/App.jsx`): select seats and create a digital demo ticket.
- **Shared components/storage** (`src/components`, `src/storage.js`): navigation and Local Storage helpers.

## Run locally
Requires Node.js 20.19+ or 22.12+.

```bash
npm install
npm run dev
```
Open the URL printed by Vite (usually http://localhost:5173).

## Build and check
```bash
npm run lint
npm run build
npm run preview
```

## Demo accounts
- Admin: `admin@tickethub.com` / `admin123`
- User: choose Sign Up and create a new account.

Accounts, events, bookings and current login are saved in the browser's Local Storage. Data is browser/device-specific. This is suitable for a classroom demonstration only: passwords are not securely hashed, there is no backend/database, no email verification, no server-side authorization, and no real payment gateway. The booking confirmation is a simulated demo flow, not proof of payment.

## GitHub
Create an empty GitHub repository, then run these commands from this project folder:

```bash
git init
git add .
git commit -m "TicketHub React Vite project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

## Vercel deployment
1. Push the project to GitHub.
2. Sign in at https://vercel.com and choose **Add New → Project**.
3. Import the TicketHub GitHub repository.
4. Framework preset: **Vite**; Build command: `npm run build`; Output directory: `dist`.
5. Click **Deploy** and wait for the deployment to finish.
6. Open the generated `*.vercel.app` URL and test signup, login, user booking, and admin login.

No environment variables are required. Vercel deployment and GitHub push require your own account authorization; this package is prepared but not published on your behalf.
