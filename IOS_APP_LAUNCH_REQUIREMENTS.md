# Meal Prep iOS Launch Requirements

This document consolidates the metadata, assets, and compliance items needed to submit **PantrySage** to App Store Connect.

## App Store Connect Metadata
- **App Name (<=30 chars)**: PantrySage
- **Bundle Display Name**: Meal Prep
- **Subtitle (<=30 chars)**: Plan. Shop. Cook smarter.
- **Promotional Text (<=170 chars)**: Let the AI Chef plan your week, build smart shopping lists, and guide every recipe while keeping all of your data safely on device.
- **Description (<=4000 chars)**:
  ```
  Cook smarter every day with Meal Prep, the AI-powered kitchen companion that plans, shops, and guides every meal while keeping your data on device.

  - Discover recipes that match 40+ cuisines, dietary needs, cook times, and skill levels.
  - Let AI craft weekly meal plans that balance nutrition goals with your schedule.
  - Auto-build grocery lists organized by aisle and synced to your smart pantry.
  - Switch to Cooking Mode for step-by-step guidance, automatic timers, and measurement conversions.
  - Capture kitchen wins, rate recipes, and save notes to refine future plans.

  Premium unlocks advanced efficiencies:
  - Meal Plan Smart Lists that update instantly when plans change.
  - Barcode-powered pantry tracking with confidence scores and substitutions.
  - AI chef chat for personalized advice, ingredient swaps, and recipe generation.
  - Recipe import from any site plus unlimited recipe saves across devices.

  Privacy comes first - Meal Prep collects zero personal data. Everything stays on your device, from preferences to saved recipes, so you can focus on cooking with confidence.
  ```
- **Keywords (<=100 chars)**: mealprep,aichef,mealplanner,recipes,cookingassistant,shoppinglist,pantrytracker
- **Primary Category**: Food & Drink
- **Secondary Category (optional)**: Health & Fitness
- **Age Rating**: 4+
- **Price Tier**: Free with optional in-app purchase (Meal Prep Premium subscription)
- **In-App Purchase**: Meal Prep Premium (auto-renewing subscription; include screenshots/pricing tiers)
- **App Icon (1024x1024 PNG)**: Export from `assets/images/apple-touch-icon.png` without transparency.
- **Support URL**: https://mealprep.ai/support (points to `support.html`)
- **Marketing URL**: https://mealprep.ai/ (points to landing page `index.html`)
- **Privacy Policy URL**: https://mealprep.ai/privacy (points to `privacy.html`)
- **Copyright**: (c) 2025 Meal Prep
- **Trade Representative Contact (if required)**: 705 King Street West, Toronto, ON M5V 2W8, Canada
- **Company Contact Email**: hello@pantrysage.app
- **Languages**: English (US and Canada). Add localized metadata later if available.

## App Privacy (Data Not Collected)
- **Data Collection**: None. Declare "Data Not Collected" across all privacy categories.
- **Data Usage Notes**: Highlight that meal preferences are processed anonymously for AI meal generation.
- **Link**: Ensure `privacy.html` clearly states zero personal data collection (already satisfied).
- **App Tracking Transparency**: Not used; confirm "No" inside App Store Connect.

## Screenshot Order and Taglines
Export 6.5" (1242x2688) portrait screenshots (and 6.7" if desired). Apply the following order and captions in App Store Connect:

| # | Asset Path | Tagline | Feature Spotlight | Notes |
| - | - | - | - | - |
| 1 | `assets/images/Screenshots/Recipes_Photos` | "Personalized recipes for every craving." | Advanced discovery and filters | Use as hero screenshot with strongest visual dish. |
| 2 | `assets/images/Screenshots/Meal Planner` | "Weekly meal plans built by your AI chef." | AI-driven planning and nutrition goals | Show calendar view plus nutrition summary. |
| 3 | Capture new (Shopping List view) | "Smart shopping lists organized by aisle." | Auto-synced grocery lists | Take fresh screenshot showing list grouped by aisle with pantry indicators. |
| 4 | `assets/images/Screenshots/Pantry` | "Track pantry items with barcode scanning." | Smart pantry with confidence levels | Highlight barcode scanner UI. |
| 5 | `assets/images/Screenshots/Cooking a recipe start to FInish` | "Step-by-step cooking guidance with timers." | Cooking Mode timers and progress | Show timers and conversions in action. |
| 6 | `assets/images/Screenshots/Ai Chef Chat` | "Ask the AI Chef anything in the kitchen." | Conversational assistant and substitutions | Capture response explaining ingredient swap. |
| 7 | `assets/images/Screenshots/Selecting a Recipe` | "Powerful filters to find your perfect dish." | Multi-filter discovery | Optional for additional locales or App Preview stills. |
| 8 | `assets/images/Screenshots/User Guide` | "Onboarding that teaches every feature." | User guidance and activation | Use for iPad or secondary set if needed. |

> For devices lacking a specific raw asset, capture new simulator screenshots that match the design showcased on `index.html`. Maintain consistent status bars (9:41 AM, LTE, full battery) and frame them if desired.

## App Preview (Optional but Recommended)
- 30 to 45 second video highlighting: recipe discovery -> meal planning -> smart list -> cooking mode -> AI chat.
- Export at 1080x1920 portrait, upload to App Store Connect with matching callouts.
- Use the same copy tone as the taglines and include captions for accessibility.

## App Store Listing Assets Checklist
- [ ] App icon (1024x1024 PNG, no transparency)
- [ ] Universal 6.5" and 6.7" portrait screenshots (PNG)
- [ ] Optional iPad 12.9" and 8.3" screenshots if iPad supported
- [ ] Optional macOS screenshots (if distributing via Catalyst)
- [ ] App Preview video (if produced)
- [ ] Feature graphic for Apple Search Ads (required if running campaigns)

## Compliance and Review Notes
- **Sign-In Required**: No account signup. Mention in review notes that the app is fully usable without login.
- **Purchases Restored**: Confirm restore flow for Meal Prep Premium in the build.
- **Content Rights**: Document that recipes and images are original or AI-generated with rights cleared.
- **Third-Party SDKs**: None beyond Apple frameworks (state in review notes).
- **Encryption**: Uses standard Apple encryption only; answer "No" to export compliance question.
- **Test Notes for Reviewer**: Provide instructions to access premium features (for example, note paywall flow or supply TestFlight promo code).
- **Contact for Review**: hello@pantrysage.app

## Pre-Submission QA
- [ ] Build signed with release distribution certificate and provisioning profile.
- [ ] All premium paywall prices localized and match in-app purchase setup.
- [ ] Push notifications, if used, have a clear user-facing purpose (timer reminders) and toggles in Settings.
- [ ] Dynamic text, VoiceOver, and landscape support validated.
- [ ] App version number matches marketing copy (v1.0.0).
- [ ] Ensure support page and privacy policy load correctly on mobile Safari.

## Marketing Launch Notes
- Align landing page hero copy with App Store subtitle ("Plan. Shop. Cook smarter.").
- Sync promotional text across email, social teasers, and website banners.
- Highlight privacy-by-design, AI meal planning, smart shopping lists, and premium barcode scanner in launch messaging.
- Submit optional Today tab or feature request to Apple 14 days before launch if seeking editorial promotion.

---
**Next Steps**
1. Capture new simulator screenshots if any asset coverage is missing.
2. Populate App Store Connect product page with the above metadata.
3. Submit build for App Review with reviewer notes referencing the zero-data privacy approach.
