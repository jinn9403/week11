+++
author = "David Evans"
draft = false
title = "Blogging Mechanics"
slug = "blogging"
+++

Here are some suggestions for how to create the class blog posts for
your assigned classes.

I believe each team has at least a few members with enough experience
using git and web contruction tools that following these instructions
won't be a big burden, but if you have other ways you want to build
your blog page for a topic let me know and we can discuss alternative
options.

- Install [Hugo](https://gohugo.io/).  Hugo is a static website
  generator that builds a site from Markdown pages.  (With homebrew on
  Mac OS X, this is easy: `brew update && brew install hugo`. From
  what I've heard, people are also able to use Hugo on linux and
  Windows without much difficulty, but I have not tried this myself.)

- [Fork the github repository for the course website](https://github.com/llmrisks/llmrisks.github.io/fork).  This is what is used to build the
  [https://llmrisks.github.io/](https://llmrisks.github.io/) site.  If you are
  working with multiple teammates on the blog post (which you probably
  should be), you can add write permissions for everyone to the forked
  repository.

- You should create your page in the `src/content/post/`
  subdirectory. You can start by copying an earlier file in that
  directory (e.g., `week1.md`) and updating the header section
  (between the `+++` marks) and replacing everything after that with
  your content.  Don't forget to **update the date** so your page will
  appear in the right order. You can put `draft = true` in the header,
  so your page will not appear on the course website until it is
  ready.

- You can use multiple files (but probably only one in
  the `post/` directory (this will show up as pages on the front
  list).  Use the `src/content/images` directory for images and the
  `src/content/docs` directory for papers.  Using images and other
  resources to make your post interesting and visually compelling is
  highly encouraged!
   
- Write the blog page using Markdown.  Markdown is a simple markup
  language that can be used to easily generate both HTML and other
  output document formats.  You can probably figure out everything you
  need by looking at previous posts, but for a summary of Markdown,
  see [Markdown: Syntax](https://daringfireball.net/projects/markdown/syntax).

- You can incorporate latex math into your markdown. Use `\\(` inline `\\)` for inline math, e.g., `\\( J_{min}\\}` and `$$ ... $$` for display math.

- Your post should include credits for any external material you use,
  especially for any images you incorporate that you didn't produce.

- Please include full references to the papers, and links to the most
  definitive source available (usually this is to arxiv or a
  conference site, but could be the author's page). You should include
  additional links to relevant and useful reference or code
  repositories. Its good to have an overview section at the beginning
  of the post with links to all the main papers covered, and then to
  have links in specific sections to what is being covered.

- To test the post, run `make develop` (in the `src/` subdirectory of
  your repository).  This starts the Hugo development server, usually
  on port 1313 (unless that port is already in use).  Then, you can
  view the site with a browser at `localhost:1313`.

- When you are ready, submit a pull request to incorporate your
  changes into the main repository (and public course website).  Also,
  send a message to me, so I know the post is ready to review.  At
  this stage, I will probably make some requests for improvements, and
  then will post the edited version to the course site.

