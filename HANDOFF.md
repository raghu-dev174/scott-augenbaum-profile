# Hand-off notes: Scott Augenbaum landing page

Two equivalent builds of the same page. Pick one.

1. html-site/   Plain HTML, CSS, images. No build. Fastest to deploy (drag and drop on Vercel or Netlify).
2. react-site/  React + Vite. Same page split into one component per section. Run `npm install`, then `npm run build`; deploy `dist/`.

Also included in both: llms.txt, robots.txt (allows AI crawlers) and favicon.png at the site root.
No backend, no forms, no environment variables, no API keys. The only external request is Google Fonts (Carlito).

Contact: all booking buttons open an email to scottaugenbaum@cybersecuremindset.com. Other links go to cybersecuremindset.com (/contact, /speaking, /advisory, /courses), YouTube, Buzzsprout and Cybercrime Magazine.
Video and podcast cards link out; they do not embed.
Search and AI visibility: JSON-LD (Person, Book, FAQPage) sits in the head of index.html. Keep it when editing.
After deploying: add the live domain to the site (optional canonical tag and sitemap.xml), and test the page at 400px width.
Dark mode follows the visitor's system setting automatically.
