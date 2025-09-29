Invoice App – Assessment
Overview

This project is a simple invoice management app built with React based on the provided Figma design.
It demonstrates authentication, mock API integration, and real-time updates, following best practices in component structure and state management.

Features
Developed an admin dashboard and inventory system that improved small business operations and reduced manual
workload
Authentication: Signup/Login using Firebase Authentication.

Invoices:

View list of invoices.

Create a new invoice via form.

View invoice details.

Mock Backend: API calls simulated with [MSW / JSON Server] for invoices.

Realtime Updates: Invoice status updates streamed via a mock WebSocket connection.

Responsive UI: Works across desktop and mobile screens.

Tests:

Unit test: Invoice form validation.

Integration test: Login flow.

Bonus Features

Error handling for invalid routes and failed network requests.

Loading spinners when fetching or submitting invoices.

Tech Stack

React 18 + Vite 

Tailwind CSS for styling 
Firebase Authentication.

<!-- Mock Service Worker (MSW) for API simulation. -->

<!-- socket.io-client (mocked with simulated events). -->

Jest + React Testing Library for testing.

Project Structure
src/
  components/   // Reusable UI components
  pages/        // Top-level screens
  hooks/        // Custom hooks
  services/     // API + socket logic
  tests/        // Unit & integration tests

Setup Instructions

Clone the repo:

git clone https://github.com/<your-username>/invoice-app.git
cd invoice-app


<!-- Install dependencies:

npm install


Add Firebase credentials in .env:

VITE_FIREBASE_API_KEY=xxxx
VITE_FIREBASE_AUTH_DOMAIN=xxxx -->


Run the app:

npm run dev


Run tests:

npm test

<!-- Assumptions & Limitations

The backend is mocked; no persistent database.

Realtime updates are simulated (not connected to a live server).

Only key flows are tested due to time constraints. Given more time, I’d expand test coverage and productionize the socket server.



