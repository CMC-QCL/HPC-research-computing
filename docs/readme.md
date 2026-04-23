# docs folder

This folder contains the source files for the project website.
Jekyll, the website generator, uses these files to create our webpages.

- You edit Markdown files (`.md`) for posts.
- For website styling, HTML and CSS files are used. (`.html`/`.scss`).
- Jekyll turns these files into a website.
- The generated website files go into `_site`. You usually do not edit `_site` directly). For this blog, a Github Actions workflow will generate `_site`.

## Global mental model

- Content: `index.md`, `about.md`, `blog.md`, `_posts/`
- Structure: `_layouts/`, `_includes/`
- Styling: `assets/`
- Media: `images/`
- Settings: `_config.yml`


## Files and their functionality

- `_config.yml`
	Main site settings.
	This includes the title, description, navigation pages, and plugins.

- `index.md`
	The home page content.

- `about.md`
	The About page content.

- `blog.md`
	The page that lists blog posts.

- `_posts/`
	Blog post files.
	Each file name should follow this format: `YYYY-MM-DD-post-name.md`.
	Example: `2025-06-07-introduction-to-hpc-resources.md`.

- `_layouts/`
	Page templates.
	Layout files decide the structure around your content (title area, post metadata, body placement, etc.).

- `_includes/`
	Reusable page pieces (like header and footer).
	If you update a shared element here, all pages that use it will reflect that change.

- `assets/`
	Styling files (CSS/SCSS).
	`assets/main.scss` controls custom visual styles such as image sizing and footer text size.

- `images/`
	Image files used by pages and posts. Subdirectories may be used for organization.

- `slides/`
	Supporting slide files for tutorials or presentations.

## How pages get built

1. Markdown page/post files provide the text content.
2. Front matter at the top of each file (the `---` block) gives metadata like title, date, and layout.
3. Jekyll applies a layout from `_layouts/`.
4. Jekyll inserts shared pieces from `_includes/`.
5. Styles from `assets/main.scss` are applied.
6. Final static website files are generated in `_site`.

## Typical editing tasks

### Add a new blog post

1. Create a new file in `_posts/` using `YYYY-MM-DD-title.md`.
2. Copy front matter from an existing post and update:
	 - `title`
	 - `date`
	 - `permalink`
	 - `author`, `tags`, `categories` as needed
3. Write your content in Markdown below the front matter.
4. Add any images to `images/` and reference them from your post. Subfolders in `images/` is recommended for organization.

### Update navigation links

Edit `header_pages` in `_config.yml` to control which top navigation pages appear.

### Change site-wide footer content

Edit `_includes/footer.html` and/or footer values in `_config.yml` (`footer_address`, `footer_email`, `description`).