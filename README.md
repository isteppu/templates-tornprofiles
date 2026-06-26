# Torn City - Custom Profile & Layout Templates

A curated collection of clean, responsive, and game-sanitizer-safe HTML/CSS templates for **Torn City**. These layouts are engineered specifically to pass through Torn's strict HTML parser without stripping style declarations, breaking layout baselines, or warping on mobile views.

---

## 📂 Repository Structure

| Folder | Description | Focus Area |
| :--- | :--- | :--- |
| `/faction-profiles` | Full recruitment sheets, announcements, and banners. | Layout hierarchy, heavy info scaling. |
| `/bazaar-profiles` | Clean shop interfaces and trading price-lists. | Grid simulation, clear numeric tables. |
| `/signatures` | Minimalist, casual personal bios & forum code blocks. | Small footprint, vertical line adjustments. |

---

## 🛠️ Key Design Philosophy

Torn's backend editor uses a strict whitelist sanitizer. To bypass bugs and template breaking, all layouts in this repository follow these strict rules:

* **No Grid/Flexbox Dependencies:** Traditional `display: flex` and `display: grid` often trip security protocols or fail to center correctly on older mobile views inside the app. We rely heavily on robust `display: inline-block` and `vertical-align: middle` configurations.
* **Inline-Style Driven:** Everything is encapsulated natively within tags to ensure external stylesheet stripping doesn't kill your visuals.
* **Mobile-Responsive Frameworks:** Images utilize fluid percentage boundaries (`max-width: 100%`) so they shrink cleanly across desktop browsers and the official Torn mobile application.

---

## 🚀 How to Deploy to Torn

1. Navigate to the relevant folder in this repo and open the layout file (e.g., `faction-banner.html`).
2. Copy the entire raw HTML code block.
3. Log into **Torn City** and navigate to the settings page for the area you are modifying (Faction Announcement, Bazaar Description, or Change Signature).
4. Locate the visual text editor toolbar and click the **Source** button (represented by `< >` or `Source`).
5. Paste your copied code directly into the source text-box window.
6. Click **Source** again to preview your interface, then hit **Save/Update**.

> ⚠️ **Important Asset Note:** Imgur heavily restricts third-party hosting requests ("hotlinking"). For any custom graphics or animated GIFs used in these layouts, it is highly recommended to host your images on alternative providers like **ImgBB** or **Postimages** to ensure they render reliably within the game canvas.

---

## 📝 Future Adjustments
* Add interactive transition classes for button hovers.
* Build out standard data-tables for trading price matrices.