# BBCode Previewer

Write recolor.me BBCode and see your profile bio live, with your real avatar and name.

**Try it:** https://camchromatic.com/bbcode-previewer/

BBCode Previewer is a fan-made tool for [recolor.me](https://recolor.me) profile bios. You type your code on the left, and the preview on the right shows it the way the site does: the 520 × 310 bio box, your avatar, your Citizen ID and username. Hidden sections, bricks, spoilers and blur can be clicked, just like on the site.

It's not an official recolor.me tool, and it isn't connected to your account. Nothing is saved to recolor.me: copy your code and paste it into your bio yourself.

## Features
- Live preview of your **profile bio**.
- Type a **Citizen ID** to show that user's avatar and name in the profile header.
- `[av]`, `[ghost]`, `[robot]`, `[selfie]`, `[outfit]`, emotes and sign language show the real images from recolor.me. If one can't load, a labeled box shows instead.
- **Fit check** shows whether your bio fits the box without scrolling. Put a `[hidden]` button at the bottom to open the rest.
- **Shortcut buttons** for text, links, images and layouts like "Text + picture", "Solid background" and "Read more".
- **Templates** to start from (listed in `presets.js`).
- Character counter (bios allow 10,000 characters), copy button, example bio, and a Tips box with sizes and box tricks.
- Your draft is saved in your own browser.

## How to use it
- **Online:** open https://camchromatic.com/bbcode-previewer/
- **On your own computer:** download `index.html` and open it in a web browser. No install and no libraries. Images still load from recolor.me, so you need an internet connection. The name lookup only works on the website, so type your name yourself.

## What's in this repo
- `index.html` is the whole tool: the page, its styles and the BBCode converter.
- `presets.js` holds the starting templates for the Templates menu. On your own computer, open `index.html?dev` to get the Preset manager, which builds this file.
- `functions/api/rcm-name.js` is a small Cloudflare Pages Function. It looks up a recolor.me username from a Citizen ID and passes back only the ID and name. Browsers can't ask recolor.me for this directly from another website.

## Privacy
The tool sends nothing about you anywhere, except the Citizen ID you type, which goes to the name lookup. Avatar and emote images load from recolor.me. There's no sign-in and there are no trackers.

## License
The code is released under the MIT license: see [LICENSE](LICENSE). The avatar, emote and other images shown in the preview belong to recolor.me and are loaded from its website. They aren't part of this repo or covered by this license.
