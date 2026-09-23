# Harriet Joseph: portfolio site

The source for my portfolio site: plain HTML, CSS and a little JavaScript. No framework and no build step, so it loads fast and any file can be edited directly on GitHub.

## Publish it (GitHub Pages)

1. Create a new **public** repository named exactly **`HattieSpartan.github.io`**.
2. **Add file → Upload files**, drag in **every file in this folder** (they're all loose, with no subfolders), then **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", pick **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute or two the site is live at **https://hattiespartan.github.io/**.

If you publish under a different address (e.g. a custom domain), update `SITE_URL` everywhere it appears: the `<link rel="canonical">` and `og:` tags at the top of each `.html` file, `sitemap.xml` and `robots.txt`.

## Files

| File | What it is |
|---|---|
| `index.html` | Home: introduction, how I work, featured work, skills, research, contact |
| `work.html` | All work: featured case studies plus smaller projects |
| `case-*.html` | One page per case study (Problem → Approach → Analysis → Result → Why it matters → Tools) |
| `research.html` | MSc research (in progress) |
| `about.html` | Professional story |
| `resume.html` | Resume summary and CV download |
| `Harriet_Joseph_CV.pdf` | Web version of the CV (no phone number or referee contacts) |
| `style.css` | All styling. Colours and fonts are set at the top in `:root` |
| `main.js` | Mobile menu, gentle fade-ins, case-study contents highlight |
| `img-*.png/jpg` | Charts and figures used in case studies |
| `og-image.png` | Preview image shown when the link is shared on LinkedIn/WhatsApp |
| `404.html`, `sitemap.xml`, `robots.txt`, `favicon.svg` | Housekeeping and SEO |

## Things to fill in (search the files for `PLACEHOLDER`)

- `work.html`: the churn project's best model score, the Bella chatbot's GitHub link, and a link for the big-data pipeline once published.
- `case-sentiment-lstm.html`: a "Try the live app" button once the Streamlit app is deployed.
- `research.html`: final methods, data source and supervisor once agreed.
- `about.html`: optional professional photo (save it as `harriet.jpg` and un-comment the line).

## Editing tips

- The header and footer are repeated in every page. If you change a nav link, change it in each `.html` file.
- To add a new case study, copy an existing `case-*.html` file, change the text, and add a card for it on `work.html` (and on `index.html` if it should be featured).
- Update the CV by replacing `Harriet_Joseph_CV.pdf` with a file of the same name.
