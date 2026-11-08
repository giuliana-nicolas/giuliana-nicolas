# Wedding website

A small static site designed for GitHub Pages. It uses plain HTML, CSS, and JavaScript, so there is no build step and the layout is easy to replace later.

## Content

The invitation is set up for Giuliana and Nicolás, with the ceremony details,
Google Maps directions, and the embedded RSVP form in `index.html`. The names,
date, venue, and floral artwork are loaded from the extracted images in
`assets/`.

## Languages and gifts

Spanish is the default page (`index.html`); the English version is `en.html`.
The ES / EN links at the top right switch between them. Keep both pages in sync
when updating event details. Both versions include the Banco Itaú gift account.
The embedded Google Form is shared and its questions remain in Spanish.

## RSVP submissions

The RSVP section embeds a published Google Form. Responses are handled by Google and can be connected to a Google Sheet; no guest data is stored in GitHub.

After deployment, submit one test response from the embedded form and confirm that it appears in the form's **Responses** tab.

## Preview locally

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## Deploy with GitHub Pages

Push these files to a GitHub repository, then open **Settings → Pages**, choose **Deploy from a branch**, and select the branch and `/ (root)` folder.
