# Your interactive portfolio

## Open it

Double-click `index.html`. Keep it in the same folder as `styles.css`, `script.js`, `profile.jpg`, and `about.jpeg`. The site works locally without installing anything or connecting to the internet.

The preview opened in Codex uses a temporary local server. Its address works on this computer while that server is running; it is not a public website address.

## The three parts of a website

- **HTML is the content and structure.** `index.html` holds your headings, paragraphs, photographs, buttons, and links.
- **CSS is the appearance.** `styles.css` controls colors, spacing, phone layouts, and the rotating 3D sculpture.
- **JavaScript is the behavior.** `script.js` follows the pointer, tilts cards, reveals sections as you scroll, and remembers the motion preference.

## Your first edit: change a headline

1. Right-click `index.html` and open it with a text editor, such as Notepad.
2. Find `Less chaos.` and replace it with your preferred headline. Keep the surrounding `<h1>`, `<br>`, and `<em>` tags.
3. Save the file, then refresh the browser.

For example:

```html
<h1>Your operations.<br>My <em>focus.</em></h1>
```

Make one change at a time so you can see what it does.

## Change the colors

At the beginning of `styles.css`, change `--blue:#8eaaff` to another color, such as `--blue:#8ee8c0`. `--bg` controls the background, `--text` the main text, and `--muted` the secondary text. Keep enough contrast for easy reading.

## Understand and adjust the 3D motion

The orbit uses CSS `perspective`, `transform-style:preserve-3d`, `rotateX`, and `rotateY`. These put flat elements at different angles in a 3D scene. Gradients and shadows give the center sphere its depth.

Find `animation:turn 24s linear infinite` in the stylesheet. A smaller duration spins faster; a larger duration spins slower. Change the `counterturn 24s` duration to the same value so the center lettering stays aligned.

In `script.js`, the pointer position changes rotation variables such as `--rx` and `--ry`. The division by `16` controls how strongly the sculpture follows the pointer. Try `10` for a stronger effect or `25` for a gentler one.

Cards use the same idea with `--tx` and `--ty`. Touch visitors can scroll normally. The Motion button pauses animation, and the site respects the visitor's reduced-motion accessibility setting.

## Change photographs and contact links

Replace `profile.jpg` or `about.jpeg` with your own image using exactly the same filename, or edit each image's `src` in the HTML. Update its `alt` text to describe the photo.

For an email link, update both the visible text and its `href`:

```html
<a href="mailto:you@example.com">you@example.com</a>
```

Email buttons open the visitor's email app. This site does not submit messages through a server or store visitor information.

## Add another experience

Copy one complete `<details>...</details>` block inside the `timeline` section. Change its date, role, and description. The browser provides the expand/collapse interaction, including keyboard access.

## Before sharing

Check your dates, experience claims, email address, phone number, and social links. These were adapted from your original page. Keep only contact details you want publicly visible. Test the page on a phone and click each link.

## Put it online

This is a static website. A static website host can publish the folder's HTML, CSS, JavaScript, and images, then give you a public HTTPS address. A custom domain is optional and points to that hosting service. No database or backend is needed for the current version.

The site has not been published. When you choose a host, upload all five site files together and keep `index.html` at the site's root. Do not upload just the HTML file, because its styling, interactions, and images live beside it.

## Simple learning path

1. Edit a heading in HTML and refresh.
2. Change a color in CSS and refresh.
3. Adjust the orbit duration and compare the motion.
4. Add an experience entry.
5. Try the navigation, keyboard Tab key, motion toggle, and a narrow browser window.

You now have the basic edit → save → refresh workflow used to build websites.

## New interactive features

The project lab includes a clickable three-step concept demo and a Play workflow button. It is a visual demonstration, not an actual n8n execution. The background particles react to a mouse pointer; the top line shows reading progress. The existing Motion control pauses decorative animation.

### Add your actual n8n screenshot

The screenshot was not available when this ZIP was created. Save your screenshot as `n8n-project.png` beside `index.html`, then refresh. The project card will show it automatically and visitors can open it in a larger viewer. If you use a different image filename, change `projectImage` in `script.js`. Do not merely rename a JPEG extension to PNG; either export PNG or use the correct filename in the script.

Update “My n8n workflow” in the HTML with your actual project title and add a factual description. The sample three-step concept is separate from your real project.
