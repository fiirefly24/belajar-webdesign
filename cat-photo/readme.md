# 🧠 Understanding the Basics of Semantic HTML

## 1. What is Semantic HTML?

Semantic HTML means using tags that describe **what the content is**, not just how it looks.

For example:

- `<h1>` says: "This is the main heading."
- `<nav>` says: "This is a navigation bar."
- `<main>` says: "This is the main content of the page."

These help with:

- **Accessibility** (screen readers understand better)
- **SEO** (search engines know what’s important)
- **Code readability** (easier for developers to understand)

---

## 🔹 When to Use `<main>`

✅ **Purpose:**  
The `<main>` tag represents the **primary content** of the document.

✅ **Where to Use It:**

- Wrap your main content area inside `<main>`
- There should be **only one** `<main>` per page
- Should **not** be nested inside `<header>`, `<footer>`, or other sections

✅ **Example:**

```html
<body>
  <header>...</header>

  <main>
    <h1>Welcome to My Blog</h1>
    <p>This is the main article...</p>
  </main>

  <footer>...</footer>
</body>
```

---

## 🔸 When to Use `<section>`

✅ **Purpose:**  
A `<section>` is a **thematic grouping of content**.  
It's used when you want to group related content together on the page.

✅ **When to Use It:**

- To divide your `<main>` into logical parts (e.g., introduction, features, contact)
- Each section should have a heading (`<h1>`–`<h6>`) to define its purpose
- Think of it like chapters in a book or sections in an article

✅ **Example:**

```html
<main>
  <section>
    <h2>About Me</h2>
    <p>I'm a web developer...</p>
  </section>

  <section>
    <h2>My Projects</h2>
    <ul>
      <li>Project 1</li>
      <li>Project 2</li>
    </ul>
  </section>
</main>
```

---

## 🔺 When to Use `<div>`

✅ **Purpose:**  
A `<div>` is a **generic container** for grouping elements without any semantic meaning.

✅ **When to Use It:**

- When you need to group elements for styling purposes only (like layout, spacing, etc.)
- When no other semantic tag fits (but try to avoid this if possible)

❌ **Not Recommended:**  
Don’t overuse `<div>` when there’s a more appropriate semantic tag available (like `<section>`, `<article>`, `<nav>`, etc.)

✅ **Example:**

```html
<div class="card">
  <img src="cat.jpg" alt="Cat" />
  <p>Cute cat photo</p>
</div>
```

You might use this in CSS to style all cards the same way.

---

## 🔄 How to Be Consistent

Here are some best practices to keep your code clean and consistent:

| Best Practice          | Explanation                                                                              |
| ---------------------- | ---------------------------------------------------------------------------------------- |
| `<main>`               | Always one per page. Wrap your core content in it.                                       |
| `<section>`            | Use for major content blocks. Always include a heading.                                  |
| `<div>`                | Only use when you need a generic container for styling. Avoid overuse.                   |
| Nesting                | Keep nesting shallow. Too many layers make code hard to read.                            |
| Indentation            | Always indent properly. Most editors can auto-format for you.                            |
| Meaningful IDs/Classes | Name them based on their purpose (e.g., `class="navigation"` instead of `class="nav1"`). |

---

## 📝 Summary Table

| Tag         | Purpose                      | Should Have Heading? | Best For                                              |
| ----------- | ---------------------------- | -------------------- | ----------------------------------------------------- |
| `<main>`    | Main content of the page     | ❌                   | The primary part of your website                      |
| `<section>` | Thematic grouping of content | ✅                   | Grouping related paragraphs, lists, images            |
| `<div>`     | Generic container            | ❌                   | Styling layouts or fallback when no better tag exists |

# 🧩 List of All Semantic Tags in HTML5

Semantic tags help describe the **purpose and meaning** of content, improving accessibility, SEO, and code readability.

---

## 🔹 `<main>`

**Represents the main content of the document**

- Should be used once per page
- Contains the primary content

```html
<main>
  <h1>Welcome to My Blog</h1>
  <p>This is the main article...</p>
</main>
```

---

## 🔹 `<header>`

**Introduces a section or the whole page**

- Often contains headings, navigation, logos

```html
<header>
  <h1>My Website</h1>
  <nav>...</nav>
</header>
```

---

## 🔹 `<footer>`

**Contains info about author, copyright, contact info, etc.**

- Usually at the bottom of a page or section

```html
<footer>
  <p>&copy; 2025 CatPhotoApp</p>
</footer>
```

---

## 🔹 `<nav>`

**Defines a set of navigation links**

- Used for menus, site navigation
- Avoid using it for minor internal links

```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
  </ul>
</nav>
```

---

## 🔹 `<section>`

**A standalone section of a document**

- Groups related content (e.g., chapters, topics)
- Always include a heading (`<h1>`–`<h6>`)

