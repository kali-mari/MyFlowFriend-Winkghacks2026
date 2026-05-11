# MyFlowFriend
Tamagotchi-inspired menstrual tracker built for WiNGHacks 2026 at the University of Florida and winner of the WiNG Track

## Tech Stack

**Hardware**
- ESP32 + 3.5" TFT ILI9488 display
- SPI-optimized rendering via `TFT_eSPI` + double-buffering with `TFT_eSprite` (RAM canvas → single-burst push)
- Non-blocking C loop handling touch interrupts + Wi-Fi concurrently
- NVS persistence via `Preferences` library

**Mobile**
- React Native + TypeScript
- Firebase backend — ESP32 posts symptoms over HTTPS → syncs to app in real time

**AI**
- Gemini 2.5 Flash — cycle phase prediction from daily logs + health chatbot

## Authors
* Kali Schuchhardt: [@kalischuchhardt](https://github.com/kalischuchhardt)
* Kalista Oberes: [@kali-mari](https://github.com/kali-mari)

## Additional links
* [Devpost Page](https://devpost.com/software/my-flowfriend)
* [Demo Video](https://youtu.be/hejCKkAaBac?si=jXBUU0PBryCIKwtq)
