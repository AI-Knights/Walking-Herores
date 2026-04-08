# Publishing Your Landing Page on GitHub Pages

This guide outlines how to easily deploy your landing page (`index.html` and `styles.css`) for free using GitHub Pages.

## Prerequisites
1.  A GitHub account (https://github.com/).
2.  Git installed on your machine (if deploying via command line).

## Method 1: Using the GitHub Web Interface (Easiest)

1.  **Create a New Repository:**
    *   Go to GitHub and click **New Repository**.
    *   Name it something like `geography-geyser-app`.
    *   Make the repository **Public**.
    *   Check "Add a README file" (optional but recommended).
    *   Click **Create repository**.

2.  **Upload Files:**
    *   In your new repository, click **Add file** -> **Upload files**.
    *   Drag and drop `index.html` and `styles.css` from your `marketting` folder into the upload area.
    *   Click **Commit changes**.

3.  **Enable GitHub Pages:**
    *   Go to the **Settings** tab of your repository.
    *   In the left sidebar, click on **Pages**.
    *   Under "Build and deployment" Source, select **Deploy from a branch**.
    *   Under "Branch", select your main branch (usually `main` or `master`) and set the folder to `/ (root)`.
    *   Click **Save**.

4.  **View Your Site:**
    *   At the top of the Pages settings, you'll see a message like "Your site is live at `https://[your-username].github.io/geography-geyser-app/`".
    *   It might take a minute or two to build the first time. Refresh the page to see the link.

## Method 2: Custom Domain (Optional)
If you want a custom domain (e.g., `geographygeyser.com`):

1.  Purchase a domain from a registrar (like Namecheap, Google Domains, Route53).
2.  In your GitHub repository **Settings -> Pages**, scroll down to **Custom domain**.
3.  Enter your custom domain and click **Save**.
4.  Configure your DNS records at your registrar:
    *   Add `A` records pointing to GitHub's IPs (e.g., `185.199.108.153`, `185.199.109.153`, etc.).
    *   Add a `CNAME` record for `www` pointing to `[your-username].github.io`.
5.  Check "Enforce HTTPS" in GitHub Pages settings.

## Adding App Images
To make the page look complete, we left an optional section in the HTML for an app preview. 
1. Take a nice screenshot of your app (perhaps framed in an iPhone/Android mockup).
2. Save it as `app-screenshot.png`.
3. Uncomment the `<div class="app-preview">...</div>` block in `index.html`.
4. Upload `app-screenshot.png` directly to your repository via GitHub (or commit it if using CLI).
