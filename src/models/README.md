# 🧩 Tailwind CSS Modals Collection

This folder contains beautiful, responsive modal components built using **Tailwind CSS**. Each modal is interactive and showcases different UI scenarios – from login forms to confirmation dialogs.

---

## 📁 Folder Structure

modals/
├── login-modal.html
├── confirm-delete-modal.html
├── login-modal.png
├── confirm-modal.png
└── README.md



---

## 🔐 1. Login Modal

A modal popup with a clean login form inside.

### ✅ Features:
- Smooth fade-in effect
- Centered form
- Fields: email, password
- Submit + Close buttons
- Responsive design

### 💡 Tailwind Classes Used:

| Class | Purpose |
|-------|---------|
| `fixed inset-0` | Fullscreen modal |
| `bg-black bg-opacity-50` | Overlay |
| `flex justify-center items-center` | Center the modal |
| `rounded-lg shadow-xl` | Card effect |
| `focus:outline-none` | Input accessibility |
| `hover:bg-blue-700` | Button hover effect |

### 🖼️ Screenshot:

![Login Modal](./login-modal.png)

---

## ❗ 2. Confirm Delete Modal

A warning-styled modal to confirm destructive actions.

### ✅ Features:
- Bold warning icon (⚠️)
- Clear prompt: "Are you sure?"
- Red `Delete` button
- Cancel to dismiss
- Click outside to close

### 💡 Tailwind Classes Used:

| Class | Purpose |
|-------|---------|
| `text-red-600` | Visual warning |
| `border-l-4 border-red-500` | Emphasis |
| `bg-white rounded-md` | Modal card |
| `transition ease-in-out` | Smooth animation |
| `hover:bg-red-700` | Button hover warning |

### 🖼️ Screenshot:

![Confirm Modal](./confirm-modal.png)

---

## 🧠 JavaScript Logic (shared for all modals)

```js
// Basic open-close modal logic
const openBtn = document.getElementById('openModal');
const closeBtn = document.getElementById('closeModal');
const modal = document.getElementById('modalOverlay');

openBtn.addEventListener('click', () => modal.classList.remove('hidden'));
closeBtn.addEventListener('click', () => modal.classList.add('hidden'));

window.addEventListener('click', (e) => {
  if (e.target === modal) modal.classList.add('hidden');
});


🧡 Built with Tailwind CSS
✨ Created by Yukti Sahu