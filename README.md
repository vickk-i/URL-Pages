# URL Pages – Encode Your Website in a Link

## 🔍 About This Project

This project is a lightweight, client-side web tool that allows users to create and share full web pages directly encoded into URLs—no servers, no hosting, and no external storage needed.

### 🚀 Key Features
- Edit HTML, CSS, and JavaScript directly in a built-in editor.
- Instantly "publish" pages by sharing a single URL.
- No signups, no tracking, and completely free.
- Bookmarklet tool for cloning existing pages.
- Works entirely offline after loading.
- Minimal codebase with zero dependencies.

This was built as an exploration of how far you can push the concept of "the URL as a host." It’s an experiment in lightweight, censorship-resistant publishing.

## 🔐 Encryption Support

I integrated compatibility with [Link Lock](https://github.com/jstrieb/link-lock) to allow optional client-side encryption of the data embedded in the URL. This ensures that sensitive pages can be securely shared using a password-protected link.

## ⚙️ How It Works

URL Pages works by encoding the entire HTML/CSS/JS content of a page into a compressed and base64-encoded URL fragment.

- The **editor** takes your page content and converts it into a sharable URL.
- The **viewer** (main page) decodes this data and renders the web page.
- The **bookmarklet** allows you to quickly clone any live page into a URL-encoded format.

Since the data is stored in the `#hash` of the URL, it never leaves the client’s browser, preserving privacy and functionality.

## 📚 Example Use Cases

- Share quick web experiments without hosting.
- Build offline documentation or tools.
- Bypass censorship by hiding full pages in links.
- Archive static web pages.

## 🧠 Inspiration

This started out as a static CodePen-like editor, but I became intrigued by the idea of using the URL itself as a publishing medium. After a few experiments, I developed this proof-of-concept and realized how powerful and flexible this approach could be for small-scale web publishing.

## 📌 To-do / Future Enhancements

- Integrate a code editor like Ace or CodeMirror for better UX.
- Improve the bookmarklet’s performance and reliability.
- Explore URL compression (e.g., Brotli) to allow longer pages.
- Add more example templates and multi-page site support.
- Explore alternative encodings like base65536 for ultra-compressed URLs.

## ⚠️ Disclaimer

This is a proof of concept and not intended for large-scale websites or apps. It's best used for small tools, experiments, and creative expressions. Always test thoroughly and understand how the encoding works before using it for anything critical.

---