```html
<section>
  <h2>About Me</h2>
  <p>I'm a web developer...</p>
</section>
```

---

## 🔹 `<article>`

**Self-contained composition that can be distributed independently**

- Useful for blog posts, news articles, forum posts

```html
<article>
  <h3>Why Cats Are Great Pets</h3>
  <p>Cats are low maintenance and very affectionate...</p>
</article>
```

---

## 🔹 `<aside>`

**Content indirectly related to the main content**

- For sidebars, pull quotes, ads, or additional info

```html
<aside>
  <p>Did you know? Cats spend up to 70% of their lives sleeping.</p>
</aside>
```

---

## 🔹 `<figure>`

**Self-contained content like images, diagrams, or code snippets**

- Often paired with `<figcaption>`

```html
<figure>
  <img src="cat.jpg" alt="Cute cat" />
  <figcaption>A cute orange cat lying on its back</figcaption>
</figure>
```

---

## 🔹 `<figcaption>`

**Caption/description for a `<figure>`**

- Helps describe the content of a figure

```html
<figure>
  <img src="chart.png" alt="Sales chart" />
  <figcaption>Sales Performance Q1 vs Q2</figcaption>
</figure>
```

---

## 🔹 `<time>`

**Represents a date or time**

- Makes it easier for search engines and screen readers to parse dates

```html
<p>Published on <time datetime="2025-04-05">April 5th, 2025</time></p>
```

---

## 🔹 `<mark>`

**Highlights text for reference or emphasis**

- Visually marks important parts of the content

```html
<p>You should <mark>read this carefully</mark> before proceeding.</p>
```

---

## 🔹 `<summary>`

**Summary, caption, or legend for a `<details>` element**

- Appears as a clickable title for the details

```html
<details>
  <summary>Click to read more</summary>
  <p>This is hidden until clicked.</p>
</details>
```

---

## 🔹 `<details>`

**Represents a disclosure widget from which the user can expand or collapse content**

- Used with `<summary>`

```html
<details>
  <summary>Technical Details</summary>
  <p>Version: 1.0 | Last Updated: April 5, 2025</p>
</details>
```

---

## 🔹 `<dialog>`

**Represents a dialog box or window**

- Can be used for modals or popups

```html
<dialog open>
  <p>Are you sure you want to delete this?</p>
</dialog>
```

---

## 🔹 `<meter>`

**Scalar measurement within a known range**

- E.g., progress bars, disk usage

```html
<label>Storage Used: <meter value="0.8">80%</meter></label>
```

---

## 🔹 `<progress>`

**Completion progress of a task**

- E.g., uploading a file, form submission

```html
<label>Loading... <progress value="70" max="100">70%</progress></label>
```

---

## 🛠️ Non-Semantic Tags (Non-Descriptive)

These don't describe the content — they just group or style things:

| Tag      | Description                                     |
| -------- | ----------------------------------------------- |
| `<div>`  | Generic container for layout or styling         |
| `<span>` | Inline container for styling small bits of text |

Use these only when no semantic tag fits.

---

## ✅ Best Practices

- Use **semantic tags first** — they improve accessibility and SEO
- Only use `<div>` or `<span>` if necessary — prefer semantic tags whenever possible
- Group related content into `<section>`, `<article>`, or `<aside>`
- Use `<header>` and `<footer>` consistently across your pages
- Use `<nav>` for major navigation menus — avoid using it for minor links
- Use `<figure>` and `<figcaption>` for media elements to improve context

---

## 🎯 Example Using Multiple Semantic Tags

Here’s how you might use several semantic tags together:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>CatPhotoApp</title>
  </head>
  <body>
    <header>
      <h1>CatPhotoApp</h1>
      <nav>
        <ul>
          <li><a href="#photos">Cat Photos</a></li>
          <li><a href="#lists">Cat Lists</a></li>
          <li><a href="#form">Cat Form</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section id="photos">
        <h2>Cat Photos</h2>
        <p>Everyone loves <a href="#">cute cats</a> online!</p>
        <a href="#"
          ><img src="#" alt="A cute orange cat lying on its back."
        /></a>
      </section>

      <section id="lists">
        <h2>Cat Lists</h2>
        <article>
          <h3>Things cats love:</h3>
          <ul>
            <li>catnip</li>
            <li>laser pointers</li>
            <li>lasagna</li>
          </ul>
        </article>
        <aside>
          <p>Did you know? Cats spend up to 70% of their lives sleeping.</p>
        </aside>
      </section>

      <section id="form">
        <h2>Cat Form</h2>
        <form action="#">
          <!-- Your form fields go here -->
        </form>
      </section>
    </main>

    <footer>
      <p>No Copyright - <a href="#">freeCodeCamp.org</a></p>
    </footer>
  </body>
</html>
```

Let me know if you'd like this saved as a downloadable `.md` file or added to your collection! 💪
