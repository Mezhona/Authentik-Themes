# My Custom Authentik Themes

I wasn't a huge fan of the default Authentik look, so I messed around with some CSS to make these themes. One is for a retro Windows 95 vibe, and the other is a sci-fi terminal look (Alien/Nostromo style).

They are just CSS files, so they are easy to install and won't break your actual authentication logic.

## The Themes

### 1. Redmond 95
**Style:** Windows 95 / Classic Win32

This basically turns your dashboard into a Windows 95 desktop. I spent a lot of time getting the "3D" borders right (the raised and sunken gray edges) so it actually feels like the old OS.

* **Classic Colors:** Uses the specific Teal background and Silver grays from the 90s.
* **The Look:** Buttons, input fields, and cards all look like Windows controls.
* **Layout:** It fixes some of the spacing issues in the default layout so things sit side-by-side better.

![Redmond 95 Preview](https://github.com/user-attachments/assets/f18b0cbc-425e-460e-ab0a-e406194a4afa)

---

### 2. USCSS Nostromo (LV-426)
**Style:** Alien / Retro Terminal / Weyland-Yutani

This is a heavy "dark mode" theme inspired by the computers in *Alien*. It uses glowing green text, scanlines, and a few visual tricks to make it look like an old CRT monitor.

* **CRT Effects:** It has a slight flicker and scanlines overlay to give it that retro screen feel.
* **Fonts:** Uses `Michroma` and `Quantico` fonts to match the movie aesthetic.
* **Group Boxes:** I changed how the application groups look—now they are distinct boxes with the "Weyland-Yutani" style labels on top.
* **Alerts:** "Danger" buttons (like delete) glow red so you don't miss them.

![Nostromo Preview](https://github.com/user-attachments/assets/72cbf6a4-d12b-4491-9724-8ffa04df5451)

![Nostromo Detail](https://github.com/user-attachments/assets/8ac09200-547a-4495-93b2-208df9ebc2b3)
(Note: if you dont like the application groupings here, just dont add the last part (12. Dashboard Layout))

---

## How to Install

You don't need to mess with docker volumes or host files. You can just paste this right into the settings.

1.  Open the `.css` file for the theme you want and copy everything.
2.  Log in to Authentik as an Admin.
3.  Go to **System** -> **Brands**.
4.  Edit your brand.
5.  Scroll down to **Branding Settings**, find the **Custom CSS** box, and paste the code there.
6.  Hit **Update**.

*Note: You might need to force refresh (Ctrl+F5) to see the font changes properly.*

## Compatibility

I'm running this on **Authentik 2025.10.2** and it works fine on Chrome and Firefox. Since it's just CSS, it should be pretty safe to use, but obviously, things might look different if the Authentik team changes their layout in the future.

## License

Do whatever you want with this! It's public domain. Feel free to fork it, change the colors, or use it however you like.
