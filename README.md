<p align="center">
    <br/>
    <a href="https://github.com/bslockhart/brians-text-editor">	
        <img src="https://imgur.com/GnWkBAS.png" alt="Brian's Text Editor">
    </a>
</p>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

The task is to build a text editor that runs in the browser. The following app is a single-page application that meets the PWA criteria. Additionally, it features a number of data persistence techniques that serve as redundancies in case one of the options is not supported by the browser. The application also functions offline.

This text editor was built with an existing application and implements methods for getting and storing data to an IndexedDB database, using a package called idb, which is a lightweight wrapper around the IndexedDB API. It also features a number of methods that are useful for storing and retrieving data, and is used by companies like Google and Mozilla.

## Table of Contents

- [Tools](#tools)
- [Mock Up](#Mock-Up)
- [Instructions](#Instructions)
- [User Story](#User-Story)
- [Acceptance Criteria](#Acceptance-Criteria)
- [Technical Acceptance Criteria](#Technical-Acceptance-Criteria)
- [Deployment](#Deployment)
- [Application Quality](#Application-Quality)
- [Repository Quality](#Repository-Quality)
- [Submission](#Submission)

## Tools

- Webpack
- HTMLWebpackPlugin
- idb
- Workbox

## Mock Up

![Text Editor](./assets/images/00-demo.gif)

## Instructions

1. Clone the main project, then open the cloned file.
2. Make sure you are in the main project folder using the 'cd' command.
3. Open command prompt and run: npm install
4. To use offline, open in browser and hit the "install" button in top left corner.

## User Story

```text
AS A developer
I WANT to create notes or code snippets with or without an internet connection
SO THAT I can reliably retrieve them for later use
```

## Acceptance Criteria

```text
GIVEN a text editor web application
WHEN I open my application in my editor
THEN I should see a client-server folder structure
WHEN I run `npm start` from the root directory
THEN I find that my application should start up the back end and serve the client
WHEN I run the text editor application from my terminal
THEN I find that my JavaScript files have been bundled using webpack
WHEN I run my webpack plugins
THEN I find that I have a generated HTML file, service worker, and a manifest file
WHEN I use next-gen JavaScript in my application
THEN I find that the text editor still functions in the browser without errors
WHEN I open the text editor
THEN I find that IndexedDB has immediately created a database storage
WHEN I enter content and subsequently click off of the DOM window
THEN I find that the content in the text editor has been saved with IndexedDB
WHEN I reopen the text editor after closing it
THEN I find that the content in the text editor has been retrieved from our IndexedDB database
WHEN I click on the Install button
THEN I download my web application as an icon on my desktop
WHEN I load my web application
THEN I should have a registered service worker using Workbox
WHEN I register a service worker
THEN I should have my static assets precached upon loading along with subsequent pages and static assets
WHEN I deploy to Heroku
THEN I should have proper build scripts for a webpack application
```

## Technical Acceptance Criteria

- Application uses IndexedDB to create an object store and includes both GET and PUT methods.
- Application works without an internet connection.
- Application automatically saves content inside the text editor when the DOM window is unfocused.
- Application is bundled with webpack.
- Application has created a service worker with Workbox that caches static assets.
- Application uses Babel in order to use async / await.
- Application has a generated manifest.json using the WebpackPwaManifest plug-in.
- Application can be installed as a Progressive Web Application.

## Deployment

- Application is deployed to Heroku at live URL with build scripts.
- Application loads with no errors.
- Application’s GitHub URL is submitted.
- GitHub repo contains application code.

## Application Quality

- Application user experience is intuitive and easy to navigate.
- Application user interface style is clean and polished.
- Application resembles the mock-up functionality provided in the Challenge instructions.

## Repository Quality

- Repository has a unique name.
- Repository follows best practices for file structure and naming conventions.
- Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.
- Repository contains multiple descriptive commit messages.
- Repository contains a quality README file with description, screenshot, and link to deployed application.

### Submission

- Date Submitted: December 7, 2022
- You are required to submit BOTH of the following for review:

1. The URL of the functional, deployed application:
2. The URL of the GitHub repository. Give the repository a unique name and include a README describing the project: https://github.com/bslockhart/Brians-Text-Editor
