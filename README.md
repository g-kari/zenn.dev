# Zenn.dev Repository

This repository is set up for managing [Zenn.dev](https://zenn.dev/) articles and books using the official [zenn-cli](https://zenn.dev/zenn/articles/zenn-cli-guide) tool.

## Repository Structure

```
.
├── articles/          # Directory for article files
├── books/            # Directory for book files
├── .gitignore        # Git ignore file
└── README.md         # This file
```

## Prerequisites

- Node.js (version 14 or later)
- npm or yarn

## Setup

This repository is already initialized with the Zenn CLI structure. You can start using it immediately without additional setup.

## Usage

### Creating Content

Create a new article:
```bash
npx zenn-cli new:article
```

Create a new book:
```bash
npx zenn-cli new:book
```

### Managing Content

List all articles:
```bash
npx zenn-cli list:articles
```

List all books:
```bash
npx zenn-cli list:books
```

### Preview Content

Start the local preview server:
```bash
npx zenn-cli preview
```

The preview server will start at `http://localhost:8000` where you can view your articles and books locally before publishing.

### Publishing

To publish your content to Zenn.dev, push your changes to the main branch. Zenn.dev will automatically sync with your repository.

## File Naming Conventions

### Articles
- Article files should be placed in the `articles/` directory
- File names should follow the pattern: `[slug].md`
- Example: `articles/my-first-article.md`

### Books
- Book files should be placed in the `books/` directory
- Each book should have its own subdirectory
- Configuration file: `books/[book-name]/config.yaml`
- Chapter files: `books/[book-name]/[chapter-name].md`

## Resources

- [Zenn CLI Guide](https://zenn.dev/zenn/articles/zenn-cli-guide) - Official documentation
- [Zenn.dev](https://zenn.dev/) - Official website
- [Markdown Guide](https://zenn.dev/zenn/articles/markdown-guide) - Zenn's markdown syntax guide
