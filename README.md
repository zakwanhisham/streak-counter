# `@zakwanhisham/streak-counter` - a basic streak counter

This is a basic streak counter - inspired by Duolingo - written in TypeScript and meant for the browser (uses `localStorage`).

## Install

yarn:

```bash
yarn add @zakwanhisham/streak-counter
```
npm:
```bash
npm install @zakwanhisham/streak-counter
```

## Usage

```javascript
import {streakCounter} from "@zakwanhisham/streak-counter";

const today = new Date();
const streak = streakCounter(localStorage, today);
// streak returns an object:
// {
//    currentCount: 1,
//    lastLoginDate: "11/11/2021",
//    startDate: "11/11/2021",
// }
```
