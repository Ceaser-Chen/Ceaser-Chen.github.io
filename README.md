# Yunyue Chen — academic website

Personal website using the official [Academic Pages](https://github.com/academicpages/academicpages.github.io) default theme, based on upstream commit `9e19e6318817bd3a6060a76d5af98124d394f3a0`.

This version uses information already public at https://sites.google.com/view/yunyuechen and the owner's explicitly approved homepage and job market paper content. The homepage contains only three short paragraphs. Research contains the job market paper, awards and selected central bank presentations. The CV page displays lossless page previews rendered from the owner-approved public CV and provides links to view or download the unchanged original PDF.

## Update content

- Homepage: `_pages/about.md`
- Research page: `_pages/research.md`
- Sidebar information: `_config.yml`
- Navigation: `_data/navigation.yml`
- CV page: `_pages/cv.md`
- Approved public CV: `files/Yunyue_Chen_CV.pdf`
- CV page previews: `files/Yunyue_Chen_CV_page_1.png` and `files/Yunyue_Chen_CV_page_2.png` (144 dpi, lossless)
- Original profile photo: `images/yunyue-chen.jpg`

Academic Pages remains the base theme. `_sass/layout/_profile.scss` implements the agreed compact portrait, wider text column, mobile layout, and footer in document flow. The navigation includes Home, Research and CV. Keep `site_theme: default` in `_config.yml`.

## Publish on GitHub Pages

1. Create the public repository `Ceaser-Chen.github.io` in the `Ceaser-Chen` account and upload this source, including `.github/workflows/jekyll.yml`.
2. Set **Settings → Pages → Source → GitHub Actions**.
3. Push to `main` or `master`, or run **Publish Yunyue Chen website** from the Actions tab.
4. After the workflow succeeds, the website is available at https://ceaser-chen.github.io/.

Subsequent commits publish automatically. Deployment has not been confirmed until a successful GitHub Pages workflow is observed.

## Local build

Requires Ruby 3.4, Bundler, and Node.js.

```sh
bundle install
npm install
npm run build:js
bundle exec jekyll serve --host 127.0.0.1
```

## Future additions

Add publications or update the public CV only after the owner supplies and approves the exact public content. Do not upload the private source CV or infer permission from its contents. PDF files are ignored except for `files/Yunyue_Chen_CV.pdf`, which contains only the exact public CV approved by the owner.

Academic Pages and Minimal Mistakes attribution and the upstream MIT license are preserved.
