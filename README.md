
# Tailwind CSS v4 



### 1. Base Layout Structure

We create the base layout with a vertical flex container:

```html
<div class="flex min-h-screen flex-col bg-white dark:bg-gray-800">
  <!-- Content here -->
</div>
````

* `min-h-screen`: makes the container full height
* `flex-col`: stacks children vertically
* `dark:bg-gray-800`: sets dark mode background

---

### 2. Building the Navbar

We create a responsive navigation bar with:

* Left-aligned title
* Right-aligned links
* A dark mode toggle

```html
<div class="flex justify-between px-6 py-4 shadow-lg bg-white dark:bg-gray-900 text-black dark:text-white">
  <h1 class="text-lg font-bold">MyWebsite</h1>
  <nav class="flex gap-4">
    <a href="#">Home</a>
    <a href="#">Blog</a>
    <a href="#">Contact</a>
    <button onclick="document.documentElement.classList.toggle('dark')">Toggle Theme</button>
  </nav>
</div>
```

✅ `dark:` classes allow us to define alternate styles in dark mode
✅ We use `document.documentElement.classList.toggle('dark')` to trigger the theme

---

### 3. Hero Section

Next, we add a centered hero section with a heading and supporting paragraph.

```html
<section class="text-center py-24 px-6">
  <h2 class="text-4xl font-semibold mb-4">Welcome</h2>
  <p>This is the main content area of the website.</p>
</section>
```

You’ll learn:

* How to use **text utilities** for typography
* How to control **spacing** using `py`, `px`, and `mb`

---

### 4. Features Grid

Now we build a responsive grid of feature cards using Tailwind’s **grid** and **hover effects**:

```html
<section>
  <h2 class="text-xl font-semibold text-center mb-4">Features</h2>
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 px-6">
    <div class="p-4 rounded bg-gray-200 dark:bg-neutral-800 hover:bg-gray-300 dark:hover:bg-neutral-700 transition-colors">Feature 1</div>
    <!-- ...Repeat for more cards -->
  </div>
</section>
```

You’ll learn:

* Responsive grid syntax (`sm:`, `md:` breakpoints)
* Hover states for dark and light modes
* Consistent card styling with padding, rounded corners, and background color

---

### 5. Footer

We wrap up with a simple footer styled to match the header.

```html
<footer class="mt-4 py-6 text-center text-sm bg-white dark:bg-gray-900 text-gray-600 dark:text-gray-400 border-t dark:border-white/10">
  &copy; 2025 My Website. All rights reserved.
</footer>
```

You’ll learn:

* How to use **border and text utilities** in both themes
* How to apply layout spacing with `mt`, `py`

---

### 6. Smooth Transitions

To make dark mode feel polished, we apply transitions to the body or outer div:

```html
<body class="transition-colors duration-300">
```

This allows for a fade effect when toggling themes.

---

### 7. Final Touches & Recap

By the end of this course, you’ve learned how to:

* Build clean layouts using utility classes
* Make designs mobile-friendly using responsive breakpoints
* Support light and dark themes
* Create interactive hover styles
* Build a real-world landing page using Tailwind CSS v4

---

## ✅ Final Code Preview

Your final site includes:

* A full-page layout
* Responsive navigation and grid
* A hero section with styled text
* A working light/dark toggle

Everything is done **without custom CSS** — just Tailwind v4 utility classes.

---

## 🧪 Try It Online

You can experiment with the full code here:
👉 [Tailwind Play](https://play.tailwindcss.com)

---


