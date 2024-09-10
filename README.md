<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AutoDeploy: Automating Spring Boot and React Build & Publish</title>
</head>
<body>
    <h1>AutoDeploy: Automating Spring Boot and React Build & Publish</h1>

    <h2>Project Overview</h2>
    <p>
        <strong>AutoDeploy</strong> is an automated solution for building and publishing both a Spring Boot backend and React frontend to GitHub’s npm registry using GitHub Actions. This project simplifies continuous deployment and enhances version control and error handling while maintaining security.
    </p>

    <h2>Key Features</h2>
    <ul>
        <li><strong>GitHub Actions Workflow:</strong> Automates the build and publish process for both the backend and frontend applications.</li>
        <li><strong>Spring Boot Backend:</strong> Automatically compiles and packages the Spring Boot application, preparing it for deployment.</li>
        <li><strong>Frontend Packaging:</strong> Publishes a TypeScript Axios package for seamless API interaction with the backend.</li>
        <li><strong>Node.js and npm Integration:</strong> Installs npm dependencies and automatically bumps package versions.</li>
        <li><strong>GitHub Authentication:</strong> Uses GitHub tokens to securely authenticate and publish packages.</li>
        <li><strong>API Integration:</strong> Allows the React frontend to dynamically fetch backend data via the npm package.</li>
        <li><strong>Error Handling:</strong> Implements input validation and error management to ensure a smooth user experience.</li>
    </ul>

    <h2>Tech Stack</h2>
    <ul>
        <li><strong>Backend:</strong> Spring Boot, Maven</li>
        <li><strong>Frontend:</strong> React, TypeScript, Axios</li>
        <li><strong>CI/CD:</strong> GitHub Actions</li>
        <li><strong>Package Management:</strong> npm, GitHub npm Registry</li>
        <li><strong>Authentication:</strong> GitHub Tokens</li>
    </ul>

    <h2>How It Works</h2>
    <ol>
        <li><strong>GitHub Actions Setup:</strong> The workflow automates building and publishing for both backend and frontend.</li>
        <li><strong>Backend (Spring Boot):</strong> The Spring Boot backend is compiled using Maven, preparing it for deployment.</li>
        <li><strong>Frontend (React + Axios):</strong> The frontend app is built with React and TypeScript Axios and published to npm.</li>
        <li><strong>Secure Publishing:</strong> GitHub tokens authenticate and publish the npm package securely.</li>
        <li><strong>API Integration:</strong> The React app dynamically fetches data from the backend via the npm package.</li>
        <li><strong>Error Management:</strong> Input validation and error handling ensure a seamless experience.</li>
    </ol>

    <h2>Installation</h2>

    <h3>Clone the Repository</h3>
    <pre>
        <code>
git clone https://github.com/yourusername/AutoDeploy.git
cd AutoDeploy
        </code>
    </pre>

    <h3>Backend Setup (Spring Boot)</h3>
    <pre>
        <code>
# Navigate to backend directory
cd backend

# Build the Spring Boot project
mvn clean package
        </code>
    </pre>

    <h3>Frontend Setup (React + TypeScript Axios)</h3>
    <pre>
        <code>
# Navigate to frontend directory
cd ../frontend

# Install npm dependencies
npm install

# Start the frontend server for local development
npm start
        </code>
    </pre>

    <h3>GitHub Actions CI/CD</h3>
    <p>
        Set up the <code>.github/workflows</code> folder for GitHub Actions with the necessary configuration files for building and publishing. On each push to the main branch, the workflow will automatically build, bump the version, and publish the package.
    </p>

    <h2>Environment Variables</h2>
    <p>Ensure to set up the following environment variables in your repository:</p>
    <ul>
        <li><strong>GITHUB_TOKEN:</strong> GitHub token for authentication.</li>
        <li><strong>DATABASE_URL:</strong> URL for your Spring Boot backend database.</li>
    </ul>

    <h2>Usage</h2>
    <ul>
        <li><strong>Frontend:</strong> Fetch data from the backend by importing the published npm package.</li>
        <li><strong>Backend:</strong> Serve data to the frontend and manage API requests.</li>
    </ul>

    <h2>Contributing</h2>
    <ol>
        <li>Fork the repository.</li>
        <li>Create a new branch (<code>git checkout -b feature-branch</code>).</li>
        <li>Make your changes.</li>
        <li>Push to the branch (<code>git push origin feature-branch</code>).</li>
        <li>Open a pull request.</li>
    </ol>
</body>
</html>

