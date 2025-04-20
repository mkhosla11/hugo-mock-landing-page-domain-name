# 🧘‍♀️ MindTap Meditations (a Hugo mock landing page)

**MindTap Meditations** is a mindfulness landing page built using the [Hugo static site generator](https://gohugo.io/) and the [Hugo Bootstrap Theme](https://github.com/filipecarneiro/hugo-bootstrap-theme). It is designed to introduce and promote a wellness product tailored for busy professionals looking to integrate mindful habits into their daily routines.

## 🌟 Purpose

The MindTap landing page serves as the central marketing site for a meditation platform focused on:

- **Personalized meditation goals** (focus, stress relief, better sleep)
- **Quick sessions** (2, 5, or 10 minutes)
- **Motivating streaks and stats tracking**
- And more...

This site is a live demonstration of brand storytelling, user feature illustrations, and lightweight modern design.

## 🚀 Live Preview

🌐 [Visit the Live Site](https://mkhosla11.github.io/hugo-mock-landing-page-autodeployed/)  
(Hosted via GitHub Pages on the `gh-pages` branch)

## 🔄 GitHub Actions: Build & Deploy Automation

This project uses a **GitHub Actions workflow** to automatically build and deploy the MindTap Meditation landing page to **GitHub Pages**. Every time changes are pushed to the `main` branch, the workflow performs the following:

1. **Checks out the repository**  
   Including any Hugo themes added as submodules, with full Git history to support `.GitInfo` and `.Lastmod`.

2. **Initializes the Hugo environment**  
   Installs Hugo Extended v0.144.1 using the `peaceiris/actions-hugo` GitHub Action.

3. **Compiles the static site**  
   Runs the command `hugo -D --gc --minify` to:
   - Include drafts
   - Run garbage collection
   - Minify the output for faster loading

4. **Deploys to GitHub Pages**  
   Uses `peaceiris/actions-gh-pages` to publish the generated content to the `gh-pages` branch.

The entire process is automated and ensures your Hugo site is always up-to-date and deployed live with minimal manual work.
