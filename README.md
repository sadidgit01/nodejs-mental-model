# Node.js — The Complete Mental Model

**Not a tutorial. Not a roadmap.** Everything
that makes Node.js *actually work*, connected as a single system instead of
a list of isolated topics. A page that maps how V8, libuv, the Event Loop, modules, globals, and core APIs all fit together into one system, so the syntax you learn afterward actually lands on solid footing.

🔗 **[View it live](https://sadidgit01.github.io/nodejs-mental-model/)**

---

## What's inside

- **The Big Picture** — what Node.js is, why it exists, and how V8 + libuv
  + the OS stack on top of each other
- **Running Your Code** — `node file.js`, the REPL, `console.log`, nodemon
- **The Event Loop** — the actual heart of Node, as a hand-drawn diagram:
  Call Stack → Web APIs/libuv → Callback Queue + Microtask Queue → Event
  Loop → back to the Call Stack, with a numbered step-by-step walkthrough
- **Async Patterns** — callbacks → Promises → async/await, shown side by
  side solving the exact same problem three ways
- **Modules & npm** — `require`/`import`, `package.json`,
  `package-lock.json`, `node_modules`, npm scripts, `npx`, dependencies vs
  devDependencies
- **Globals & Environment** — `process`, `console`, `__dirname`/`__filename`,
  environment variables
- **Core Built-in APIs** — `fs`, `http`, `path`, `os`, `Buffer`, Streams,
  EventEmitter, Timers
- **Project Structure** — a real folder tree, explained file by file
- **31-question self-check** — no code lookup, just a gut check on whether
  the mental model actually stuck
- **One-screen cheat sheet** — every term above, condensed to a single
  skimmable reference

## Why this exists

Most people jump straight into "build a REST API with Express" without ever forming a mental model of *why* any of it works: why Node doesn't freeze on slow I/O, what a callback actually is, why `npm install` creates that giant `node_modules` folder. Designed to be read once from **start to finish**, then kept it as a reference.
This page treats Node as **one connected machine**: your code calls
modules, modules call the runtime, the runtime hands slow work to libuv,
and results flow back through the Event Loop- all traceable on one
scroll, front to back.

## How to use it

- Read it once, top to bottom, in order.
- Click any card marked **›** to expand a short, focused explanation
  (what it is, why it exists, what it does, how it connects).



