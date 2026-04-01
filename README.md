# Lovely Hearts Rewards – production-ready starter

Lovely Hearts Rewards is a polished Node/Express web app starter for an ad-supported wellness rewards product.

## What this version includes
- Secure account registration and login with hashed passwords and signed sessions
- SQLite-backed persistence for users and daily steps
- Dashboard for steps, hearts, streaks, milestone, and rewards
- Weekly leaderboard
- AdSense-ready ad slots with sponsor fallbacks
- Live Walk Mode using browser motion sensors for real in-session step tracking on supported mobile browsers
- Admin profile card using your photo

## Important production note on real step tracking
This release includes real browser motion tracking while the app is open. For deeper platform sync:
- Android Health Connect requires a native Android companion integration
- Apple Health requires a native iOS app with HealthKit capability
- Google Fit REST should not be used as the long-term path because it is being deprecated

## Local development
```bash
npm install
cp .env.example .env
npm start
```
Then open `http://localhost:5000`

## Prepare for GitHub
```bash
git init
git add .
git commit -m "Initial production-ready Lovely Hearts Rewards"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/lovely-hearts-rewards.git
git push -u origin main
```

## Deploy on Render
1. Push this repo to GitHub.
2. Create a new Render Web Service from the repo.
3. Set `BASE_URL` to your Render app URL.
4. Set `JWT_SECRET` to a long secret.
5. Add `ADSENSE_CLIENT` and slot IDs once approved by Google.

## Suggested next production upgrades
- Move persistence from SQLite to Supabase Postgres or managed Postgres
- Add email verification and password reset
- Add a native mobile companion for Apple Health and Health Connect sync
- Add analytics and event tracking for ad placement performance








