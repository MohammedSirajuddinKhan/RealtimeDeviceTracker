# RealtimeDeviceTracker

A small MERN-learning project providing real-time device/location updates using Express, EJS and Socket.IO.

## Features
- Real-time location/device updates via Socket.IO
- Server-rendered UI using EJS
- Static frontend assets in `public/`

## Prerequisites
- Node.js (v14+ recommended)
- npm

## Install
1. Install dependencies:

```bash
npm install
```

## Run
- Start the server:

```bash
node app.js
```

- The app runs on http://localhost:3000 by default.

## Usage
- Open http://localhost:3000 in a browser.
- Clients can emit `send-location` events (see `public/js/script.js`) and will receive `receive-location` events broadcast from the server.

## Project Structure
- `app.js` - Express + Socket.IO server
- `views/index.ejs` - Main front-end template
- `public/js/script.js` - Client-side Socket.IO code
- `public/css/style.css` - Styles

## Notes
- `package.json` currently does not include a `start` script; use `node app.js` or add a script such as:

```json
"scripts": {
  "start": "node app.js"
}
```

## License
This project is provided as-is.
