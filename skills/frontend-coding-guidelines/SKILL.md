---
name: frontend-coding-guidelines
description: Frontend architecture and coding standards. Use when writing, reviewing, or refactoring frontend code.
---
# Frontend Coding Guidelines

Use the following rules when coding frontend applications, except when applications have different rules or structure. self instruct yourself through genereting .local/frontend-coding/SKILL.md explaining the rules and structure in similar format like this one.

## Architecture

The architecture should be feature + page, components. e.g

```text
<feature>/layouts/*
<feature>/pages/*
<feature>/components/*
<feature>/services/*
```

where in root you have:
layouts/* (Shared) e.g AuthLayout, AppLayout
components/* (Shared)
services/* (Shared and bases)
utils/* (Shared) e.g utils.ts, constants.ts etc.

The services you always write in this format
services/example/hooks.ts -- contains hooks
services/example/api.ts -- contains basic fetch
services/example/utils.ts -- optional helpers

## Dependencies

must use the following deps:

- Tenstack for queries
- Antd + AntdX UI library
- React Router
- Vite
- Vitest for testing

Whenever you are using any dependencies always check for latest versions and best practices for that dependency.

## Principles

no app-defined classes, functions driven, simple one layer, modular components, strive for human maintainability, stateless logic, and pure functions, tidy-as-you go

**important**: You strive to have tests, you focus on writing the goal through the tests, you define the output of the system through testing and for critical workflows use e2e tests.
