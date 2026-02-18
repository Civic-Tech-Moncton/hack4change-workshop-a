# Hack4Change Workshop Client Repository
This is the sample client repository for the first Hack4Change workshop. Combined with one of the Hack4Change server applications, you can use this client as a basis to build your own full stack web application.

# Getting Started
To start working with this client project, do the following:

- Download Node.js with npm from https://nodejs.org/en/download and follow the instructions to install it. This project was created using Node version 22.22.0, but should work with any recent version of Node.
- Copy this folder to a convenient location, ie. a "project" folder.
- From this directory, run the following command in a command line: `npm install`. This will install all of the project's dependencies.
- Use the scripts listed below to run and test the client.

# Scripts
You can run the following commands from a command line in this directory:

- `npm run dev` will run a development server. When you run the command, it'll provide you with a localhost address that you can use to access the client.
- `npm run build` will compile the client and send its output to a `dist` folder. The folder will contain the HTML page and the assets required to run it.
- `npm run test` will run any unit tests that you've implemented. By convention, unit tests are stored alongside the files that they are testing and end with ".spec.ts". The test runner will continue to run and monitor files for changes, so you can leave this running while developing your application in order to automatically re-run tests as you update your code.
- `npm run e2e` will run any end-to-end tests that you've implemented. These tests are stored in the "tests" directory, and will run the full UI application in the browser. You can use this to automatically test any functionality that you've implemented and make sure that it works across all major browsers.

# Layout
The base directory for the web client contains all of the configuration files for the project, as well as this README file. It also contains `index.html`, the entry point for the application.

The `public` directory contains any static files served with the web client. To start with, it contains an SVG file for the application's favicon.

The `src` directory contains all of the code and stylesheets for the application. The root of the directory contains a handful of sample components and files, and an `api` folder contains files that access the API. Unit tests are also contained in this folder alongside the files that they test, using the `*.spec.ts` naming convention.

The `tests` directory contains end-to-end tests, which can be used to automate testing of the application when it is running in a browser with a server providing its data.

# Frameworks and Tools
This application is built using the Typescript programming language. Documentation for the language and its features is available at https://www.typescriptlang.org/docs/handbook/intro.html.

The build process and dev server use the Vite build tool. If you want to adjust the build process, you can find more information on how to use the tool at https://vite.dev/guide/.

Unit test support is provided by the Vitest testing framework. For more information on how to write and run tests using this framework, see https://vitest.dev/guide/.

End-to-end testing is done via Playwright. Documentation on Playwright testing is available at https://playwright.dev/docs/intro.
