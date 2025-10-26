# Screenshot Reward Bot (Normal version)

## Quick deploy (GitHub → Render)

1. Create a GitHub repository and push entire `screenshot-reward-bot` folder.
2. On Render.com create a **New Web Service** → Connect GitHub → choose this repo.
3. Set:
   - Environment: Node
   - Start Command: `node server.js`
4. Add Environment Variables in Render dashboard (Environment):
   - BOT_TOKEN
   - CHANNEL_ID
   - BASE_URL (Render URL you will get after deploy; you can add it later)
   - DB_PATH = ./db.json
5. Deploy. Once deployed, open your Render URL.

## Usage (Frontend)
- POST `/register` with JSON `{ "username":"yourname" }`
- POST `/upload` multipart/form-data: `screenshot` file + `username` field
- GET `/balance?username=yourname`

## Notes
- Each upload gives ৳0.15 and max 3 uploads per user.
- Make sure BASE_URL is the public Render URL so Telegram can fetch the image.
- Never commit real `.env` to public repo.
