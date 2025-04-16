# Seth Rose | AI Solutions Consultant - Portfolio

This is the source code for [sethrose.dev](https://sethrose.dev), a personal portfolio and contact site for Seth Rose, AI Solutions Consultant.

## Features
- Modern, responsive, single-page design
- Social links and project/resume buttons
- Newsletter signup (Sender.net integration)
- SEO-friendly meta tags and Open Graph/Twitter Card support
- Custom favicon and profile image

## Deployment: GitHub Pages

### 1. Push to GitHub
- Push all files to your GitHub repository (e.g., `TheSethRose/github.io`).

### 2. Enable GitHub Pages
- Go to your repository on GitHub.
- Click **Settings** > **Pages**.
- Under **Source**, select the `main` branch and `/ (root)` folder.
- Click **Save**. Your site will be live at `https://<your-username>.github.io/`.

### 3. Set a Custom Domain (sethrose.dev)
- In the **Pages** settings, enter `sethrose.dev` as your custom domain and save.
- GitHub will create a `CNAME` file automatically.

#### DNS Configuration
- Go to your domain registrar (where you bought `sethrose.dev`).
- Set the following DNS records:
  - **A** records (for apex domain):
    - `185.199.108.153`
    - `185.199.109.153`
    - `185.199.110.153`
    - `185.199.111.153`
  - **CNAME** record (for www):
    - Name: `www`
    - Value: `<your-username>.github.io.`
- Remove any old A/AAAA/CNAME records for the root or www.

- Wait for DNS to propagate (can take up to 24 hours).
- GitHub Pages will automatically issue an SSL certificate for HTTPS.

## Customizing
- **Profile image:** Replace `assets/images/profile.png` with your own.
- **Resume:** Replace `resume.pdf` with your own file.
- **Social links:** Edit `index.html` to update your links.
- **Newsletter:** Configure Sender.net as described in the code comments.

## Local Development
Just open `index.html` in your browser. No build step is required.

---

For more, see the [GitHub Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages) and [custom domain setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages).
