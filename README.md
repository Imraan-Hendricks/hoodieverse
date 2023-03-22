# Hoodieverse

Hoodieverse is a premier online destination for high-end hoodies

<br />

## Table of contents

1. [Introduction](#introduction)
   - [Framework](#framework)
   - [Design System](#design-system)
   - [Data Management](#data-management)  
   - [Testing](#testing)
   - [Payment Processing](#payment-processing)
2. [Key Technologies](#key-technologies)
   - [Design](#design)
   - [Development](#development)
   - [Testing](#testing)      
3. [NPM Scripts](#npm-scripts)  
4. [Usage](#usage)
   - [Requirements](#requirements)
   - [Environment Variables](#environment-variables)
   - [Setup](#setup)
   - [Development](#in-development)
   - [Production](#in-production)

<br />

### Introduction
Hoodieverse is a premier online destination that offers an unparalleled shopping experience for fashion-forward individuals who demand the best in high-end hoodies.

#### Framework
Hoodieverse is built using the latest release of Next.js which includes exciting features such as React server components, data fetching, route handlers, metadata, layouts, suspense, and error boundaries. These features enable Hoodieverse to deliver lightning-fast performance, load data more efficiently and produce a seamless user experience. 

#### Design System
To build a custom UI design system, Hoodieverse leverages tailwindCSS and Storybook. These technologies allow for rapid prototyping, efficient styling, and easy documentation of UI components. The design system is inspired by the atomic design principles. This means that the UI components are designed and organized based on their atomic nature, starting from the smallest building blocks and gradually combining them to create larger components. 

By following this approach, the design system is structured in a way that makes it easy to maintain, scale, and reuse components across different applications and projects. Additionally, atomic design principles allow for a more systematic and consistent approach to UI design, resulting in a cohesive and user-friendly interface.

#### Data Management
Data management is a crucial aspect of an e-commerce site, and Hoodieverse relies on MongoDB with Mongoose for data management, which is a flexible NoSQL database that simplifies data modeling and allows for seamless scalability. React Query is used for data synchronization, which allows the site to update data in real-time and provide users with the most up-to-date information. 

In addition Hoodieverse uses zod for data validation to ensure that all data entered into the system meets the necessary requirements and constraints, reducing the risk of errors and improving the overall reliability of the site.

#### Testing
To ensure high-quality code, Hoodieverse uses Jest and Supertest for unit and integration testing. These testing frameworks allow developers to catch bugs and errors early on in the development process, which saves time and money down the line.

End-to-end testing is handled by Cypress, which automates testing of the site's functionality and ensures that everything is working as intended. This is essential to provide users with a seamless experience and to prevent any issues that could cause frustration or loss of sales.

#### Payment Processing
Payments are processed through Yoco, and the site offers cart functionality to ensure a seamless checkout experience. By providing users with a simple and intuitive checkout process, Hoodieverse ensures that users can easily purchase the high-end hoodies they desire.

<br />

### Key Technologies:

#### Design:
- Storybook: A frontend workshop for building UI components and pages in isolation.
- Tailwindcss: A utility-first CSS framework.

#### Development:
- Next.js: An open-source React front-end development web framework.
- Mongoose: MongoDB object modeling for Node.js.
- React Query: Performant and powerful data synchronization for React.
- TypeScript: A strongly typed programming language that builds on JavaScript.
- Zod: TypeScript-first schema validation with static type inference.

#### Testing:
- Cypress: Front end testing tool for web applications.
- Jest: A Javsacript testing framework built on top of Jasmine.
- SuperTest: A high-level abstraction for testing HTTP.

<br />

### NPM Scripts:

In the root directory, you can run:

- `npm run build` - builds the application for production.
- `npm run dev` - starts the application in development mode.
- `npm run start` - starts the application in production mode.
- `npm run cypress:component` - launches component tests.
- `npm run cypress:e2e` - launches end-to-end tests.
- `npm run cypress:open` - opens the cypress launchpad.
- `npm run jest:unit` - launches unit tests.
- `npm run jest:watch` - launches unit tests in interactive mode.
- `npm run storybook` - start Storybook locally and output the address.

<br/>

### Usage:

Clone this repository and follow the instructions below to set up your environment and run the project locally. Instructions are also provided for production usage.

#### Requirements:
To get started, ensure that you have Node.js version 16.8.0 or higher installed.

#### Environment Variables:
To set up the required environment variables, create a .env.development.local file and .env.test.local file in the root directory of the project. A sample of these files is provided in the expected location for reference. It should be noted that in a production environment, environment variables should be set up on the host server.

Cypress requires the specification of environment variables, which should be included in a file named cypress.env.json, situated in the root directory of the project. A sample of this file is provided in the expected location for reference. The presence of this file is mandatory for executing end-to-end tests using Cypress.

#### Setup:
In the root directory use `npm ci` to install dependencies.

### In development:
Use `npm run dev` to run the application in the development mode. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

#### In production:
Use `npm run build` to build the app for production. Then use `npm start` to start the application in production mode.

<br />
