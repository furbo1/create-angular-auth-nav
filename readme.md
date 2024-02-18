# Create a Fullstack* Angular Auth Navigation Project

This CLI tool, `npx create-angular-auth-nav` provides a template for quickly setting up an Angular application with register/login functionality, utilizing Express, Passport and Bcrypt for encryption and basic navigation between pages. It incorporates [TailwindCSS](https://tailwindcss.com/) for its modern and responsive styling.

![Register Page](/assets/register.jpg "Register page")
![Login Page](/assets/login.jpg "Login Page")

## Features

- Register/Login functionality with basic client-side validation.
- Passport.js for handling user authentication with flexible and modular middleware for Node.js.
- Bcrypt for password security with automatic salt generation and hashing to protect against attacks.
- Navigation bar with access to Home, About, and Contact pages.
- User credentials stored in local storage for demonstration purposes, with the option to connect to any database of choice.
- TailwindCSS integration for a sleek, responsive user interface design.

## Using the Template

To get started with this template, you can clone the repository or use a CLI tool to create a new project:

`npx create-angular-auth-nav`


## Installation and Running the Project

This project is organized into separate frontend and backend directories, promoting a clean separation of concerns.

### Running both frontend and server from the root folder

This requires the "concurrently" package:

- Run `npm install` to install all dependencies.
- Execute `npm start` to boot up both frontend and backend servers.
- Access the application at http://localhost:4200 (default Angular port).
- Register and login with user credentials, which are stored in local storage (switch to a database for production use).

### Running frontend and backend separately

#### Backend Setup

- Navigate to the backend directory with `cd backend`.
- Install dependencies with `npm install`.
- Start the server with `node server.js` or `nodemon server.js`.

#### Frontend Setup

- Navigate to the frontend directory with `cd frontend`.
- Install dependencies with `npm install`.
- Start the Angular server with `ng serve`.
- Access the application at http://localhost:4200.
- Register a user, credentials will be stored in local storage this should not be used in production, for production connect to any database of your choice
- Login with the user you just registered and modify the app as you desire

## Customization

### Database Integration

While user credentials are stored in local storage for demonstration, production applications should use a secure database. The backend can be modified to integrate with databases such as MongoDB, PostgreSQL, Firebase, etc.

### TailwindCSS Customization

Customize the appearance of the frontend by modifying the `tailwind.config.js` file. Refer to the [official TailwindCSS documentation](https://tailwindcss.com/docs) for detailed instructions.

## Contribution

Contributions are welcome! Feel free to suggest improvements, report issues, or submit pull requests on GitHub.

## License

This template is open source, licensed under the MIT License. See the LICENSE file for more details.

```
CREATE-ANGULAR-AUTH
├── backend
│ ├── index.js
│ ├── package-lock.json
│ └── package.json
└── frontend
├── .angular
├── .vscode
├── node_modules
├── src
│ ├── app
│ │ ├── components
│ │ │ ├── about
│ │ │ ├── contact
│ │ │ ├── footer
│ │ │ ├── header
│ │ │ ├── home
│ │ │ ├── login
│ │ │ ├── navigation
│ │ │ └── register
│ │ ├── guards
│ │ │ └── auth.guard.ts
│ │ ├── services
│ │ ├── app-routing.module.ts
│ │ ├── app.component.html
│ │ ├── app.component.spec.ts
│ │ ├── app.component.ts
│ │ └── app.module.ts
│ ├── assets
│ ├── environments
│ │ ├── environment.ts
│ ├── index.html
│ ├── main.ts
│ └── styles.css
├── .editorconfig
├── .gitignore
├── angular.json
├── package-lock.json
├── package.json
├── README.md
├── tsconfig.app.json
├── tsconfig.json
└── tsconfig.spec.json
```

## App 
![Home Page](/assets/home.jpg "Home Page")
![Home Page](/assets/about.jpg "About Page")
![Home Page](/assets/contact.jpg "Contact Page")
![Register Page](/assets/register.jpg "Register page")
![Login Page](/assets/login.jpg "Login Page")

Disclaimer:

This project, [create-angular-auth-nav](https://www.npmjs.com/package/create-angular-auth-nav), is provided as-is without any warranty of any kind, either express or implied, including but not limited to the implied warranties of merchantability, fitness for a particular purpose, or non-infringement. The use of [create-angular-auth-nav](https://www.npmjs.com/package/create-angular-auth-nav) is entirely at your own risk. The author(s) or contributors shall not be liable for any damages, including but not limited to direct, indirect, incidental, special, consequential, or punitive damages arising out of or in connection with your access to, use of, or reliance on this project. By using [create-angular-auth-nav](https://www.npmjs.com/package/create-angular-auth-nav), you agree to this disclaimer and acknowledge that the project is offered freely for use, modification, and distribution under its specified MIT license, without any obligation for support, maintenance, or updates.

*Database is missing from this app as this depends on user's needs.
