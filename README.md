# book-club-website
Website for book club

## How to Add Content

### 1. Add a New Member Profile
1. Go to `src/profiles/` and create a new file named `profile-<name>.html` (replace `<name>` with the member's name, all lowercase).
2. Use one of the existing profile files (e.g., `profile-amanda.html`) as a template. Update the `<title>`, `<h1>`, and profile content as needed.
3. In `src/index.html`, find the `<ul class="members-list">` under the `#members` section. Add a new `<li>` entry linking to the new profile, e.g.:
   ```html
   <li><a href="profiles/profile-yourname.html">yourname</a></li>
   ```

### 2. Add a New Book
1. Add the book cover image to `src/imgs/` (recommended size: similar to existing covers, e.g., `the_bell_jar.jpg`).
2. In `src/index.html`, find the `<div class="books-list">` under the `#books` section. Add a new book entry using the following format:
   ```html
   <div class="book-item">
     <a href="blogs/blog-bookname.html"><img src="imgs/bookname.jpg" alt="Book Name cover" class="book-cover"></a>
     <div><a href="blogs/blog-bookname.html">Book Name</a></div>
   </div>
   ```
   - Replace `bookname` and `Book Name` with the appropriate values.
   - Make sure the image filename and blog filename match your new book.

### 3. Add a New Blog Post
1. Go to `src/blogs/` and create a new file named `blog-<bookname>.html` (replace `<bookname>` with the book's name, all lowercase and hyphens for spaces).
2. Use `blog-belljar.html` as a template. Update the `<title>`, `<h1>`, and blog content as needed. Each blog post can have multiple entries, each in a `<div class="blog-post">`.
3. Make sure the blog filename matches the link you added in the Books section of `index.html`.

---

**Tip:**
- Keep file naming consistent (lowercase, hyphens for spaces).
- Use the same HTML structure as the provided templates for a consistent look.
