# 🌈 Typography Trial with Tailwind – Hello Yukti! 💜

## 📅 Date: May 20, 2025  
## 📁 Folder: `/typography/index.html`

---

## 🐣 What I Did Today

So today, I tried something super exciting in my web development journey — **I used Tailwind CSS to make my first ever styled text appear on a webpage!**

And guess what? It said:

> **"Hello Yukti!"**  
> ...in a super pretty purple font 😍✨

---

## 🧠 What I Learned (aka the ‘Ohh now I get it!’ moments)

1. **Tailwind needs to SEE your files**
   - At first, Tailwind didn’t show anything. I was confused like, “Where’s my purple text?”
   - Then I realized Tailwind wasn’t seeing my files because I didn’t tell it where to look.
   - So in the file called `tailwind.config.js`, I added this:

     ```js
     content: ["./src/**/*.{html,js}"]
     ```

   - That means, “Hey Tailwind! Look inside all my folders inside `src` for HTML and JS stuff, okay?”

2. **Linking the CSS the right way**
   - My HTML page was in this long path: `src/typography/index.html`
   - And my final style file (Tailwind-made) was in `dist/style.css`
   - So I wrote this in the `<head>`:

     ```html
     <link rel="stylesheet" href="../../dist/style.css">
     ```

   - It’s like saying “walk two folders back, then open the CSS box 🎁!”

3. **Don’t write `<body>` twice 😅**
   - Oopsie! I wrote two `<body>` tags. Fixed it and now it works like a charm.

---

## 🖼️ What My HTML Looked Like

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
  <link rel="stylesheet" href="../../dist/style.css" />
</head>
<body class="bg-gray-100 min-h-screen flex items-center justify-center">
  <h1 class="text-3xl font-bold text-purple-600">Hello Yukti!</h1>
</body>
</html>
