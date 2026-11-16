# Collin Chiong — Personal Portfolio
## INFR3120 Assignment 2 (Express & EJS)

A four-page responsive portfolio website refactored from static HTML/CSS into a dynamic Node.js / Express.js application using the EJS templating engine. The site is hosted live on Render.

## Live Site
https://my-portfolio-ejs-edition.onrender.com/

## GitHub Repository
https://github.com/Collinagun/my-portfolio-ejs-edition

## Pages
/ (index.ejs) - Home page with Hero Banner and Project Grid
/about (about.ejs) - About Me, Profile Photo, and Intro Video
/projects (projects.ejs) - Grid of past projects and assignments
/contact (contact.ejs) - Styled contact form



## Site Structure & Technology
This project was generated using the Express Generator with the --view=ejs flag, following the standard MVC structure:

routes/index.js: Acts as the Controller. Defines the router.get paths for all four pages and renders the corresponding EJS views.
views/: Contains the EJS page templates (index.ejs, about.ejs, projects.ejs, contact.ejs).
views/partials/: Contains the shared header.ejs and footer.ejs to avoid repeating code across pages.
public/: Contains all static assets, separated into /images, /javascripts, and /stylesheets.
Responsive Design & Bootstrap
Unlike Assignment 1 (which used three separate custom CSS files and media queries), this site uses the Bootstrap 5 framework for responsive layout and grid management.



## Viewport Behavior (via Bootstrap)
Class	Behavior
container	Centers content and provides responsive max-widths.
row / col-md-4	Creates a responsive grid. Cards sit side-by-side on desktop (3 columns) and stack vertically on mobile.
navbar-expand-lg	Collapses the navigation menu into a hamburger toggle on smaller screens.
Every page includes the viewport meta tag:

<meta name="viewport" content="width=device-width, initial-scale=1.0">



## Colour Scheme
The custom Adobe Colour scheme from Assignment 1 was retained, implemented using CSS variables within partials/header.ejs.

#D99437 Warm orange (Accents)

#23B7D9 Teal (Headings, form borders)

#1FA65A Green (Hover states)

#F2E2CE Cream (Page background)

#8176D7 Purple (Navbar/Footer backgrounds)



## Testing (Simple)
Node/Express: Tested locally on localhost:3000 (All routes return 200 OK).

Responsive testing: Tested using Chrome DevTools (Mobile, Tablet, Desktop viewports).

Form testing: mailto: action successfully opens the default email client.



## EJS Features
EJS Partials: <%- include('partials/header') %> and <%- include('partials/footer') %> are used to inject shared layout elements.

EJS Conditional Logic: Used for the navigation bar to apply the active class dynamically based on the page title variable passed from routes/index.js.

<video>: Embedded intro video with controls and poster attributes.



## Visual Layout Inspiration
The hero banner, grid layout, and footer structure were inspired by the Sample Student Portfolio provided in the INFR3120 Assignment 2 PDF (Nvi Mai's portfolio: https://nvimai.com/).



## Citations
Bootstrap 5 (CSS/JS): Bootstrap. “Bootstrap.” Getbootstrap.Com, 2025, https://getbootstrap.com/. Accessed 15 Nov. 2026.

Font Awesome (Icons): Font Awesome 5. “Font Awesome 5.” Fontawesome.Com, Font Awesome 5, 2024, https://fontawesome.com/. Accessed 15 Nov. 2026.

Google Fonts (JetBrains Mono): “JetBrains Mono - Google Fonts.” Google Fonts, 2025, https://fonts.google.com/specimen/JetBrains+Mono. Accessed 15 Nov. 2026.

“HTML Input Type=’Tel.’” Www.W3schools.Com, https://www.w3schools.com/tags/att_input_type_tel.asp. Accessed 15 Nov. 2026.

W3Schools. “HTML Input Type=’Email.’” Www.W3schools.Com, https://www.w3schools.com/tags/att_input_type_email.asp. Accessed 15 Nov. 2026.



Frameworks & Libraries were loaded via CDN.

The base project structure and boilerplate server code were generated using the official express-generator. All routes, EJS views, custom styling, and content are my own work. Code from the course lectures was used to understand Express routing and EJS includes.

Deepseek was used to help remedy errors and ensure I was on the right track.

Collin Chiong
Student of FBIT Faculty — Ontario Tech University
collin.chiong@ontariotechu.net

© 2026 by Collin Chiong. All rights reserved.
