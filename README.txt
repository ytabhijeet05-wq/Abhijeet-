HEARTLET DECOR WEBSITE
======================

Files:
- index.html
- style.css
- script.js
- favicon.svg
- assets/hero-anime.jpg (your uploaded anime collage, if included)

HOW TO PREVIEW
1. Extract the ZIP.
2. Open index.html in a browser. For best results use a local static server or publish to a host such as Netlify/GitHub Pages.
3. The site works without an email service for browsing, filtering, wishlist, order list and enquiry form validation.

HOW TO ADD POSTERS
1. Put poster files in assets/, e.g. assets/poster-01.jpg.
2. Open script.js and find the PRODUCTS array.
3. For each product, edit name, imageUrl, price, category and description.
4. Use imageUrl: "assets/poster-01.jpg" for local files, or a publicly accessible direct image URL.
5. Add productUrl only if you have a real product page.
6. Set featured: true or bestSeller: true only for your chosen products.
7. Set available: false to hide a product from the shop.
The 50 sample prices are ₹199 and are clearly editable placeholders, not live product offers.

EMAIL ORDER SETUP
1. Create a Formspree account and a form.
2. Set the form's receiving/verified email to ytabhijeet05@gmail.com.
3. Copy the endpoint, normally https://formspree.io/f/FORM_ID.
4. Paste it into CONFIG.formspreeEndpoint in script.js.
5. Publish and test a real test enquiry. Verify it arrives in your inbox.
Until configured, the site clearly refuses to claim that an enquiry was sent.
Note: Formspree's own dashboard and spam protection settings may require extra setup. Do not add secret keys to frontend code.

WHATSAPP
Configured WhatsApp number: 918840731216 (India country code 91 + the number you supplied). The floating WhatsApp button will open a chat with a prefilled message. If you change your number, edit CONFIG.whatsappNumber in script.js using digits only.

HERO BACKGROUND
The uploaded image is stored at assets/hero-anime.jpg and configured in CONFIG.heroImage. The page adds a subtle scroll parallax and desktop pointer movement. Keep the image file in the same assets folder when hosting.

TESTING
- Search a name, then try a nonsense search to test the empty state.
- Change category and sort settings.
- Test Load More and wishlist.
- Temporarily rename a poster image file to check its fallback.
- Set a product price to -1 to confirm it is excluded from the catalogue.
- Submit the order form before configuring Formspree: it should show a clear not-configured message.
- After configuring Formspree, test success and failure cases. Disconnecting internet can test a network failure.
- Test phone and desktop widths, keyboard focus, and reduced-motion setting.

PUBLISH
Recommended simple route: Netlify Drop or GitHub Pages.
- Netlify: create an account, upload/extract the whole website folder (keep assets folder and files together), then open the generated URL.
- GitHub Pages: create a repository, upload all files and assets, enable Pages in repository settings.
- Use a custom domain only if you own it.
Before launch, replace placeholder products and review the privacy policy, terms, delivery, cancellation and refund policies.
