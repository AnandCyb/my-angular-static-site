# My Angular Static Site

Angular 7 static website for testing purposes with multiple pages and routing.

## Overview

This is a simple static website built with Angular 7, demonstrating basic routing and component-based architecture. The project includes three main pages:

- **Home Page**: Welcome page with project features
- **About Page**: Information about the project and technologies used
- **Contact Page**: Contact information and details

## Features

- Built with Angular 7.3.10
- Multi-page navigation using Angular Router
- Responsive design with modern CSS
- Clean and maintainable component structure
- Production-ready build configuration

## Prerequisites

- Node.js (v8.x or higher)
- npm (v5.x or higher)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AnandCyb/my-angular-static-site.git
   cd my-angular-static-site
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build:

```bash
ng build --prod
```

For GitHub Pages deployment, build with the correct base-href:

```bash
npm run build:prod -- --base-href=/my-angular-static-site/
```

## Deployment to GitHub Pages

This project is configured for automatic deployment to GitHub Pages using GitHub Actions.

### Automatic Deployment

The project will automatically deploy to GitHub Pages when you push to the `main` branch. The workflow:

1. Builds the Angular application with production optimizations
2. Configures the correct base-href for GitHub Pages
3. Uploads the build artifacts
4. Deploys to GitHub Pages

### Setup Instructions

To enable GitHub Pages deployment for your fork:

1. Go to your repository settings on GitHub
2. Navigate to **Settings > Pages**
3. Under **Build and deployment**, select:
   - **Source**: GitHub Actions
4. Push changes to the `main` branch
5. The workflow will run automatically and deploy your site

Once deployed, your site will be available at: `https://[username].github.io/my-angular-static-site/`

### Manual Deployment

You can also trigger a deployment manually:

1. Go to the **Actions** tab in your repository
2. Select the "Deploy to GitHub Pages" workflow
3. Click "Run workflow"

## Project Structure

```
src/
├── app/
│   ├── home/          # Home page component
│   ├── about/         # About page component
│   ├── contact/       # Contact page component
│   ├── app-routing.module.ts  # Routing configuration
│   └── app.component.*        # Main app component
├── assets/            # Static assets
└── environments/      # Environment configurations
```

## Technologies Used

- **Angular 7**: Web application framework
- **TypeScript**: Programming language
- **Angular Router**: Client-side routing
- **CSS3**: Styling and layout

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## License

This project is created for testing and demonstration purposes.
