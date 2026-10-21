FATI FAST - STATIC WEBSITE (GITHUB PAGES-COMPATIBLE)
===================================================

WHAT CHANGED
- Existing site styling, truck images, and page layout are preserved.
- The Contact form sends JSON from the browser to FormSubmit AJAX.
- The Documents form sends a normal multipart POST to FormSubmit (all four files).
- Both forms target: fatifastbusiness.companyllc@gmail.com
- Changed the combined upload maximum to 10 MB to match FormSubmit's documented limit.
- Added a thank-you page for regular file submissions.
- Removed PHP SMTP server code because GitHub Pages cannot execute PHP.

SETUP ON GITHUB PAGES
1. Create a GitHub repository. Upload index.html, thanks.html, .nojekyll,
   and the images/ directory directly into the repository root.
   (Upload the contents of this ZIP, not the ZIP file itself.)
2. In Settings > Pages, select "Deploy from a branch", choose main and / (root).
3. Visit your https://USERNAME.github.io/REPOSITORY/ URL once it is deployed.
4. SUBMIT A TEST CONTACT MESSAGE on the live site.
5. IMPORTANT: Log into fatifastbusiness.companyllc@gmail.com. Open the activation email
   from FormSubmit and click the activation/confirmation link.
   Check spam/junk/promotions if you do not see it.
6. Send a new contact test and ensure it arrives in the mailbox.
7. Submit four NON-SENSITIVE test files under 10 MB TOTAL and check that
   all four attachments arrive. The document form may show provider CAPTCHA.
8. Keep copies of important received attachments; FormSubmit's archive does
   not retain the file attachments.

IMPORTANT LIMITATIONS
- This does not use Gmail SMTP, a Gmail app password, or PHP.
- This code is wired to FormSubmit but live inbox delivery is NOT verified here.
  The recipient MUST activate delivery before the forms will work end to end.
- Contact messages show an inline acknowledgement only if the service returns
  an explicit success value; document uploads navigate to a thank-you page.
- Do not test from file://; deploy or use a local HTTP server instead.
- FormSubmit processes the uploaded documents. The uploaded documents could
  contain sensitive tax/banking information (W-9, voided check). For a live
  production business, prefer a vetted secure document-upload portal, clear
  privacy disclosures, and appropriate data handling instead of email files.
- GitHub Pages' terms say it is NOT intended or allowed as free hosting for
  an online business or a site primarily facilitating commercial transactions.
  Prefer an appropriate business website host (e.g. Cloudflare Pages/Netlify)
  for the actual public commercial site; these static files can move there.
- IMPORTANT: Keep the original README outside the uploaded root if you want
  only site files exposed on the published GitHub Pages website.

OFFICIAL DOCUMENTATION
https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
https://formsubmit.co/documentation
https://formsubmit.co/ajax-documentation

NO PASSWORDS OR PRIVATE API KEYS SHOULD EVER BE UPLOADED TO GITHUB.
