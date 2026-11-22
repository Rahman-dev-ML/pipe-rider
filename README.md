# Tube Riders

Ultra 3D pipe racer — Capacitor iOS wrapper for App Store / TestFlight via Codemagic.

## Bundle

- **Name:** Tube Riders  
- **Bundle ID:** `com.piperider.game`  
- **Privacy:** https://cdn.jsdelivr.net/gh/Rahman-dev-ML/pipe-rider@main/privacy.html  

## App Store Connect (do this once)

1. Create a new iOS app → Bundle ID `com.piperider.game`  
2. Copy the numeric **Apple ID** from App Information  
3. Put it in `codemagic.yaml` as `APP_STORE_APPLE_ID`  
4. Create an **App Store** distribution provisioning profile for `com.piperider.game` and upload it in Codemagic (same team as Chroma / Tube Riders)  
5. Codemagic → add this GitHub repo → start **Tube Riders iOS (App Store)** on `main`

## Local

```bash
npm install
npx cap sync ios
```

Web game lives in `web/index.html`.
