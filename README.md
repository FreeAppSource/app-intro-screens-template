# App Intro Screens Template

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Jones Geckler** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `app-intro-screens-template-jones-heckler.sketch` by **Jones Geckler**: one route per artboard, with the artboard's layout, colours, images and text.

![App Intro Screens Template screens](./showcase.jpg)

## 📱 Screens (4 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Intro Screen 1** · start screen | `src/app/intro-screen-1.jsx` | 375 × 812 | 5 |
| 2 | **Intro Screen 2** | `src/app/intro-screen-2.jsx` | 375 × 812 | 6 |
| 3 | **Intro Screen 4** | `src/app/intro-screen-4.jsx` | 375 × 812 | 5 |
| 4 | **Intro Screen 3** | `src/app/intro-screen-3.jsx` | 375 × 812 | 6 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Abril Fatface, Inter, Lato), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/app-intro-screens-template> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **App Intro Screens Template** design by **Jones Geckler**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Jones Geckler](https://www.sketchappsources.com/contributor/jonesheckler) |
| Original design | [App Intro Screens Template](https://www.sketchappsources.com/contributor/jonesheckler) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4430-app-intro-onboarding-screens-template-sketch-freebie-resource.html) |
| Original file | `app-intro-screens-template-jones-heckler.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "App Intro Screens Template" by Jones Geckler (https://www.sketchappsources.com/contributor/jonesheckler), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4430-app-intro-onboarding-screens-template-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
