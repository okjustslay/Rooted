Project Name: Rooted - Emotional Regulation Prototype Application (please open on max screen size)

Overview

This README file provides an overview of the folder structure and the contents of the project package for the "Rooted" prototype application. 
This document will guide you through the various files and directories included in the submission.
When the package has been extracted please read the INSTRUCTIONS.pdf for a full guide on running the prototype.

There are 2 files in the "happy app vf.zip/.rar" folder once extracted there are 2 folders

├── happy_app//          - This is the backend of the prototype 
├── happy_app_front//    - This is the frontend of the prototype 

happy_app - Backend - The structure of all the main backend folders (please note for a matter of simple viewing, not all folders have been explicitly mentioned, only those that 						 are important to the development of the product package). 
Please note the main files and their extensions will be explained so you, the viewer needs to understand the behaviour of certain files. 
This can be handy when looking at code and understanding files and directories and how they are connected.

happy_app/                           - The root directory containing the entire backend code for the "Rooted - Happy Moment" application.
├── happy_app/
│   ├── .env                       * .env Environment variables file for storing configuration variables such as database credentials, secret keys, and other settings.
│   ├── core/                      * core/ contains the core functionality of the application, including user management and common utilities.
│   │   ├── _pycache_/            - pycache/: Directory containing compiled Python bytecode files.
│   │   ├── migrations/           - migrations/: Directory containing database migration files for the core app.
│   │   ├── users/                - users/: Contains files related to user management.
│   │   │   ├── _pycache_/         - pycache/: Directory containing compiled Python bytecode files.
│   │   │   ├── serializers.py     - serializers.py: Defines how data is converted between Python objects and JSON.
│   │   │   ├── urls.py            - urls.py: URL configurations for the user-related endpoints.
│   │   │   ├── views.py           - views.py: Views/functions handling HTTP requests for user-related actions.
│   │   ├── __init__.py           - init.py: Marks the directory as a Python package.
│   │   ├── admin.py              - admin.py: Configuration for the Django admin interface.
│   │   ├── apps.py               - apps.py: Configuration for the core application.
│   │   ├── models.py             - models.py: Data models for the core application.
│   │   ├── tests.py              - tests.py: Automated tests for the core application.
│   │   ├── views.py              - views.py: Views/functions handling HTTP requests for the core application.
│   ├── happy_app/
│   │   ├── __init__.py
│   │   ├── settings.py           - settings.py: Configuration settings for the Django project.
│   │   ├── urls.py               - urls.py: URL declarations for the Django project.
│   │   ├── wsgi.py               - wsgi.py: Entry point for WSGI-compatible web servers to serve the project.
│   │   └── asgi.py               - asgi.py: Entry point for ASGI-compatible web servers
│   │   ├── templates/rest_framework * templates/: Directory for storing HTML templates.
│   │   │   ├── api.html                                           
│   │   └── _pycache_/
│   ├── media/                     * The media files used within the database, it consist of image types, video types
│   ├── moment/                    * moment/ contains the functionality related to moments within the application. moment cant be reused and acts as its own application
│   │   ├── __init__.py
│   │   ├── admin.py
│   │   ├── apps.py               - apps.py: Configuration for the moment application.
│   │   ├── models.py             - models.py: Data models for moments.
│   │   ├── serializers.py        - serializers.py: Defines how data is converted between Python objects and JSON for moments.
│   │   ├── tests.py              - tests.py: Automated tests for the moment application.
│   │   ├── urls.py               - urls.py: URL configurations for the moment-related endpoints.
│   │   ├── views.py              - views.py: Views handling HTTP requests for moment-related actions.
│   │   ├── _pycache_/
│   │   └── migrations/           * migrations/: Directory containing database migration files for the moment app.
│   ├── .gitignore                 - .gitignore specifies files and directories that should be ignored by Git version control.
│   ├── db.sqlite3                 - db.sqlite3 SQLite database file for the project, containing all the data for the application.
│   ├── manage.py                  - manage.py Django's command-line utility for administrative tasks, such as running the server, making migrations, and managing users.
│   ├── requirements.txt           - requirements.txt List of Python dependencies required for the backend.
├── README.md            - README.md file providing an overview of the prototype project, installation instructions, and other relevant information.




happy_app_front - Frontend - The structure of all the main frontend folders (please note for a matter of simple viewing, not all folders have been explicitly mentioned, only those that are important to the development of the product package). 
Please note the main files and their extensions will be explained so you, the viewer needs to understand the behaviour of certain files. This can be handy when looking at code and understanding files and directories and how they are connected and implement the overall project.

