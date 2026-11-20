# INTERNET PROGRAMMING 1 — CAT 3 FINAL SUBMISSION

## Project title
**CivicFlow — Community Service Navigator**

## Student details
**Name:** Ndei Emmanuel Nzyoki  
**Registration number:** BCS-03-0029/2026  
**Copyright:** © 2026

## 1. Chosen area of interest

The selected area is **Any Other of Your Choice: a community service navigator**.

CivicFlow addresses the practical problem of residents struggling to find reliable local support. Information about healthcare, learning, food assistance, safety, and transport is often spread across offices, posters, social media, and separate websites. CivicFlow provides one clear, searchable starting point where a visitor can discover a service, compare basic details, and submit a support request.

## 2. System objectives

The system is designed to make community-service information easier to find and understand. It demonstrates how HTML provides structure, CSS creates a responsive interface, and JavaScript adds client-side interactivity. It also shows how a static client-side prototype could later connect to an application server, database, and web APIs.

The project is a five-page website. Each page is linked through the shared navigation menu, and each page includes the required student footer: **Ndei Emmanuel Nzyoki · BCS-03-0029/2026 · © 2026**.

## 3. Webpage descriptions

### Home page — `index.html`

The Home page introduces CivicFlow with the message “Find the right help. Without the runaround.” It presents the Discover–Compare–Connect service path, links visitors to the Services and About pages, and uses JavaScript counters to reveal the sample directory summary. The page uses semantic sections, headings, paragraphs, hyperlinks, cards, and a footer.

### About page — `about.html`

The About page explains the problem and assigns a purpose to each webpage. It also explains client/server architecture, shared hosting, application servers, dedicated servers, responsive design, single-page applications, web APIs, and progressive enhancement. Expandable accordion sections and an interactive button demonstrate JavaScript behaviour.

### Services page — `services.html`

The Services page is the main directory. It contains six sample service cards across four categories: Health, Learning, Essentials, and Safety. Users can search by keyword or filter by category. JavaScript updates the displayed cards and shows an empty-state message when no match is found. The page also includes hyperlinks and a structured HTML comparison table.

### Gallery page — `gallery.html`

The Gallery page demonstrates multimedia HTML. It uses CSS-generated visual panels, an HTML5 audio element, and an HTML5 video element with a poster image and native controls. The page explains how media can provide context and make a service system more human and accessible.

### Contact page — `contact.html`

The Contact page contains a support-request form with labels, text inputs, an email field, a category select menu, a message textarea, and a submit button. JavaScript validates required fields and checks the email pattern. The page displays field-level error messages and a success message after valid submission.

## 4. HTML implementation review

The source uses HTML5 document structure with `<!doctype html>`, language declarations, character encoding, responsive viewport metadata, page titles, semantic `header`, `nav`, `main`, `section`, `article`, `aside`, `form`, `table`, `audio`, `video`, and `footer` elements.

The five pages share a consistent navigation structure and relative hyperlinks, making them interconnected. The Services page demonstrates table markup and data attributes. The Contact page demonstrates form controls and accessible labels. All pages load the shared `styles.css` and `script.js` files.

## 5. JavaScript implementation review

The shared `script.js` file waits for `DOMContentLoaded` before attaching behaviour. It includes the following functionality:

1. **Mobile navigation:** toggles the navigation menu and updates the `aria-expanded` attribute.
2. **Animated counters:** reads `data-counter` values, increments them with `requestAnimationFrame`, and updates the displayed numbers.
3. **Service filtering:** reads the search box and category select menu, loops through service cards, checks matching text and category values, and hides or shows cards with the `hidden` class.
4. **Empty-state handling:** displays a message when the search produces no matching services.
5. **Accordion controls:** opens and closes About-page information panels and updates `aria-expanded`.
6. **Form validation:** checks required fields, validates the email pattern, writes error messages, and displays a success response for valid data.
7. **Flash messages:** provides temporary dynamic status messages for interactive buttons.

The implementation demonstrates variables, functions, arrays, loops, conditionals, DOM selection, DOM updates, event listeners, regular expressions, and browser methods.

## 6. Client/server architecture

In the current prototype, the browser is the client. It downloads the HTML, CSS, and JavaScript files, renders the interface, and performs the interactive work locally.

In a production deployment, an application server could receive contact requests, authenticate service providers, store service records in a database, and return JSON responses through web APIs. The browser could then request live service availability, opening hours, map locations, and emergency updates without requiring all information to be hard-coded into the HTML.

## 7. Hosting options

**Shared hosting:** suitable for the current static prototype because HTML, CSS, and JavaScript files can be served at low cost. Multiple websites share server resources.

**Application server:** suitable for a production CivicFlow system that needs accounts, server-side form processing, a database, provider management, authentication, and web APIs.

**Dedicated server:** suitable for a large or high-traffic deployment that requires predictable performance, stronger infrastructure control, or specialized security configuration. It is more expensive and requires more administration.

## 8. Emerging trends demonstrated

CivicFlow demonstrates responsive design through flexible grids, mobile breakpoints, touch-friendly controls, and a collapsible mobile navigation menu. It follows progressive enhancement by keeping the core information in semantic HTML while using CSS and JavaScript to improve the experience.

The system could evolve into a single-page application where directory results update without full-page reloads. Web APIs could connect the site to maps, live opening hours, provider databases, emergency alerts, and notification services.

## 9. Testing and review summary

The five HTML pages were served successfully through the development server. The route manifest lists all five pages. Desktop and mobile layouts were visually checked. The required footer was verified on every page. The JavaScript source was reviewed for navigation, counters, filtering, accordions, flash messages, and form validation.

The Gallery page uses externally hosted sample media URLs, so audio, video, and the poster image require an internet connection when viewed. In a final production system, these assets should be stored locally or in reliable project storage.

## 10. Conclusion

CivicFlow meets the CAT 3 requirement for a creative multi-page Internet Programming project. It addresses a real-world need, demonstrates HTML, CSS, JavaScript, forms, tables, hyperlinks, lists, graphics, audio, video, client/server concepts, hosting options, responsive design, and emerging web trends. The system is structured so that the current prototype can grow into a database-backed community service platform.
