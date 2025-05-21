# ✨ Buttons Component — TailwindCSS

This folder contains all my button experiments using Tailwind CSS!

## 📚 What I Practiced:
- Primary Button (Blue)
- Hover effects
- Rounded corners & shadows
- Font weight & padding

## ✨ More Buttons I Built

- ✅ Green Success Button
- ❌ Red Danger Button
- 🧊 Gray Outline Button
- ⚡ Purple Icon Button with Emoji

Each button taught me new things like using `border`, `hover:bg`, and even using emoji as quick icons!


## 👀 Focus State

I learned how to use `focus:` with Tailwind!

- Makes buttons more accessible for keyboard users
- Looks cool with `focus:ring-4` and glow effects ✨

Example:
```html
<button class="bg-green-500 hover:bg-green-600 focus:ring-4 focus:ring-green-300 ...">Success</button>

## 🛑 Disabled and ⏳ Loading Buttons

I learned how to show when a button is:

- **Disabled** – can't be clicked, faded
- **Loading** – when something is processing

### 🔒 Disabled Button

```html
<button class="bg-gray-400 text-white ... opacity-50 cursor-not-allowed" disabled>
  Disabled
</button>

### Loading Button
```html
 <button class="bg-blue-500 text-white font-medium py-2 px-4 rounded-lg flex items-center gap-2" > <span class="animate-spin rounded-full h-4 w-4 border-t-2 border-b-2 border-white" ></span>Loading...</button>

Made with 💖 by Yukti  
