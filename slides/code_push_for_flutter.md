autoscale: true
footer: @felangelov - Flutter & Friends 2023
slidenumbers: true

# Shorebird: Flutter Code Push

![inline](../assets/shorebird_logo.png)

### By: Felix Angelov

---

# 👋 Hello

![inline](../assets/about_me.png)

---

# 🦸 Flutter Gives Us Superpowers

- 🎯 Dart
- ⚡️ Hot Reload
- 📱 Mobile (iOS + Android)
- 🖥️ Desktop (MacOS, Linux, Windows)
- 🧩 Declarative UI
- 🔌 Plugins
- 🛠️ Developer Tools

---

# 📱 Flutter & Friends App

![inline fit](../assets/app_hero.png)

---

# 📦 Download It

![inline fit](../assets/app_store_qr.png)![inline fit](../assets/google_play_qr.png)

---

![inline fit](../assets/schedule.png)

---

![inline fit](../assets/talk_details.png)

---

![inline fit](../assets/favorites.png)

---

![inline fit](../assets/sponsors.png)

---

![inline fit](../assets/settings.png)

---

# There's only one problem...

# 😅

---

![inline fit](../assets/meme_5.jpeg)

---

![inline fit](../assets/exhibit_a.png)

---

![inline fit](../assets/exhibit_b.png)

---

![inline fit](../assets/meme_1.png)

---

![inline fit](../assets/meme_2.jpeg)

---

![inline fit](../assets/meme_3.jpeg)

---

[.background-color: #1f2023]
[.text: #ffffff]

![inline](../assets/shorebird_hero.png)

---

![inline](../assets/issue.png)

---

# 🐦 Shorebird Code Push

- ⚡️ Hot Restart in Production
- ✨ Change Any Dart Code
- ⏱️ Deliver Over-The-Air Updates Instantly
- 🧵 Seamless Integration
- 💸 Try For Free

Get Started: **https://shorebird.dev**

---

![inline fit](../assets/meme_4.jpeg)

---

# 🧑‍🍳 Prep

[.column]

- 💨 Integrated Shorebird

  - Visited: https://console.shorebird.dev
  - Installed Shorebird CLI
  - `shorebird init`

- 📦 Created a Release

  - `shorebird release android`
  - `shorebird release ios-alpha`

- 📱 Submitted to the AppStore and PlayStore

[.column]

![inline fit](../assets/console_01.png)

---

# Let's Fix it Live

# 🧑‍🔧🐦

---

### 🥳 Update Available

[.column]

![inline](../assets/update_available.png)

[.column]

**👀 Closer Look**

- 🔔 Silent Notification

- 📦 Patch Downloaded Async In Background

- 🔐 Patch Hash Verification On Device

- 🔁 Restart To Boot From Patch

- 🛼 Automatic Rollback On Bad Patch

---

# ✨ Highlights

- ✅ Android 🤖
- ✅ Flavors 🍧
- ✅ Add-To-App 🧩
- ✅ CI Integration 🚦 (GitHub, Codemagic)
- ✅ Multiple Flutter Versions 🐦
- ☑️ iOS 🍎 (alpha)
- 🚧 Asset Support 🖼️ (coming soon)

---

# ⚠️ Current Limitations

- 😴 iOS Runs ~100x Slower (100% Interpreted)
- 🎈 iOS Patch Sizes Are Large (No Diffing)
- 📜 Flutter Versions >=3.10.0
- 🐎 Stable Channel Only
- 📱 Mobile Platforms Only

---

# 🤔 How Does Shorebird Work?

- 🏎️ Custom Flutter engine that includes Shorebird updater
- 🎯 Custom Dart compiler + Custom Dart interpreter
- ☁️ Compiled binaries hosted on our servers
  - 🙈 We never see your source code
- 🔌 Dart bindings to interact with the updater
  - `package:shorebird_code_push`

---

# 🍰 Layers

![inline](../assets/layers.png)

---

# 🫳 Drop-In Replacement

```sh
# Flutter CLI
$ flutter build appbundle --release
$ flutter build ipa --release

# Shorebird CLI
$ shorebird release android
$ shorebird release ios-alpha
```

---

# 🚦 Continuous Integration

[.column]

```sh
# Generate a CI Token
$ shorebird login:ci
```

[.column]

```yaml
steps:
  - name: 📚 Git Checkout
    uses: actions/checkout@v3

  - name: 🐦 Setup Shorebird
    uses: shorebirdtech/setup-shorebird@v0
    with:
      flutter-version: 3.13.2

  - name: 🤖 Patch Android
    run: shorebird patch android --force
    env:
      SHOREBIRD_TOKEN: ${{ secrets.SHOREBIRD_TOKEN }}

  - name: 🍎 Patch iOS
    run: shorebird patch ios-alpha --force
    env:
      SHOREBIRD_TOKEN: ${{ secrets.SHOREBIRD_TOKEN }}
```

---

# 🏎️ You Are In Control

![inline fit](../assets/package.png)

---

# ✅ Safe For Stores

[.column]
**Play Store**

“An app … may not modify, replace, or update itself using any method other than Google Play's update mechanism.” … “This restriction does not apply to code that runs in a virtual machine or an interpreter”

**Shorebird uses the Dart Virtual Machine. Similar to how other apps use JavaScript or Lua.**

[.column]
**App Store**

3.2.2. “Application may not download or install executable code. Interpreted code may be downloaded…”

**Shorebird uses a custom Dart interpreter on iOS to both comply with store guidelines and provide excellent performance.**

---

[.background-color: #26272b]
[.text: #ffffff]

![inline fit](../assets/join_the_flock.png)

---

# 🔌 Add Shorebird To Your App

## 🗓️ Workshop Tomorrow

![inline fit](../assets/workshop.png)

---

# 💬 Chat With Us

![inline fit](../assets/discord_qr.png)![inline fit](../assets/x_qr.png)

**https://discord.gg/shorebird**
**@shorebirddev**

---

# Thank You!

# 💙🙏
