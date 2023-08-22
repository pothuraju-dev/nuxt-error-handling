# Nuxt Error Handling Example

This repository contains an example Nuxt.js project that demonstrates various techniques for error handling in different contexts, including Vue rendering lifecycle, global error handling, server and client startup errors, and more.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Middleware Error Handling](#middleware-error-handling)
- [Global Error Handling](#global-error-handling)
- [Server Middleware Error](#server-middleware-error)
- [Custom Error Page](#custom-error-page)

## Introduction

This project showcases how to handle errors in different scenarios within a Nuxt.js application. It covers error handling during Vue rendering, global error handling, server and client startup errors, and also includes a custom error page.

## Project Structure

- `middleware/error.global.ts`: This middleware demonstrates how to handle errors during routing using the `defineNuxtRouteMiddleware` function. It simulates an error when a specific query parameter is present.

- `plugins/error.ts`: This plugin showcases global error handling using various hooks and the Vue error handler. It outputs console logs for different error types.

- `server/middleware/error.ts`: This server middleware demonstrates handling errors on the server side. It throws an error when a specific query parameter is present.

- `error.vue`: This is a custom error page that displays error information and provides options to clear the error or navigate to other routes.

- `layouts/default.vue`: This layout wraps the content of each page.

- `nuxt.config.js`: The Nuxt configuration file that sets up plugins and global settings.

## Middleware Error Handling

The `middleware/error.global.ts` middleware simulates an error during routing when a specific query parameter is present. To see this in action:

1. Run the project using `npm run dev`.
2. Navigate to a route with the query parameter `middleware`.
3. The custom error page will be displayed with the error message.

## Global Error Handling

The `plugins/error.ts` plugin demonstrates global error handling using various hooks and the Vue error handler. Console logs are output for different error types. To see this in action:

1. Run the project using `npm run dev`.
2. Open the browser's developer console.
3. Trigger different types of errors (e.g., Vue error, app startup error) by interacting with the app.
4. Observe the console logs showing error messages.

## Server Middleware Error

The `server/middleware/error.ts` server middleware throws an error on the server side when a specific query parameter is present. To see this in action:

1. Run the project using `npm run dev`.
2. Navigate to a route with the query parameter `api`.
3. An error will be thrown and displayed on the console.

## Custom Error Page

The `error.vue` page serves as a custom error page that displays error information and provides options to clear the error or navigate to other routes. To see this in action:

1. Run the project using `npm run dev`.
2. Trigger errors by interacting with the app or navigating to routes with error conditions.
3. Observe the custom error page displaying error information and options to clear the error or navigate to other routes.

---

Certainly! Here are the reference links from the Nuxt.js documentation that relate to error handling:

1. [Nuxt Official Documentation - Error Handling](https://nuxt.com/docs/getting-started/error-handling)
2. [Nuxt Official Documentation - Advanced Error Handling Example](https://nuxt.com/docs/examples/advanced/error-handling)
3. [Nuxt Official Documentation - showError Utility](https://nuxt.com/docs/api/utils/show-error)
4. [Nuxt Official Documentation - useError Composable](https://nuxt.com/docs/api/composables/use-error)
5. [Nuxt Official Documentation - clearError Utility](https://nuxt.com/docs/api/utils/clear-error)
6. [Mastering Nuxt - Custom Error Pages in Nuxt 3](https://masteringnuxt.com/blog/custom-error-pages-in-nuxt3?utm_source=drip&utm_medium=email&utm_campaign=Creating%20Custom%20Error%20Pages%20in%20Nuxt%203)

These links will provide you with more detailed information about each aspect of error handling in a Nuxt.js project, including examples, utilities, and composables provided by Nuxt.js for effective error management.
