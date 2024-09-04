# Job Application App

This is a Job Application App built using React, Vite, and Tailwind CSS. The app allows users to apply for jobs and manage their applications. However, please note that the app does not display job listings because it is running on a local JSON server, and there is no backend setup.

## Features

- **Job Application Management**: Allows users to apply for jobs and track their applications.
- **Modern UI**: Built with Tailwind CSS, providing a responsive and clean interface.
- **React Router Integration**: For smooth navigation between different pages.
- **Local JSON Server**: Used to simulate API calls and data storage.

## Tech Stack

- **React**: A JavaScript library for building user interfaces.
- **Vite**: A fast development build tool and dev server for modern web projects.
- **Tailwind CSS**: A utility-first CSS framework for designing custom UI components.
- **React Icons**: For easy access to popular icons.
- **React Router Dom**: For managing routes in the app.
- **React Spinners**: For loading spinners to indicate loading states.
- **React Toastify**: For showing notifications.

## Keep in Mind

- The app does not display job lists because it is running on a local JSON server, and no backend is created.

## Installation and Setup

Follow these steps to set up and run the project locally:

### Installation Steps

1. **Create a Vite project**:

   ```bash
   npm create vite@latest
   ```

2. **Navigate to the project directory**:

   ```bash
   cd JobApplicationApp
   ```

3. **Install project dependencies**:

   ```bash
   npm install
   ```

4. **Install Tailwind CSS and related tools**:

   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   ```

5. **Modify the Tailwind CSS configuration**:

   In `tailwind.config.js`, update the content paths and extend the theme:

   ```javascript
   /** @type {import('tailwindcss').Config} */
   export default {
     content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
     theme: {
       extend: {
         fontFamily: {
           sans: ["Roboto", "sans-serif"],
         },
         gridTemplateColumns: {
           "70/30": "70% 28%",
         },
       },
     },
     plugins: [],
   };
   ```

6. **Modify `index.css`**:

   Add the following Tailwind directives to your `index.css`:

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

7. **Install React Icons**:

   ```bash
   npm i react-icons
   ```

8. **Install React Router DOM**:

   ```bash
   npm install react-router-dom
   ```

9. **Install JSON Server**:

   ```bash
   npm i -D json-server
   ```

10. **Modify `package.json`**:

    Update the necessary scripts or configurations in your `package.json`.

11. **Install React Spinners**:

    ```bash
    npm i react-spinners
    ```

12. **Install React Toastify**:

    ```bash
    npm install react-toastify --legacy-peer-deps
    ```

13. **Build the project**:

    ```bash
    npm run build
    ```

14. **Preview the project**:

    ```bash
    npm run preview
    ```

### Commands

1. **Start the JSON server**:

   ```bash
   npm run server
   ```

   This command runs the JSON server to simulate API requests for job data.

### New Commands

1. **Check outdated packages**:

   ```bash
   npm outdated
   ```

## Usage

- Run the project locally by following the steps above.
- Use the app to manage job applications.
- Make sure to start the JSON server to simulate API data.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- **React** for the powerful UI components.
- **Vite** for the fast development and build tool.
- **Tailwind CSS** for the modern design utility.
