# Lab 1: Node.js and Express server

**Name:** Ch.Sriram · **Registration number:** 252U1R1057 · **Section:** CSE-2A(223)

**Live link:** Not deployed yet — paste your Render/Railway/Cloud IDE URL here

## How to run

```bash
npm install
npm start            # Express server (server.js) on http://localhost:3000
npm run start:http   # plain http module server (server-http.js)
```

Environment variables: `PORT` (optional, defaults to 3000). No secrets are needed.

## Endpoints

| Method | Path     | Description                          | Status |
| ------ | -------- | ------------------------------------ | ------ |
| GET    | `/`      | Welcome text                         | 200    |
| GET    | `/about` | JSON with name and section           | 200    |
| GET    | `/time`  | Current date and time                | 200    |
| GET    | any other| "404 - Route not found" message      | 404    |

## Screenshots

![Route /](screenshots/root.png)
![Route /about](screenshots/about.png)
![Route /time](screenshots/time.png)
![Unknown route 404](screenshots/404.png)

## package.json fields

- **name / version / description**: identify the project.
- **main**: entry file of the project (`server.js`).
- **scripts**: shortcuts run with `npm run <name>` (`npm start`).
- **keywords / author / license**: metadata about the package.
- **dependencies**: packages the project needs (Express); installed into `node_modules`.

## Notes

- `package.json` lists what the project needs; `node_modules` holds the actual installed code, so it is not committed.
- The 404 handler is placed after all routes so it only runs when nothing else matched.
- Add your problems faced and how you solved them here.
