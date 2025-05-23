```markdown

# 🌐 Responsive Navbar with Tailwind CSS

Hey there! 😊  
I built this navbar as part of my Tailwind CSS learning journey — and oh boy, it's not just any navbar... it's packed with ✨ **cool features** like dropdowns, active links, and even a dark mode toggle! I’m super excited to share how it works and what I learned. Let's gooo 🚀

---

## 🔧 Features I Built

### ✅ Active Link State
To show which page the user is on, I made the "Home" link bold and purple!

```html
<a href="#" class="text-purple-700 font-semibold">Home</a>
```

This is how websites subtly tell users, “Hey! You’re right here 👈”

---

### 📂 Dropdown Menu on Hover

I created a dropdown under the "Projects" link using Tailwind’s group-hover magic:

```html
<div class="relative group">
  <a href="#" class="text-gray-700 hover:text-purple-600 font-medium">Projects</a>

  <div class="absolute left-0 mt-2 w-40 bg-white shadow-md rounded-md hidden group-hover:block z-10">
    <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">Websites</a>
    <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">UI Components</a>
    <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100">Experiments</a>
  </div>
</div>
```

#### 🧠 Things I learned:

- `relative` on the parent + `absolute` on the dropdown = perfect dropdown positioning.
- `group-hover` is a superhero! 🦸‍♀️ It lets you control child visibility when hovering over the parent.

---

### 🌙 Dark Mode Toggle (with JavaScript)

Because… why not? 😎

```html
<button id="darkToggle" class="ml-4 px-3 py-1 text-sm border border-gray-300 rounded-md hover:bg-gray-100">
  Toggle Dark 🌙
</button>
```

```js
<script>
  const toggleBtn = document.getElementById('darkToggle');
  const body = document.body;

  toggleBtn.addEventListener('click', () => {
    body.classList.toggle('bg-white');
    body.classList.toggle('bg-gray-900');
    body.classList.toggle('text-white');
  });
</script>
```

I’ll improve this later using `dark:` classes with Tailwind config — but this is a fun start!

---

## 📱 Responsive Design

Tailwind makes it super easy to make things look good on all screen sizes!  
I used:

```html
<div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
```

### 🤔 What does this mean?

| Class        | What it does                                                                 |
|--------------|------------------------------------------------------------------------------|
| `max-w-7xl`  | Limits content width to a large max size so it doesn’t stretch on big screens |
| `mx-auto`    | Horizontally centers the content block                                        |
| `sm:px-6`    | Adds 1.5rem (24px) horizontal padding on small screens and up                 |
| `lg:px-8`    | Adds 2rem (32px) horizontal padding on large screens and up                   |

This helps in building consistent, responsive layouts 📱➡💻

---

## 🧱 Folder Structure

Here’s how I organized this in my project:

```
src/
├── navbar/
│   ├── index.html
│   └── README.md
├── buttons/
├── typograph/
└── ...
dist/
└── style.css (compiled Tailwind output)
```

> Each component folder has its own `README.md` and HTML file — so I can grow my design system over time like a pro 🌱

---

## 🌈 What I Want to Add Next

- [ ] Mobile menu toggle for smaller screens (hamburger menu 🍔)
- [ ] Transition effects on dropdown
- [ ] Real dark mode using Tailwind's `dark:` utilities

---

## 🧠 Final Thoughts

This navbar might look simple, but it taught me **so much**:

- Responsive layouts
- How dropdowns actually work
- Tailwind’s smart utility classes
- A little JavaScript makes things interactive!

If you're learning Tailwind too — let’s be build buddies 🤜❤️  
Feel free to fork, try it, or suggest ideas!

---

Made with 🧠 and 💜 by [Yukti](https://github.com/yukti-says)
```
