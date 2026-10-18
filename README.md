# AI Crew

<p align="center">
  <img src="https://img.shields.io/badge/AI%20Crew-its%20own%20screen-6366f1?style=for-the-badge" alt="AI Crew — its own screen" />
</p>

> Give the AI its own screen.

AI Crew lets you run an AI agent inside a real desktop environment. The agent works on its own display — reading and writing files, executing code, running shell commands, taking screenshots, and capturing apps or the browser — while you watch everything live through a noVNC iframe. You can jump in at any time and take over the machine directly, with full mouse and keyboard input.

## <img src="./assets/icons/monitor.svg" width="18" height="18" alt=""/> How it works

- <img src="./assets/icons/monitor.svg" width="16" height="16" alt=""/> **The AI has its own screen.** The agent operates inside a virtual desktop instead of just chatting in a terminal. You see exactly what it sees, in real time.
- <img src="./assets/icons/eye.svg" width="16" height="16" alt=""/> **Watch live.** The AI's screen is streamed over VNC and embedded in the app as a noVNC iframe — no plugins or extra clients required.
- <img src="./assets/icons/pointer.svg" width="16" height="16" alt=""/> **Take over.** Switch into takeover mode to interact with the same desktop the AI is using. Fullscreen takeover runs over the same VNC session with input enabled, so you can click, type, and drive the machine yourself.

## <img src="./assets/icons/sparkles.svg" width="18" height="18" alt=""/> Features

- <img src="./assets/icons/file.svg" width="16" height="16" alt=""/> **File operations** — the AI can read and write files on its own desktop
- <img src="./assets/icons/code.svg" width="16" height="16" alt=""/> **Code execution** — run scripts and programs directly in the environment
- <img src="./assets/icons/terminal.svg" width="16" height="16" alt=""/> **Shell access** — full shell command execution
- <img src="./assets/icons/camera.svg" width="16" height="16" alt=""/> **Screenshots** — capture the current state of the AI's screen
- <img src="./assets/icons/window.svg" width="16" height="16" alt=""/> **App / browser capture** — grab specific applications or browser windows
- <img src="./assets/icons/tv.svg" width="16" height="16" alt=""/> **Live screen view** — watch the AI work through an embedded noVNC iframe
- <img src="./assets/icons/fullscreen.svg" width="16" height="16" alt=""/> **Fullscreen takeover** — take remote control of the AI's session with input enabled

## <img src="./assets/icons/cpu.svg" width="18" height="18" alt=""/> Tech stack

- <img src="./assets/icons/rocket.svg" width="16" height="16" alt=""/> [Next.js](https://nextjs.org) (App Router) + React 19 + TypeScript
- <img src="./assets/icons/wind.svg" width="16" height="16" alt=""/> Tailwind CSS v4 + [shadcn/ui](https://ui.shadcn.com) (Base UI)
- <img src="./assets/icons/globe.svg" width="16" height="16" alt=""/> noVNC for browser-based VNC viewing and control

## <img src="./assets/icons/rocket.svg" width="18" height="18" alt=""/> Getting started

Install dependencies:

```bash
npm install
```

Start the dev server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## <img src="./assets/icons/scroll.svg" width="18" height="18" alt=""/> Scripts

| Command             | Description                    |
| ------------------- | ------------------------------ |
| `npm run dev`       | Start the development server   |
| `npm run build`     | Production build               |
| `npm run start`     | Serve the production build     |
| `npm run lint`      | Run ESLint                     |
| `npm run typecheck` | Run the TypeScript compiler    |
| `npm run format`    | Format files with Prettier     |

## <img src="./assets/icons/layers.svg" width="18" height="18" alt=""/> Adding UI components

To add shadcn/ui components to the app:

```bash
npx shadcn@latest add button
```

Then import them where needed:

```tsx
import { Button } from "@/components/ui/button";
```
