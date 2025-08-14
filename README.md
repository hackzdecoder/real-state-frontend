Real Estate Listings Web Application – Frontend Setup
1. Project Overview
The frontend of the Real Estate Listings Web Application is built using React, TypeScript, and Material-UI (MUI). It provides a responsive and mobile-first interface for users to browse, search, and view real estate listings. Admin users can manage listings through full CRUD operations.
The frontend interacts with the backend API hosted on Node.js + Express and uses Supabase for authentication and storage.

Project link: https://real-state-frontend-jcde.onrender.com
________________________________________
2. Prerequisites
Before setting up the frontend, ensure you have the following installed on your computer:
•	Node.js version 16 or above
•	npm version 8 or above, or yarn
•	Git for version control
•	A code editor such as Visual Studio Code
________________________________________
3. Cloning the Repository
1.	Open a terminal or command prompt.
2.	Run the command to clone the project repository from GitHub: 
Frontend Repo: https://github.com/hackzdecoder/real-state-frontend.git
Backend Repo: https://github.com/hackzdecoder/real-state-backend.git
3.	Navigate to the frontend folder, usually named app.
________________________________________
4. Installing Dependencies
1.	Open the frontend folder in your terminal.
2.	Install all required dependencies for the frontend, including React, TypeScript, and Material-UI.
3.	Ensure the installation completes without errors.
Use  npm install for Both Frontend & Backend
________________________________________
5. Starting the Development Server
1.	In the frontend folder, start the development server.
2.	The application will open in your default browser at http://localhost:3000.
3.	Any changes made to the frontend code will automatically refresh the browser.
________________________________________
6. Building for Production
1.	Create an optimized production build of the frontend.
2.	The build will generate a folder with static assets ready for deployment on platforms like Vercel or Netlify.
3.	Configure environment variables on the hosting platform instead of using a local .env file.
________________________________________
7. Running with Backend
•	Ensure the backend server in the api folder is running on the URL specified in your environment variables.
•	The frontend communicates with the backend for authentication, CRUD operations on listings, and image uploads via Supabase storage.
________________________________________
8. Deployment Notes
•	Recommended hosting platforms: Vercel or Netlify
•	Set environment variables on the hosting platform dashboard for production use
•	Use HTTPS and secure your API keys when deploying
________________________________________
9. Environment Variables (.env)
Create a .env file in your backend folder (api) with the following details:
•	SUPABASE_URL: Your Supabase project URL from your Supabase dashboard
•	SUPABASE_ANON_KEY: Your Supabase anon/public API key for client-side requests or service key if backend
•	JWT_SECRET: JWT secret or public key to verify Supabase JWT tokens (optional)
•	PORT: Server port for your Node backend, for example 5000
•	Optional: STORAGE_PROVIDER to indicate local, Supabase, or S3 for image uploads
•	Optional: STORAGE_PATH to indicate the upload folder, e.g., uploads/
Example values can be filled according to your setup.
________________________________________
10. Test Credentials
Admin User:
•	Username: anonymous_admin
•	Password: admin123
Regular User:
•	Username: anonymous_user
•	Password: anonymoususer123
________________________________________
GitHub Setup for Real Estate Listings Web Application
1. Repository Creation
1.	Go to GitHub and create a new repository for your project, for example, real-estate-app.
2.	Initialize the repository with a README file (optional).
________________________________________
2. Organize Local Project
1.	Ensure your local project folder has the following structure:
•	app for the frontend React application
•	api for the backend Node.js + Express application
2.	Add sensitive files such as .env to .gitignore in both app and api folders.
________________________________________
3. Git Clone and Push Procedure
1.	Open a terminal in the project root.
2.	Clone the repository using: https://github.com/hackzdecoder/real-state-frontend.git & : https://github.com/hackzdecoder/real-state-backend.git 
3.	Navigate to the project folder.
4.	After making changes, stage files using: git add .
5.	Commit changes with a message: git commit -m "Your descriptive commit message"
6.	Push commits to GitHub: git push origin main (or your working branch)
________________________________________
4. Branching and Feature Development
1.	Create separate branches for each new feature or task, for example, feature/user-auth.
2.	Work on the feature in the branch and commit regularly with descriptive messages.
3.	Merge completed features into the main branch using pull requests.
________________________________________
5. Collaboration
1.	Add collaborators to the repository on GitHub.
2.	Pull the latest changes from the main branch before starting new work.
3.	Resolve merge conflicts carefully when they arise.
________________________________________
6. Notes
•	Keep .env files and other sensitive data out of GitHub
•	Use clear commit messages and maintain separate branches for features and bug fixes
•	Regularly push changes to keep the remote repository up to date

