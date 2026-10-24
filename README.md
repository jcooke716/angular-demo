# AngularDemo

## Project overview

An Angular 13 training application that separates several browser interactions into routed components. The central example is an in-memory book catalog, supported by smaller text-copy, counter, display-toggle, and list-rendering exercises.

### Problem and approach

The project explores how to separate component presentation from shared application state. `BookService` owns the book collection and implements lookup, add, update, and delete operations; the book-list component consumes that service through dependency injection.

| Route | Exercise |
| --- | --- |
| `/book-crud` | Book listing, an add form, and deletion backed by an in-memory service. |
| `/counter` | Incrementing and decrementing component state. |
| `/copy` | Copying a value between bound fields. |
| `/display` | Toggling displayed text. |
| `/list-fruit` | Rendering a list. |

### Local use

Use Node.js and npm versions compatible with the committed Angular 13 dependencies.

```bash
npm ci
npm start
```

Open `http://localhost:4200/book-crud`. The data is held in a JavaScript array and resets when the application reloads; no database or backend API is included. `npm run build` and `npm test` are the build and test scripts declared in `package.json`.

### Portfolio context and attribution

Components, routing, dependency injection, forms, and service-based state management. This is a training fork of [DeveloperOneDemo/angular-demo](https://github.com/DeveloperOneDemo/angular-demo). The upstream material and original Angular CLI guidance below are retained.

## Angular CLI reference


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.2.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
