Installation Guide
Step 1: Create a New Vite Project
Install Vite (if not already installed):

bash
npm create vite@latest
Choose the following options when prompted:

Project name: paste
Framework: React
Variant: JavaScript or TypeScript (choose based on your preference).
Navigate to your project folder:

bash
cd paste
Step 2: Install and Configure Tailwind CSS
Install Tailwind CSS and its dependencies:

bash
npm install -D tailwindcss postcss autoprefixer
Initialize Tailwind CSS configuration:

bash
npx tailwindcss init
This creates a tailwind.config.js file.

Configure Tailwind to scan your files by updating tailwind.config.js with:

js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    './index.html',
    './src/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
Add Tailwind’s directives to your main CSS file (src/index.css or src/main.css):

css
@tailwind base;
@tailwind components;
@tailwind utilities;
Step 3: Install Project Dependencies
To ensure all necessary dependencies are installed, run:

bash
npm install
Step 4: Run the Project
Start the development server with:

bash
npm run dev
Your project will now be accessible at http://localhost:5173.
 
 
