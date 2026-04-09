# E-Invoices (Angular 21)

A modern Angular 21 application for managing electronic invoices with a clean, scalable architecture.

## Overview

This project is built with Angular 21 and is intended as a foundation for full-stack e-invoicing workflows, including:

- invoice creation and editing
- customer and product management
- tax and total calculations
- export, reporting, and future API integrations

## Tech Stack

- Angular 21
- TypeScript
- RxJS
- Angular Router
- Angular CLI

## Prerequisites

Install the following before running the project:

- Node.js 22.x (LTS recommended)
- npm 10+
- Angular CLI 21

Install Angular CLI globally:

```bash
npm install -g @angular/cli@21
```

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/devhasnat/e-invoices.git
cd e-invoices
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
ng serve
```

4. Open the app in your browser:

```text
http://localhost:4200/
```

## Useful Scripts

Use these commands after dependencies are installed:

- Start dev server:

```bash
npm run start
```

- Build production bundle:

```bash
npm run build
```

- Run unit tests:

```bash
npm run test
```

- Run linting:

```bash
npm run lint
```

## Build for Production

```bash
ng build --configuration production
```

Build output is generated in the `dist/` directory.

## Suggested Project Structure

```text
src/
	app/
		core/           # singleton services, guards, interceptors
		shared/         # reusable components, pipes, directives
		features/       # domain modules (invoices, customers, reports)
		app.routes.ts   # route configuration
	assets/
	environments/
```

## Environment Configuration

Use Angular environment files for runtime configuration:

- `src/environments/environment.ts` for development
- `src/environments/environment.prod.ts` for production

Typical values include API base URL, feature flags, and logging toggles.

## Coding Standards

- Prefer standalone components and feature-based folders.
- Keep components lean; place business logic in services.
- Use strict typing and avoid `any` whenever possible.
- Write tests for services, components, and critical workflows.

## Roadmap

- Authentication and role-based access
- PDF invoice generation
- Email delivery integration
- Dashboard analytics
- Multi-currency and localization support

## Contributing

1. Create a feature branch.
2. Make small, focused changes.
3. Add/adjust tests for your changes.
4. Open a pull request with a clear description.

## License

This project is licensed under the MIT License.
