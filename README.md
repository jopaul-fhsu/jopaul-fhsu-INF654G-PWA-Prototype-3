# INF654G-PWA-Prototype-3

## Overview of the Service Worker and Manifest File

### Service Worker

- **Purpose**: Manages caching of assets for offline use.
- **Cache Name**: contact-list-cache-v1.
- **Assets to Cache**:

- The root (/), index.html, styles.css, and app.js from assets.
- **External files:** Materialize CSS and JavaScript from a CDN and Google Material Icons.
- **Installation Event:** Opens the cache with the specified name and adds all listed URLs.
- **Fetch Event:** Intercepts fetch requests, serving cached content if available. Otherwise, it fetches from the network.

### Manifest

#### App Metadata:

- **name**: "Contact List App"
- **short_name**: "Contacts"
- **description**: "A simple contact list application."
- **Icons**: Defines two icon sizes (192x192 and 512x512) for the app.

#### Appearance and Initialization:

- **start_url**: Launches at index.html.
- **display**: standalone, for standalone app behavior.
- **background_color**: White background color (#ffffff)
- **theme_color**: Light Blue UI theme color(#64b5f6)
