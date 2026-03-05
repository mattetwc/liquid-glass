# 🧊 liquid-glass - Smooth Glass Effect for Home Assistant

[![Download liquid-glass](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://github.com/mattetwc/liquid-glass/releases)

---

## ❄️ What Is Liquid Glass?

Liquid Glass adds a smooth, frosted glass look to your Home Assistant cards. It uses advanced visual effects like SVG displacement filters and squircle masking. These effects create a modern, polished backdrop that looks like liquid glass. The card edges have smooth, rounded corners and a subtle glass rim, making your Home Assistant interface look cleaner and more refined.

This effect works best on Chromium-based browsers such as Chrome, Edge, and Brave. These browsers support the features needed to create the visual style. Other browsers like Firefox and Safari might not show the effect properly.

---

## 🌟 Main Features

- Fast, high-quality SVG displacement filter for the frosted look
- Squircle corners that gently round the edges for a soft feel
- Decorative rim that adds depth to the glass effect
- Works easily with card_mod integration
- Automatically applies styles with classes or config settings
- Customize radius and rim thickness to suit your style

---

## 💻 System Requirements

- Windows 10 or newer
- A Chromium-based web browser (Chrome, Edge, Brave) installed
- Home Assistant setup with Lovelace UI
- Basic access to Home Assistant configuration or HACS for installation

---

## 🚀 How to Download and Install on Windows

Follow these steps to get liquid-glass running on your Windows machine with Home Assistant.

### Step 1: Visit the Releases Page

Click the green button below to visit the liquid-glass releases page. This page has the latest version ready for you to get.

[![Download liquid-glass](https://img.shields.io/badge/Download-Now-ff6f61?style=for-the-badge)](https://github.com/mattetwc/liquid-glass/releases)

---

### Step 2: Choose Your Installation Method

You can install liquid-glass either through HACS (the recommended way) or manually. HACS makes updates and management simpler, but manual installation also works.

---

## 📥 Installation via HACS (Recommended)

1. Open your Home Assistant dashboard in your browser.
2. Click on **HACS** in the sidebar.
3. Click the menu icon (three dots) in the top right corner.
4. Choose **Custom repositories**.
5. In the URL field, enter:  
   `https://github.com/mattetwc/liquid-glass`
6. Set the category to **Lovelace**.
7. Click **Add**.
8. Now, go to the HACS store and search for “Liquid Glass”.
9. Click to install it.
10. Restart Home Assistant to activate the new effect.

After the restart, you can enable the liquid glass effect via card_mod configuration or by adding the provided CSS classes to your cards.

---

## 📂 Manual Installation

1. Go to the [liquid-glass releases page](https://github.com/mattetwc/liquid-glass/releases).
2. Find the latest release.
3. Download the file named `liquid-glass.js`.
4. Save the file into your Home Assistant `www` directory (usually `/config/www/`).
5. Add a reference to this file in your Lovelace resources:

```yaml
resources:
  - url: /local/liquid-glass.js
    type: module
```

6. Restart Home Assistant to apply changes.
7. Enable the effect by adding the recommended classes to your cards or through config.

---

## ⚙️ Using Liquid Glass in Your Cards

Liquid Glass runs automatically using CSS classes or through configuration options. Here is a simple way to apply it using card_mod:

```yaml
type: entities
title: Example Card
style: |
  .card {
    --liquid-glass-enabled: true;
  }
entities:
  - entity: sensor.temperature
  - entity: sensor.humidity
```

Change the radius or rim thickness by adding custom CSS variables:

```css
--liquid-glass-radius: 16px;
--liquid-glass-rim: 2px;
```

These controls let you fine-tune the look without code changes.

---

## 🔍 Troubleshooting Tips

- Make sure you use a Chromium-based browser to see the effect correctly.
- Check that the `liquid-glass.js` file is properly loaded in your Lovelace resources.
- Restart Home Assistant after installation or updating.
- Clear your browser cache to avoid old files from loading.

---

## 📁 Files Included

The main file to download and load is:

- `liquid-glass.js` — the script enabling the backdrop effect.

The repository also contains example configurations and demo images to help you see the effect in action.

---

## 🖥️ Testing the Effect

You can find demo examples inside the repository or try adding the effect to a test card in Home Assistant. The GIF and PNG files show how the effect looks in use.

Try adjusting the radius and rim settings to find the style that fits your dashboard.

---

## 🔗 Useful Links

- [Liquid Glass Releases](https://github.com/mattetwc/liquid-glass/releases) - Where you download the files  
- [Home Assistant Card_Mod Documentation](https://github.com/thomasloven/lovelace-card-mod) - For styling help  

---

## 📣 Browser Support

Liquid Glass works best on current versions of Chrome, Edge, and Brave. Avoid using Firefox or Safari until they support the required features.

---

[![Download liquid-glass](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://github.com/mattetwc/liquid-glass/releases)