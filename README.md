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
import "./styles.css";
+ import { streakCounter } from "@zakwanhisham/streak-counter";

export default function App() {
+ const today = new Date();
+ const { currentCount } = streakCounter(localStorage, today);

 return (
   <div className="App">
     <h1 style=>Current streak</h1>
     <div>
       <p style=>
         <span aria-label="fire emoji" role="img">
           🔥
         </span>
       </p>
     </div>
     <p style=>
+       {currentCount} day
+       {currentCount > 1 ? "s" : ""}
     </p>
   </div>
 );
}```
[![Edit streak-counter (ts-course)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/streak-counter-ts-course-twsw1?fontsize=14&hidenavigation=1&theme=dark)
