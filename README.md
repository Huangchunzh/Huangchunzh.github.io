# Personal academic website

A four-page website (Home, Research, CV, About me) in plain HTML and CSS. There is nothing to install and no build step: you edit the text, upload the files to GitHub, and GitHub Pages hosts the site for free.

## What's in this folder

| File | What it holds |
| --- | --- |
| `index.html` | Home: photo, introduction, job market paper, references |
| `research.html` | Research: job market paper, working papers, work in progress |
| `cv.html` | CV: education, teaching, awards, presentations, link to the full PDF |
| `about.html` | About me: a longer introduction and contact details |
| `style.css` | Colors, fonts and layout shared by all four pages |
| `images/photo.jpg` | Placeholder photo |
| `files/cv.pdf`, `files/jmp.pdf`, `files/paper-2.pdf` | Placeholder PDFs |

To preview the site on your computer, double-click `index.html`.

## 1. Put the site online with GitHub Pages

1. Sign in to [github.com](https://github.com), or create a free account. Your username becomes part of the web address.
2. Click **+** in the top-right corner, then **New repository**. Name it exactly `USERNAME.github.io`, using your own username. Set it to **Public** (free accounts can only publish public repositories), then click **Create repository**.
3. On the new repository page, click **uploading an existing file** (or **Add file → Upload files**). Unzip the download, open the folder, select everything inside it and drag it onto the upload area. Check that `index.html` sits at the top level of the repository, not inside another folder. Click **Commit changes**.
4. Open **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, and click **Save**.
5. Visit `https://USERNAME.github.io`. The first publish usually takes a minute or two; GitHub says changes can take up to 10 minutes to appear.

Everything in a public repository can be seen by anyone, so upload only what you want on the site.

## 2. Fill in your details

The easiest way to edit is on GitHub itself: open a file, click the pencil icon, make your changes and click **Commit changes**. The live site updates a minute or two later. You can also edit the files on your computer in any plain-text editor (VS Code, Notepad, or TextEdit in plain-text mode) and upload them again.

Search each file for these placeholders and replace them: `Your Name`, `Your University`, `Professor Name`, `20XX`, `your.email@university.edu`. The comments in the files (lines that start with `<!--`) point to the blocks you can copy.

- **Photo**: upload your photo to the `images` folder with the name `photo.jpg`; it replaces the placeholder. A portrait of at least 800 × 1000 pixels looks best. The page crops it to a 4:5 frame automatically.
- **CV and papers**: upload your PDFs to the `files` folder with the same names (`cv.pdf`, `jmp.pdf`, `paper-2.pdf`). To use other names, change the matching `href="files/..."` links.
- **Job market paper**: its title and abstract appear on both `index.html` and `research.html`, so update both.
- **Add a paper, course or reference**: copy one block (`<article class="paper">…</article>`, `<div class="cv-item">…</div>`, or a reference `<li>…</li>`) and paste it right below the original.
- **Remove a section**: delete its whole `<section>…</section>` block.
- **Profile links**: replace the Google Scholar, GitHub and LinkedIn addresses with links to your own profiles.
- **Last updated**: change the date in the footer of each page whenever you update the site.

## 3. Change the look (optional)

All colors and fonts are set at the top of `style.css`. Change `--accent` to recolor every link and button. The two blocks below it hold the colors used when a visitor's device is in dark mode.
