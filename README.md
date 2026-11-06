<div align="center">
  <img src="branding/trailmix-logo.png" alt="Trail Mix logo" width="260">

  <p><strong>The dating app for single granola people.</strong></p>

  <img src="https://img.shields.io/badge/status-In%20development-B4552B?style=flat-square" alt="status"> <img src="https://img.shields.io/badge/platform-iOS%2017%2B-EFE6D2?style=flat-square" alt="platform"> <img src="https://img.shields.io/badge/license-proprietary-555555?style=flat-square" alt="license"> <img src="https://img.shields.io/badge/by-Aquila%20Digital%20LLC-14213D?style=flat-square" alt="Aquila Digital LLC">
</div>

> **Showcase repository.** The source code for TrailMix is not published. This page presents what the product is and how it works.

## Screenshots

The onboarding flow through Discover, match and chat (simulator, light theme).

<p align="center">
  <img src="docs/screenshots/onboarding-to-chat.jpg" width="100%" alt="TrailMix onboarding, Discover, match and chat screens">
</p>

## Overview

A native iOS dating app for outdoorsy people. Match on shared activities, plan real trips together, chat, and use built-in safety tools like trip check-ins and trusted contacts.

## How it works

```mermaid
flowchart LR
  A["Onboarding: one question per screen, 18+ confirmed"] --> B["Discover: mutual-interest matching with filters"] --> C["Like a prompt, match, chat"] --> D["Plans: host or join an activity"] --> E["Trip check-in with trusted contacts"]
```

## Features

- Sign in with Apple only; Supabase auth + RLS
- Discover feed with age, distance, goal and activity filters; like / pass / undo
- Plans: create, join and host real outings
- Chat with typing indicator, read receipts, icebreakers
- Safety center: report, block, unmatch, meeting tips, account deletion
- Custom "Granola Warm" light / "Golden Hour" dark design system with bundled Fraunces display font
- Local demo mode with sample people when no keys are configured

## Tech stack

| Layer | Choice |
|---|---|
| Language / UI | Swift 6, SwiftUI, iOS 17+, XcodeGen |
| Backend | Supabase: Postgres, Auth, Realtime, Storage, RLS |
| Design | Asset-catalog tokens, Fraunces (OFL) + SF Pro |
| Tests | XCTest + Supabase security tests |

## Privacy & security

Photos are stripped of GPS/EXIF and downscaled. Birthdate is never shown, only age. Account deletion is built in.

## Brand

| | Name | Hex | Role |
|---|---|---|---|
| <img src="https://placehold.co/44x22/EFE6D2/EFE6D2.png" alt="#EFE6D2" /> | Granola | `#EFE6D2` | Light background |
| <img src="https://placehold.co/44x22/2F4A3A/2F4A3A.png" alt="#2F4A3A" /> | Pine | `#2F4A3A` | Brand green |
| <img src="https://placehold.co/44x22/B4552B/B4552B.png" alt="#B4552B" /> | Clay | `#B4552B` | Accent |
| <img src="https://placehold.co/44x22/1B1F2E/1B1F2E.png" alt="#1B1F2E" /> | Night | `#1B1F2E` | Dark background |
| <img src="https://placehold.co/44x22/F2A65A/F2A65A.png" alt="#F2A65A" /> | Golden Hour | `#F2A65A` | Dark accent |

**Mark.** Circular badge: a heart split into an almond half and a raisin half, flanked by pine trees. "Find your trail mix."

**Voice.** Warm, a little cheeky, outdoorsy. Safety copy stays plain and serious.

## Roadmap

- Missed check-in alerts (UI only today)
- Push notifications
- Photo / ID verification
- Image moderation
- Analytics decision
- Launch region

## Notes

Brief: `TrailMix-Build-Brief.md`. Design explorations in `Design/`.

## License

Proprietary. Shared publicly for portfolio and demonstration purposes only. See [LICENSE](LICENSE).

---

<div align="center">

Built by [Aquila Digital LLC](https://github.com/Steven6Brown) · *Per Aspera Ad Astra*

</div>