happy_app_front/                     - The root directory containing the entire frontend code for the "Rooted - Happy Moment" application.
├── happy_app_front/              
│   ├── node_modules/                 * The node_modules/ directory contains all the npm packages/dependencies required for the project. It is automatically generated when you run "npm install".             
│   ├── public/                       * public/ contains static files that are directly served by the web server. 
│   │   ├── index.html                - index.html: The main HTML file that serves as the entry point for the React application.
│   ├── src/                          * Contains the source code for the React application.
│   │   ├── App.css                   - App.css: The main CSS file for styling the main app component.
│   │   ├── App.test.tsx              - App.test.tsx: Contains tests for the App component using Jest and React Testing Library.
│   │   ├── App.tsx                   - App.tsx: The root component of the React application. tsx files support TypeScript which is a further extension of JavaScript syntax used for defining React component in React Application 
│   │   ├── index.css                 - index.css: Global CSS styles for the entire application.
│   │   ├── index.tsx                 - index.tsx: The entry point for the React application, responsible for rendering the App component.
│   │   ├── logo.svg              
│   │   ├── react-app-env.d.ts        - react-app-env.d.ts: TypeScript declaration file for the React app environment.
│   │   ├── reportWebVitals.ts        - reportWebVitals.ts: A file to measure and report web vitals for performance analytics.
│   │   ├── setupTests.ts             - setupTests.ts: Configuration file for setting up tests with Jest.
│   │   └── components/               - The components/ directory contains reusable React components.
│   │       ├── indicator/            - indicator/: Components related to indicators.
│   │            └── indicatorComponent.tsx          - IndicatorComponent is a React functional component that displays a joyride indicator.                                    
│   │       └── memory/               - memory/: Components related to memories.
│   │            └── memoryComponent.tsx             - memoryComponent represents a memory component in a vertical timeline.
│   │       └── spotify/              - spotify/: Components related to Spotify integration
│   │            └── SpotifyPlayer.tsx               - SpotifyPlayer.tsx is a React functional component that renders a Spotify player for a given track ID.
│   │            └── SpotifySearch.tsx               - SpotifySearch.tsx a React component that allows users to search for tracks on Spotify.
│   │       └── Texteditor/           - Texteditor/: Components related to the text editor functionality.
│   │            └── moduleConfig.ts                 - contains the toolbar configuration for text editor, including options for formatting text and handling image uploads..ts extensions are for creating functions, classes etc
│   │            └── react-quill-image-uploader.d.ts - enables us to upload images using react-quill-image-uploader
│   │            └── TestEditor.tsx                  - A text editor component using ReactQuill for rich text editing.
│   │       └── StreakCount/          - StreakCount/: Streaks management recording the consecutive days a user has used the app
│   │            └── StreakCount.tsx                 - A React component that allows users track their app usage in consecutive days               
│   │   └── pages/                    * pages/ Contains the main page components for the application.
│   │       ├── Articles.tsx           - Articles.tsx: Page component for displaying articles.
│   │       └── Home.tsx               - Home.tsx: Home page component. Representing the Home page of the application.
│   │       └── login.tsx              - login.tsx: Login page component. A functional component that represents a login form.
│   │       └── logout.tsx             - logout.tsx: Logout page component.
│   │       └── NewArticle.tsx         - NewArticle.tsx: Page component for creating a new article. Component for creating a new article with a form to input date, title, and content.
│   │       └── NewMoment.tsx          - NewMoment.tsx: Page component for creating a new moment. Component for creating a new moment with date, location, title, description, content, photos, videos, and a Spotify track.
│   │       └── Register.tsx           - Register.tsx: Registration page component.
│   │       └── FeedbackForm.tsx       - FeedbackForm.tsx: displays the page components for users giving feedback.
│   │   └── services/                 * services/ contains service files for API interactions and configuration.
│   │       ├── apis.ts                - apis.ts: File containing API calls and related functions. handling http requests
│   │       ├── keys.ts                - keys.ts: File containing API keys and other configuration settings.
│   ├── .env                          * .env Environment variables file for storing configuration variables.
│   ├── .gitignore                    * .gitignore specifies files and directories that should be ignored by Git version control.
│   ├── env.d.ts                      * env.d.ts TypeScript declaration file for environment variables.      
│   ├── package-lock.json             * package-lock.json automatically generated file that records the exact versions of npm dependencies installed.
│   ├── tailwind.config.js            * tailwind.config.js configuration file for Tailwind CSS.
│   ├── package.json                  * package.json contains metadata about the project and its dependencies, scripts, and other configurations.
│   ├── postcss.config.js             * postcss.config.js Configuration file for PostCSS, used for transforming styles with JavaScript plugins.
│   ├── tsconfig.json                 * tsconfig.json TypeScript configuration file, specifying compiler options and project settings.
├── README.md            - README.md an overview of the project prototype , there are installation instructions and further information 


