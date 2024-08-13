## Introduction to Next.js

### Why Next.js Over React.js?

- **SSR is enabled along with CSR**  
  SSR (Server-Side Rendering) is available in Next.js, in addition to CSR (Client-Side Rendering).
  
- **CSR requires useState, button, input page (or when an error occurs)**  
  CSR relies on hooks like `useState`, and components like buttons and input fields. 
  
- **"use client" for CSR; otherwise, default is SSR**  
  Use `"use client"` for Client-Side Rendering. By default, Next.js uses Server-Side Rendering.

- **CDN is not possible in Next.js but is in React**  
  Content Delivery Networks (CDNs) can be used with React but are not directly supported in Next.js.

- **SEO Optimized product in Next.js: Solves the waterfall problem and enables fast rendering through SSR**  
  Next.js addresses the waterfall problem by serving direct HTML, CSS, and JS to the end-user, which helps SEO bots understand the page content.

- **Waterfall problem is solved**  
  In traditional approaches, the browser requests and receives JavaScript files before rendering the content. This can hinder SEO. Next.js provides direct HTML, CSS, and JS to the end-user, improving SEO.

- **Routing is enabled by Next.js**  
  Next.js includes built-in routing. While React Router is available and provides similar functionality, Next.js routing and SEO optimization are more integrated and efficient.

### Installation Steps and Understanding

- **src directory**  
  There's no installation requirement for the `src` directory. In Next.js, the `src/app` folder is used. If `src/app` does not exist, only one folder difference is noted. App Router was introduced in Next.js 13, where you create folders inside `page.tsx` and `layout.jsx`. The wonders of file-based routing are handled via the App Router.

- **@ as import alias**  
  The `@` symbol represents the root of the project for locating the app folder, e.g., `@/app`. 

- **Folder structure and routing**  
  Every folder created with a name corresponds to a route. Inside each folder, `layout.tsx` or `page.tsx` is required. `page.tsx` contains the React code that renders the route page.

- **global.css and tailwind.css**  
  `global.css` applies to the entire project, while `tailwind.css` should be tuned as per the project requirements.

- **@/app/page.tsx**  
  This file contains the render code for the root route.

- **layout.tsx**  
  Use `layout.tsx` when you need a repeated layout for all routes, such as a banner for routes like `https://domain/auth/signin` or `https://domain/auth/login`. Place the banner code in `layout.tsx` and pass props accordingly.

- **Hidden routes**  
  When you want a layout but do not want to tweak the route, make the auth folder hidden in the route by naming it with a schema like `(auth) (_folder_name_)` as part of merging routes.

- **next.config.mjs**  
  This file is the configuration file for Next.js projects and is required for deployment tweaks.

- **.next folder**  
  This folder is similar to the `.dist` folder in React projects and is where the development build is created.

- **Tailwind config file**  
  Tweak the Tailwind config file if your folder structure includes Tailwind classes. By default, root pages, app, and components folders are included.
