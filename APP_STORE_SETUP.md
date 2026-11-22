# Tube Riders — App Store setup checklist

## 1. Apple Developer / ASC

- [ ] Identifiers → App IDs → `com.piperider.game`
- [ ] Profiles → App Store distribution profile for that ID → download / upload to Codemagic
- [ ] App Store Connect → New App  
  - Name: Tube Riders (or available variant)  
  - Bundle ID: com.piperider.game  
  - SKU: piperider-ios  
- [x] Apple ID `6837967243` set in `codemagic.yaml`

## 2. Codemagic

- [ ] Application linked to `Rahman-dev-ML/pipe-rider`
- [ ] App Store Connect integration + signing for `com.piperider.game`
- [ ] Start workflow **Tube Riders iOS (App Store)** on `main`

## 3. Listing (after first build)

- Privacy / Support URL: `https://cdn.jsdelivr.net/gh/Rahman-dev-ML/pipe-rider@main/privacy.html`
- Category: Games → Racing (or Action)
- Age: check content questionnaire honestly
- App Privacy: Data Not Collected
- Encryption: No (non-exempt) — set in build
- Screenshots: capture from the HTML / TestFlight build at ASC sizes
