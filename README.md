# Bus-Website

A marketing website for a fictional or small-business bus charter company, "NJ Bus Service", serving the New York City area. It is a static front-end site with a home page and a blog post page.

Copyright of NJ Bus Company 2018. Made and designed by Max Awad.

## What it does

- Home page with a hero slider, about section, services, fleet, testimonials, counters, team and contact sections.
- A single blog post page (`blog_single.html`).
- Responsive layout built on a Bootstrap template, with sliders, a sticky menu and a video popup.
- The contact and search forms are visual only. They are not connected to any server.

## Tech stack

- HTML, CSS and JavaScript (no build step, no server code)
- Bootstrap 3, jQuery, Owl Carousel, Magnific Popup, Font Awesome, Animate.css, Hover.css, Bootsnav
- Google Fonts and the Linearicons CDN are loaded from the internet, so fonts and some icons need a network connection.

## Run it

No installation is needed. Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Live demo

The site is plain static files with no secrets, so it can be hosted as is on GitHub Pages, Netlify or any static host. The publish directory is the repository root and there is no build command.

## Docker

The `Dockerfile` serves files with Apache httpd. It currently copies from a `public-html/` folder that does not exist in this repository. To use it, either copy the site files into a `public-html/` folder first or change the `COPY` line to `COPY . /usr/local/apache2/htdocs/`.

## Status

Working as a static demo. It is a finished design, but the content is placeholder or sample text from 2018, and the forms do nothing.

## Credits

Built on a third-party Bootstrap business template (Zombiz). Images, fonts and libraries belong to their respective owners. The project has no license file, so all rights are reserved by default.
