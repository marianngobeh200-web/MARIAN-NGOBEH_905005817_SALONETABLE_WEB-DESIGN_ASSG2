# Salone Table

Salone Table is a responsive, multi-page restaurant website for a Sierra Leonean restaurant in Freetown. It introduces the restaurant, showcases example dishes and services, and gives visitors direct ways to ask questions, request a table, or start a pickup-order conversation on WhatsApp.

## Contents

- [Pages](#pages)
- [Features and behavior](#features-and-behavior)
- [Technology](#technology)
- [Run the site locally](#run-the-site-locally)
- [Publish with GitHub Pages](#publish-with-github-pages)
- [Project structure](#project-structure)
- [Content to verify before launch](#content-to-verify-before-launch)

## Pages

| File | Description |
| --- | --- |
| `index.html` | Home page with a restaurant introduction, featured dishes, service highlights, and links to the menu, WhatsApp ordering, and table requests. |
| `menu.html` | Searchable, category-filtered example dishes with photographs and sample prices, an interactive pickup-order summary, and WhatsApp order submission. |
| `about.html` | Restaurant story, local flavours, and information about the restaurant's approach to hospitality and shared meals. |
| `services.html` | Dine-in, pickup, and catering information, including links for table requests and pickup orders. |
| `contact.html` | Restaurant contact details, a Freetown map, and a question form that prepares an enquiry in WhatsApp. |

Every page includes its own navigation and footer markup. When adding or renaming a page, update the navigation and footer links on all pages.

## Features and behavior

- Responsive layouts for desktop and mobile screen sizes.
- Direct page navigation using standard HTML links.
- Menu search and category filters let visitors find dishes by name, description, and category.
- WhatsApp links open a conversation with the restaurant number configured in the page URLs. The Menu page lets visitors add dishes to a pickup order and sends the order details to WhatsApp; the Contact page question form prepares an enquiry message.
- The menu pickup cart updates quantities and an estimated subtotal in the browser. The cart is not saved and does not process payment; the restaurant must confirm menu availability and final prices in WhatsApp.
- The phone number on the contact page is a `tel:` link for devices that support calling.
- The contact page embeds an OpenStreetMap view centered on Freetown.
- Images include alternative text; non-hero images are lazy-loaded.
- No online checkout, payment processing, reservation system, or message-submission backend is included. Visitors contact the restaurant directly to confirm availability and arrangements.

## Technology

This is a static website built with:

- HTML for page content and navigation
- CSS in `style.css` for styling, layouts, and responsive behavior
- Local image files in `images/`

There is no build step, package manager, or backend required. Inline JavaScript powers the Menu page pickup cart and prepares WhatsApp messages from the Menu and Contact pages. The remaining page behavior is static HTML and CSS. Google Fonts and the embedded OpenStreetMap depend on an internet connection; the local HTML, CSS, and images can otherwise be served as static files.

## Run the site locally

### Visual Studio Code Live Server

1. Open the project folder in Visual Studio Code.
2. Install the **Live Server** extension if needed.
3. Open `index.html`, then select **Go Live** or **Open with Live Server**.


## Publish with GitHub Pages

1. Push the project files to a GitHub repository.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the branch containing the site (often `main`) and the `/ (root)` folder, then save.
5. Wait for the Pages deployment to complete. GitHub will show the published URL in the Pages settings.

The HTML files are at the project root, so no build output folder is needed.

## Project structure

```text
.
├── index.html
├── menu.html
├── about.html
├── services.html
├── contact.html
├── style.css
├── images/
│   ├── restaurant and service photos
│   └── dish and drink photos
└── .vscode/
    └── settings.json
```


                                                                              CREATED BY: MARIAN NGOBEH