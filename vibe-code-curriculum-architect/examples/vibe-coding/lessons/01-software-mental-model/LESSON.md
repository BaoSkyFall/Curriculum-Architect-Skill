# Lesson: How a Software System Responds

Duration: 90 minutes
Prerequisites: none

## Learning Objectives

Students can identify input, interface, processing, storage, and output in a familiar application and trace one request through those parts.

## Why Students Need This

AI coding agents can generate files quickly, but learners need a stable model for understanding what those files do and where failures belong.

## Mental Model

```text
Person -> Interface -> Request -> Processing -> Data -> Response -> Interface
```

## Core Concepts

Component, boundary, request, response, state, and failure.

## Instructor Explanation

Use a restaurant-order example briefly, then map it to a chat application. Stop the analogy when discussing persistent state and error boundaries.

## Demo

Trace a message from a browser form to a mocked response and label each boundary.

## Hands-on Lab

Complete `LAB.md`.

## Common Mistakes

- Calling every component "the AI."
- Treating the interface as the database.
- Assuming a successful screen means every backend step succeeded.

## Check for Understanding

Ask learners where a failure belongs when the button works but no response returns.

## Assessment

Complete `ASSESSMENT.md`.

## Homework

Draw the data flow of one application used during the week.

## Connection to Next Lesson

The next lesson names the frontend, backend, API, and database boundaries.
