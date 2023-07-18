[![License: MIT license](https://img.shields.io/badge/License-MIT_license-success)](https://opensource.org/licenses/MIT)    
![Project status](https://img.shields.io/badge/Status-Complete-success)

# CBC Week 19 Challenge: Text Editor

## General Information
This is the week 19 challenge for the UC Berkeley Coding Bootcamp.  The goal is to create a Progressive Web App (PWA) that used IndexedDB to store data locally when the user is offline.  To do this, the app uses a manifest created from a JSON file and a service worker to cache the data.  When the user is offline, the app uses IndexedDB to store the data locally.  When the user is back online, the app uses the service worker to sync the data with the server.

## Table of Contents
* [General Information](#general-information)
* [Main Technologies Used](#technologies-used)
* [Installation](#installation)
* [Usage](#usage)
* [Credits](#credits)
* [Contact](#contact)
* [License](#license)
* [How to Contribute](#how-to-contribute)

## Main Technologies Used
* [node.js v18.12.1](https://nodejs.org/en) -  A scalable server-side JavaScript runtime;
* [express v4.18.2](https://www.npmjs.com/package/express) - Web application framework for building server-side applications.
* [nodemon v2.0.22](https://www.npmjs.com/package/nodemon) - Development tool for automatically restarting the server during code changes.
* [concurrently v6.2.1](https://www.npmjs.com/package/concurrently) - Development tool for running multiple processes concurrently.
* [webpack v5.51.1](https://www.npmjs.com/package/webpack) - Development tool for bundling JavaScript files for use in the browser.
* [babel v7.15.8](https://www.npmjs.com/package/babel) - Development tool for transpiling JavaScript files for use in the browser.
* [css-loader v6.2.0](https://www.npmjs.com/package/css-loader) - Development tool for loading CSS files.
* [Heroku](https://www.heroku.com/) - Cloud platform for deploying applications.

## Installation
### Prerequisites
* [Node.js](https://nodejs.org/en/)
* [Git](https://git-scm.com/)

### Deployed Application
The application is deployed on Heroku at https://jdempe-text-editor-a3919d1f68df.herokuapp.com/.

### Local Installation
If you would prefer to see a local version of the site, follow the steps below:

1. Clone the [repository](https://github.com/JDempe/bootcamp-19-text-editor) to your local machine.
2. Navigate to the root directory of the cloned repository in your terminal.
3. Run `npm run install` to install the dependencies.
4. Run `npm run build` to build the front-end files.
5. Start the server by running `npm start:dev`.
6. Navigate to http://localhost:3001 in your browser to view the site.

## Usage
To use the app, type in the text editor.  WHen the text editor is not focused (you click elsewhere) the text is saved to the database.  When you load the page, the text is loaded from the database.  If you are offline, the text is saved to IndexedDB and then synced with the server when you are back online.

To install the app, click the install button in the address bar of your browser.  This will install the app on your device.  You can then open the app from your device's home screen.

## Credits
### Resources
#### Class Resources
The starter code for this project was provided by the UC Berkeley Coding Bootcamp program.

#### Troubleshooting
- https://github.com/arthurbergmz/webpack-pwa-manifest/issues/149
- https://developer.mozilla.org/en-US/docs/Web/API/Window/beforeinstallprompt_event
- https://stackoverflow.com/questions/65245185/new-to-webpackautoprefix-problem-with-webpack-manifest-plugin
- https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers

## Contact
### Collaborators
- Joshua Dempe - [JDempe](https://github.com/JDempe)

## License
This project is open source and available under the [MIT](./LICENSE) license.

## How to Contribute
Looking to contribute?  Find out how at https://github.com/JDempe/bootcamp-19-text-editor.