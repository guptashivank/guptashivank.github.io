# Copilot Instructions for leonidk.github.io

## Overview
This repository is built on a fork of **Jekyll Now** and serves as a static site generator for GitHub-hosted blogs. The design is a modification of Jon Barron's website, repurposing old markdown posts. The main components include:
- **Jekyll** for static site generation
- **SCSS** for styling
- **HTML layouts** for structuring content

## Architecture
- **_layouts/**: Contains layout templates like `default.html` and `post.html` that define the structure of the pages.
- **_posts/**: Contains markdown files for blog posts, which are processed by Jekyll to generate HTML.
- **style.scss**: The main stylesheet that includes base rules and imports for styling.
- **Scripts**: `_make_favicon.sh` and `_make_thumbnails.sh` automate the creation of favicons and thumbnails, respectively.

## Developer Workflows
- **Building the Site**: Run `jekyll build` to generate the static site from markdown files.
- **Serving Locally**: Use `jekyll serve` to preview the site locally.
- **Generating Thumbnails**: Execute `_make_thumbnails.sh` to create thumbnail images for posts.
- **Creating Favicon**: Run `_make_favicon.sh` to generate the favicon from the specified image.

## Project Conventions
- **Markdown Posts**: Follow the naming convention `YYYY-MM-DD-title.markdown` for posts in the `_posts/` directory.
- **Thumbnails**: Store thumbnails in the `tn/` directory, generated from original images in the `images/` directory.
- **Permalinks**: Set `permalink: /` in `_config.yml` to manage URL structure effectively.

## Integration Points
- **Google Analytics**: Integrated via the Google tag manager in the `default.html` layout for tracking site usage.
- **Image Handling**: Uses ImageMagick for image processing in scripts for favicons and thumbnails.

## External Dependencies
- **Jekyll**: Ensure Jekyll is installed and configured properly to build the site.
- **ImageMagick**: Required for running the thumbnail and favicon generation scripts.

## Conclusion
This document serves as a guide for AI coding agents to understand the structure, workflows, and conventions of the `leonidk.github.io` repository. For further details, refer to the specific files mentioned above.