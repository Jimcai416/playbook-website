# Playbook Interactive — Website

Marketing site for Playbook Interactive, a people-first HR consultancy.

A single self-contained `index.html` (HTML, CSS, and JS inlined) with five anchored sections: Home, For Businesses, For Individuals, About, Contact.

## Local preview

Just open `index.html` in a browser. No build step.

## Deploy

The site is deployed via **GitHub Pages** from the `main` branch root.

To switch to Cloudflare Pages later:
1. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git
2. Pick this repo, leave build settings empty (it's static), publish directory `/`
3. Done.

## Editing

Open `index.html`. Content lives in `<section>` blocks; styles live in the `<style>` block at the top; behaviour in the `<script>` block at the bottom.

## Contact form

Currently UX-only (shows a success message but doesn't send). To wire it up, point the form at:
- [Formspree](https://formspree.io/) — drop-in `action="..."` URL
- [Netlify Forms](https://docs.netlify.com/forms/setup/) — add `data-netlify="true"`
- Your own email/API endpoint
