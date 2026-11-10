# ECONOMIC EMPIRE — Online multiplayer

## Deploy (public internet)
1. Install Node.js 18+.
2. Upload this folder to a GitHub repository.
3. In Render.com choose New → Web Service and connect the repository.
4. Build command: `npm install`
5. Start command: `npm start`
6. After deployment, open the public HTTPS URL. Teacher creates a room; QR code is generated using that public URL.

## Local test
Run `npm install`, then `npm start`, and open http://localhost:3000.
For phone testing on the same Wi-Fi, use the computer's LAN IP and allow inbound connections.

## Features
- Teacher host panel and room QR.
- Up to four teams join from their own phones.
- Seven institutional economics case rounds, same case for all teams.
- Answer options are sent privately to each team's socket.
- Team answers remain hidden until everyone answers or the 60-second timer expires.
- Correct answer earns 1000 points plus 5 points per remaining second.
- Final leaderboard.

Room data is held in server memory and resets when the server restarts. This is a classroom prototype; for production use, add persistent storage and reconnect/session recovery.
