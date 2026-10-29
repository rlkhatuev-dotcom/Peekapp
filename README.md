# peek. — iPhone PWA

A working offline-capable progressive web app prototype. No build tools required.

## Publish (HTTPS required for iPhone installation)

1. Extract this ZIP.
2. Upload the **contents** of the `peek_pwa` folder to a static HTTPS hosting service such as Netlify Drop (https://app.netlify.com/drop), Cloudflare Pages or GitHub Pages. Keep all files together.
3. Open the deployed HTTPS URL in **Safari on iPhone**.
4. Tap **Share → Add to Home Screen → Add**.
5. Open **peek.** from the Home Screen.

## What works
- Five separate configurable modes and custom modes.
- Real elapsed time based on timestamps, including while Safari is in the background; manual distraction start/stop.
- Per-mode duration, reminder text and delay, allowed-apps note.
- Session completion, history and aggregate focus/distraction time.
- Income/expense entries, debts and partial debt payments.
- Demo steps and editable goal, dark mode, persistent localStorage.
- Service worker for offline loading after first successful online visit.

## Limitations
- This PWA **cannot detect** when you switch to another app or show a persistent overlay over other apps.
- Automatic notifications are **not implemented**. Notification permission request alone does not schedule notifications. No Dynamic Island/Live Activity integration.
- Steps are demo values, not real Apple Health steps.
- Data is local to the browser installation; clearing site data or deleting the PWA can erase it.
- An active timer uses real wall-clock elapsed time. The app cannot infer whether the user was distracted without manually starting the distraction timer.
- This is a test prototype, not an App Store iOS binary.
