# Bohemian Jewel — How to Edit & Publish Your Site

Your whole website is one file: **`index.html`**. You can open it any time by double-clicking it — it opens in your web browser. That's your live preview.

You don't need any special software. To make changes, open `index.html` in a plain text editor (on Mac: right-click → Open With → TextEdit; or use the free app **VS Code**).

---

## How editing works

Throughout the file you'll see comments in capitals like `<!-- EDIT ME: ... -->`. These mark exactly what to change. You only edit the text between the tags, not the tags themselves.

### Change your text
Find the bit you want to change (headline, about story, piece names, prices) and type over it. For example:

```
<h3>Willow Earrings</h3>
```
Change **Willow Earrings** to your piece's name. Leave the `<h3>` and `</h3>` alone.

### Add your photos
1. Make a folder called **`images`** next to `index.html`.
2. Put your photos in it (e.g. `willow-earrings.jpg`).
3. In the file, find a piece's placeholder line:
   ```
   <div class="placeholder">Your photo here</div>
   ```
   and replace it with:
   ```
   <img class="photo" src="images/willow-earrings.jpg" alt="Willow Earrings">
   ```
Tip: photos that are taller than they are wide (portrait) look best. Keep them a similar shape for a tidy grid.

### Add more pieces
Copy one whole `<article class="piece"> ... </article>` block and paste it below the others, then edit the name, materials, price, and photo.

### Hide prices for now
Delete the line `<p class="price">$68</p>` from any piece you don't want to show a price on.

### Change your brand colours
Near the top, in the `:root { }` section, change the colour codes (e.g. `--gold: #b08d57;`). You can pick new colours at a site like coolors.co.

---

## Making the contact form actually reach you

Right now the **Enquire** form opens the visitor's own email app addressed to `hello@bohemianjewel.com`. Two things to do:

1. Change that address to your real email (find `mailto:hello@bohemianjewel.com`).
2. **Better option for later:** sign up free at **formspree.io**, and they'll give you a line to paste in so enquiries land in your inbox automatically without the visitor needing an email app. I can set this up with you when you're ready.

The **newsletter** box is a placeholder for now — when you're ready to collect emails properly, a free tool like **Mailchimp** or **Beehiiv** gives you a form to drop in. Just ask and I'll wire it up.

---

## Publishing it online (free)

Your site is ready to go live. The easiest free options:

- **Netlify Drop** (netlify.com/drop) — drag your whole Bohemian folder onto the page and it's live in seconds. Free.
- **Cloudflare Pages** or **GitHub Pages** — also free, a little more setup.

To use your own domain (e.g. `bohemianjewel.com`): buy the domain (~$15/year from Namecheap or Cloudflare), then connect it in your hosting tool's settings. I can walk you through this step by step.

---

## Adding a real shop later

When you're ready to sell directly, the cleanest path is to move this design onto a platform with built-in checkout (Squarespace or Shopify), or add a lightweight "buy button" tool (like Snipcart) to this exact site. Either way your design and content carry over — nothing here is wasted. Just ask and we'll plan that step.

---

**Need a hand with any of this?** Tell me what you want to change and I'll edit the file for you directly.
