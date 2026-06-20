Project overview
A small multi-page website built with HTML, CSS and JavaScript. Pages are plain HTML templates with a shared header, navigation, content sections, and a shared footer. Static assets (CSS, images, JS) are stored in an assets directory. The site is designed for simple content display, basic forms, and client-side interactivity.

Features

Global header and navigation: consistent site title, logo placeholder, and link menu on every page.
Page content sections: each HTML file contains a content area for page-specific text, images, and components.
Responsive layout: CSS rules provide basic responsive behavior for common viewport sizes.
Forms: standard HTML forms for contact or feedback placed on one or more pages. Inputs include text, email, textarea, and submit controls.
Submit confirmation: when any submit button is clicked, a client-side popup alerts "Message submitted successfully" to confirm action. The alert is triggered on submit button click and does not block normal form submission behavior.
Dynamic footer datetime: a shared footer displays the current date and time and updates automatically (once per second) via a small JavaScript file.
Partial footer include: footer markup is stored in a partial include file and referenced from pages so the footer is consistent across the site.
Static asset organization: CSS, JavaScript, and images are grouped under assets for easy maintenance.
File structure (typical)

root HTML files for pages.
partials/footer.html for the shared footer.
assets/css for stylesheets.
assets/js/footer.js for footer datetime and submit confirmation.
assets/images for media.
How to use / run
Open any HTML file in a browser or serve the project folder with a static file server. No build step is required. Ensure assets are accessible relative to each page.

Behavior notes and maintenance

To edit the footer text or format, modify partials/footer.html.
To change confirmation wording or timing, edit assets/js/footer.js.
Ensure each page includes the footer partial or the footer HTML just before the closing body tag to keep functionality consistent.
Tested in modern browsers; graceful degradation applies for older JS-disabled environments.
