# AbstractDash Documentation

This documentation highlights the key features and technologies used throughout the project. It provides a complete guide to running the project, configuring environment variables, exploring available server APIs, and reviewing developer notes.

## Source Code

This is a **premium project** and the source code is **private** and not publicly available.

## Overview

This project provides a fully generic and modern dashboard built with **Nuxt 3 (Vue 3 + SSR)**, designed to be highly adaptable and customizable for any type of business. It serves as a flexible template that can be adapted to different domains without being tied to specific business logic.

## Demo & Showcase

- **Live Demo**: [abstract-dash.vercel.app](https://abstract-dash.vercel.app/)
- **Video Showcase**: [youtu.be/tVZOahAj5vc](https://youtu.be/tVZOahAj5vc)

## Quick Start

Get the project up and running in just a few steps:

**Note:** Make sure you have [Node.js](https://nodejs.org/) installed.

1. **Create Environment File**  
   Rename the `.env.example` file to `.env` and update the values according to your setup.

2. **Install Dependencies**  
   Open your terminal inside the project folder and run: `npm install`

3. **Run Development Server**  
   Start the development server with: `npm run dev`

4. **Build for Production (optional)**  
   To create a production build, run: `npm run build` then `npm run preview`

The project should now be up and running.  
The local server runs at [http://localhost:3000](http://localhost:3000)

## Features

- **Abstract Dashboard**  
  A generic dashboard that serves as a starting point for any business type,without being tied to a specific industry.

- **Multilingual Support**  
  Full i18n integration with **English** and **Arabic** available out of the box. Users can seamlessly switch languages within the application.

- **CRUD Operations**  
  Complete **Create, Read, Update, Delete** functionality for managing items with ease.

- **Validation**  
  Built-in client-side validation ensures required fields are filled and follow proper formatting during **Add** and **Update** operations. This prevents invalid submissions and improves overall data quality before sending to the server.

- **File & Image Upload**  
  Uploading images and files using dialog upload or drag-and-drop area.

- **Rich Data Types**  
  Support for various inputs and display types:  
  `text`, `number`, `date`, `status`, `favorite`, `price`, `rating`, `progress`, `color`, `email`, `phone`, `range`, `map`, `image`, and `file`.

- **Advanced Data Table**  
  Interactive table with: **Pagination, Sorting, Quick Search, Advanced Filtering**, Column Visibility Toggle, Items per Page Control

- **Single & Bulk Deletion**  
  Delete individual items or perform bulk deletions using checkbox row selections.

- **Modern UI/UX**  
  Beautiful, responsive design with vibrant colors and smooth animations.

- **Dark / Light Mode**  
  Built-in support for theme switching with smooth transitions. Users can seamlessly switch between **Light** and **Dark** themes for a personalized experience.

- **Responsive Layout**  
  Fully optimized for all screen sizes: mobile, tablet, and desktop following a mobile-first approach.

- **Cross-Browser Support**  
  Tested and optimized to work seamlessly across all major browsers, including **Chrome, Firefox, Safari, Edge, and Opera**.

- **Dashboard Overview Page**  
  Abstract dashboard page featuring KPIs, charts, summaries, and map for quick insights.

- **Internal Documentation Page**  
  A built-in **Docs page** powered by **Markdown** using `@nuxt/content`. The content is written in a single `.md` file and automatically transformed into a fully styled **HTML page** inside the app, ensuring consistent design and easy maintenance.

- **Settings Page**  
  A dedicated internal page that provides a centralized place for user preferences:  
  **- Switch Theme Mode**: Choose between Light and Dark.  
  **- Change Language**: Switch instantly between English and Arabic.  
  **- Pick Primary Color**: Pick a custom identity color to be applied across the app.  
  **- Live Preview Section**: A real-time preview panel that reflects all local changes to **color, theme, and language** instantly — without refreshing the page. It also shows the global static colors for consistency while testing custom options.  
  **- Configure File Upload Storage**: Select the preferred storage strategy — **Vercel Blob** (recommended) or **Binary Fallback** (store in MongoDB).

- **Persistent Preferences with Cookies**  
  User settings such as **theme mode, language, and primary color** are stored in cookies to ensure a seamless experience. Preferences are remembered across sessions without requiring reconfiguration each time.

- **Demo Mode Toggle**  
  A switch to enable **read-only mode**, preventing data modifications during demos.

- **Backend & Database Support**  
  Connected to **MongoDB** with backend logic powered by **Nuxt Nitro** (built in Nuxt framework).

- **Server API Routes**  
  Server API endpoints under `/server/api/*`

- **Clean Code & Well-Structured Project**  
  Follows clean architecture principles and a consistent code style, ensuring high readability, scalability, and maintainability.  
  Folder structure is carefully organized to separate concerns and keep the codebase intuitive for developers.

## Stack

_Core Frameworks_

- **Nuxt 3** – A framework built on top of Vue 3 and modern JavaScript/TypeScript. It extends Vue’s ecosystem with server-side rendering (SSR), file-based routing, and seamless integration of frontend + backend in a single project.
- **Vue 3** – The core JavaScript framework for building reactive, component-based UIs. It provides the foundation on which Nuxt adds advanced tooling and backend capabilities.
- **Vue Router 4** – Client-side routing integrated with Nuxt.

_Language & Tooling_

- **TypeScript** – A typed superset of JavaScript that adds static typing and better tooling, while compiling to plain JavaScript.

- **ESLint** – Linting and code quality checks.

_State Management_

- **Pinia** – Official Vue store library, integrated with Nuxt for global state management.

_Localization_

- **Vue i18n** – Provides full multilingual support (English/Arabic).

_Styling & UX_

- **Sass (Scss)** – CSS preprocessor for scalable and maintainable styles.
- **normalize.css** – Ensures consistent styling across browsers.
- **@nuxt/icon** – Icon system with support for multiple icon sets.
- **@nuxt/fonts** – Easy integration of web fonts.

_UI & Visualization_

- **Leaflet** – Interactive maps.
- **ECharts** – Powerful charting library for data visualization.

_Backend Engine_

- **Nitro** – The built-in lightweight server engine in Nuxt 3. It powers the backend with API routes, server-side logic, and supports multiple deployment targets (Node.js, Serverless, Edge).

_Database & Storage_

- **MongoDB** – Main database (using the native `mongodb` driver).
- **Vercel Blob** – Optional proxy for handling file uploads.

_Others_

- **@nuxt/content** – Manage content with Markdown, YAML, CSV, or JSON files, which are automatically converted into fully HTML pages.
- **Formidable** – Handling file uploads on the server.
- **lodash.debounce** – Utility for performance optimization (debounce).
- **Mobile-First Design** – All UI/UX decisions follow a mobile-first approach to ensure responsiveness across devices.

## Frontend Flexibility

The frontend is designed with **maximum adaptability** in mind.  
It makes use of generic and versatile field names (e.g., `smallText`, `largeText`, `number`, `status`, `date`),  
which are not tied to a specific business logic.

By keeping the schema flexible and avoiding business-specific coupling, the project ensures **easy customization** and **broad reusability**.

## Backend Flexibility

Although this project ships with a ready-made backend (using Nuxt Server Routes, MongoDB, and optional Vercel Blob storage),  
it is **not strictly coupled** to it.

The entire **frontend layer** is functional and can be integrated with any backend of choice.  
Only some adjustments to the API endpoints are required to connect to a different backend.

This makes the project flexible and reusable across multiple environments and technology stacks.

## Project Structure

The project is organized in a clean and modular way, following Nuxt 3 conventions with additional structure for backend, i18n, and content.

_Main Files_

- **.env** – Environment variables (not committed, see `.env.example`).
- **README.md** – Quick introduction and setup guide for getting started with the project.
- **package.json** – Dependencies, scripts, and metadata.
- **nuxt.config.ts** – Main Nuxt configuration.
- **tsconfig.json** – TypeScript configuration.
- **eslint.config.mjs** – ESLint configuration.
- **content.config.ts** – Nuxt Content configuration.
- **app.vue** – Root application entry.
- **CHANGELOG.md** – Tracks all notable changes, features, and fixes over project versions.
- **.editorconfig** – Ensures consistent coding styles across different editors.
- **.gitignore** – Git ignore rules.

_Core Directories_

- **/assets/scss** – Global SCSS partials (styles, variables, mixins, placeholders, etc.).
- **/public** – Static files served at the root (e.g., `favicon.ico`).
- **/components** – Vue components used across the application.
- **/layouts** – Application layouts (default, empty).
- **/pages** – Application pages, auto-mapped to routes.
- **/composables** – Reusable Vue composables (hooks).

_Content & Localization_

- **/content**
  - `documentation.md` – Main docs file powering the internal Documentation page.
- **/i18n**
  - `/locales/ar.json` – Arabic translations.
  - `/locales/en.json` – English translations.

_State & Utilities_

- **/stores** – Pinia stores for state management.
- **/types** – TypeScript type definitions.
- **/utils** – Utility constants and functions.

_Backend (Nitro)_

- **/server**
  - `/api` – API endpoints.
  - `/db` – Database connections (MongoDB).

## Single File Components (SFCs)

All Vue components in the project follow a consistent structure, clean code and coding standards to ensure readability, scalability, and maintainability.

- **Code Length** – Each component is limited to a maximum of **200 lines** (enforced by ESLint).
- **Template** – Written in **HTML** with semantic and accessible markup.
- **Script** – Uses the **`<script setup>` Composition API** with **TypeScript** for strong typing and cleaner logic.
- **Style** – Written in **SCSS** (not scoped), leveraging global SCSS **helpers, variables, mixins, and placeholders** to maintain design consistency.

> **Consistency Rule:** This structure is applied uniformly across the entire project for every component.

## Prerequisites

Before setting up the project, make sure you have the following installed and ready:

- **Node.js** – Version **18 or higher** (recommended **v22.14.0**).
- **Package Manager** – One of **npm**, **pnpm**, **yarn** or **bun** installed globally.
- **MongoDB Authentication** – A running MongoDB instance with a valid **connection URI**.  
  (If authentication is enabled, include the **username/password** in the URI).
- **Vercel Blob Authentication (Optional)** – Requires a valid **`BLOB_READ_WRITE_TOKEN`** to enable file uploads via **Vercel Blob client**. If not provided or if the storage limit is reached, the app automatically falls back to storing files as binary inside MongoDB.

- **Environment Variables** – Required keys must be configured (see the **Environment Variables** section for details).

> ⚠️ **MongoDB Network Access**:  
> If deploying to a hosting service (e.g., Vercel, Netlify), make sure your **MongoDB IP whitelist** allows external connections. You can set it to `0.0.0.0/0` (allow from anywhere) during development, but in production it’s strongly recommended to restrict to trusted IPs for better security.

> ⚠️ **Binary Upload Fallback**:  
> When falling back to binary upload, files are stored directly inside MongoDB (as binary). Uploading **large or many files** will increase the database size and may slow down queries. It is recommended to use **Vercel Blob**.

## Configuration (env)

The application relies on environment variables for runtime configuration.

To set them up:

1. Duplicate the provided `.env.example` file.
2. Rename it to `.env`.
3. Replace the placeholder values with your actual configuration values.

You can also override them directly in your hosting environment if supported.

_Required_

- **MONGO_URI** – MongoDB connection string (used by server APIs).
- **MONGO_DB** – The database name.
- **MONGO_COLLECTION** – The collection name for storing.

_Optional_

- **BLOB_READ_WRITE_TOKEN** – Token for enabling `/api/blob` uploads via the **Vercel Blob client**.  
  If not provided, invalid, **or the Vercel Blob limit is reached**, the app automatically falls back to standard **binary file upload**.

- **DEMO_MODE** – Set to `true` to disable all **write operations** including **Add, Update, and Delete** (POST/PUT/DELETE). The app will run in a safe demo mode where data can only be **read**, but not modified.

_Example_

```env
# MongoDB Configuration
MONGO_URI=mongodb+srv://******
MONGO_DB=projectDB
MONGO_COLLECTION=items

# Optional Integrations
BLOB_READ_WRITE_TOKEN=vercel_blob_rw_********
DEMO_MODE=false
```

## Database & File Storage

This project combines **MongoDB** for structured data storage with flexible file & image handling options.

_Database (MongoDB)_

- All Items data is stored inside **MongoDB**.
- The project connects using the native `mongodb` driver for performance and full control.
- Configuration is controlled via environment variables:
  - `MONGO_URI` – connection string
  - `MONGO_DB` – database name
  - `MONGO_COLLECTION` – collection name

> ⚠️ **MongoDB Network Access**:  
> If deploying to a hosting service (e.g., Vercel, Netlify), make sure your **MongoDB IP whitelist** allows external connections. You can set it to `0.0.0.0/0` (allow from anywhere) during development, but in production it’s strongly recommended to restrict to trusted IPs for better security.

- Initial Data

You can either **seed your database** with the provided sample JSON [bit.ly/4fU5dVx](https://xl2c7x22ds7lxnhx.public.blob.vercel-storage.com/items.json) as an initial dataset, or **start with a clean database**.

In both cases, make sure that all future documents strictly follow the **Item Schema** defined below.

Alternatively, you can add items directly through the application UI — built-in validation will ensure that all fields conform to the schema automatically.

Item Schema:

```ts
{
  id: number;
  smallText: string;
  largeText: string;
  number: number;
  status: "active" | "inactive" | "pending";
  date: string;
  favorite: boolean;
  price: number;
  rating: number;
  progress: number;
  color: string;
  email: string;
  phone: string;
  location: {
    lat: number;
    lng: number;
    text: string;
  }
  image: string; // url
  file: string; // url
}
```

Item Example:

```json
{
  "id": 3,
  "smallText": "item 3",
  "largeText": "Ut enim ad minim veniam, quis nostrud exercitation",
  "number": 82,
  "status": "inactive",
  "date": "2024-01-25",
  "favorite": false,
  "price": 890,
  "rating": 2.3,
  "progress": 33,
  "color": "#FFD700",
  "email": "item3@outlook.com",
  "phone": "01123456789",
  "location": {
    "lat": 25.6872,
    "lng": 32.6396,
    "text": "Karnak, Luxor"
  },
  "image": "https://xyzxyz.public.blob.vercel-storage.com/namexyz.png",
  "file": "https://xyzxyz.public.blob.vercel-storage.com/namexyz.pdf"
}
```

_File & Image Storage_

The project supports **two storage strategies** for handling uploaded **files and images**:

**1. Vercel Blob (Recommended)**

- If `BLOB_READ_WRITE_TOKEN` is provided, uploads are stored in **Vercel Blob storage**.
- Each uploaded file is accessible via a **Vercel Blob public link (URL)**.
- Best suited for production environments and large files.

**2. Binary Fallback (MongoDB)**

- If the token is **missing, invalid, or the Vercel Blob usage limit is reached**, uploads fallback to **storing the files as binary directly inside MongoDB**.
- Files are then retrieved through the custom API endpoint: `/api/download?name=<filename>`
- Suitable small files, but uploading many/large files will increase MongoDB size.

> Storage strategy can be switched from the **Settings Page**, allowing choice between **Vercel Blob Storage** and **Binary Uploads**.

## Server API (Endpoints)

Most server endpoints are exposed under `/server/api` using Nuxt server routes.
They support **pagination**, **filtering**, **sorting**, **searching**, and handle **JSON** + **multipart/form-data** (for file uploads).

_`GET /api/items`_

- **Description**: Fetch paginated items with filters, search, and sorting.
- **Query params**:
  - `page` (number, default `1`)
  - `perPage` (number, default `10`)
  - `search` (string) – Performs a full search for text across all searchable fields of the items
  - `sortBy` (string) – Specifies the field to sort by
  - `sortOrder` (string `asc` | `desc`) – Defines the order of sorting: asc for ascending or desc for descending.
  - Any other query key is treated as a filter, based on `FiltersQueries`. Examples:
    - `smallText=lorem` (substring include filter)
    - `status=active` (exact match filter)
    - `price=100,500` (range filter)

**Response example:**

```json
{
  "items": [], // Array of Item objects
  "page": 1,
  "perPage": 10,
  "total": 100
}
```

_`GET /api/items/:id`_

- **Description**: Fetch a single item by its numeric `id`.
- **Response example:**

```json
{
  "_id": "68a0e7976335b77d13c5d218", // related to mongoDB
  "id": 3,
  "smallText": "item 3",
  "largeText": "Ut enim ad minim veniam, quis nostrud exercitation",
  "number": 82,
  "status": "inactive",
  "date": "2024-01-25",
  "favorite": false,
  "price": 890,
  "rating": 2.3,
  "progress": 33,
  "color": "#FFD700",
  "email": "item3@outlook.com",
  "phone": "01123456789",
  "location": {
    "lat": 25.6872,
    "lng": 32.6396,
    "text": "Karnak, Luxor"
  },
  "image": "https://xyzxyz.public.blob.vercel-storage.com/namexyz.png",
  "file": "https://xyzxyz.public.blob.vercel-storage.com/namexyz.pdf"
}
```

_`POST /api/items`_

- **Description**: Create a new item.
- **Behavior**:
  - Automatically assigns a unique incremental `id` for the new item.
  - **File/image Uploads**:
    - **Vercel Blob (if `BLOB_READ_WRITE_TOKEN` is provided)**: Files are uploaded to Vercel Blob, and the item stores the generated Blob URL.
    - **Binary Fallback (if token is missing, invalid, or limit reached)**: Files are stored as binary data directly in MongoDB, and a download URL via `/api/download?name=<filename>` is provided.

_`PUT /api/items/:id`_

- **Description**: Updates an existing item by its `id`.

_`DELETE /api/items`_

- **Description**: Delete multiple items by id.
- **Body Example**:

```json
{ "ids": [1, 2, 3] }
```

_`DELETE /api/items/:id`_

- **Description**: Delete a single item by id.

_`POST /api/blob`_

- **Description**: Proxy upload requests to **Vercel Blob**.
- **Enabled only if** `BLOB_READ_WRITE_TOKEN` is set.
- **Note**: It used dynamically with POST - PUT APIs.

_`GET /api/download?name=<filename>`_

- **Description**: Stream a file stored in GridFS.
- **Headers**: Sets `Content-Type` based on file type.
- **Usage**: Direct download URL for uploaded binary files.

_`GET /api/items/dashboard`_

- **Description**: Returns dashboard summary statistics.
- **Response example:**

```json
{
  "itemsLength": 100,
  "favLength": 45,
  "averageRating": 3.8,
  "averagePrice": 120,
  "allActive": 40,
  "allInactive": 30,
  "allPending": 30,
  "allRating": [], // Rating numbers
  "allProgress": [], // Progress numbers
  "allLocation": [], // Locations objects
  "topProgress": [], // Items objects
  "recentItems": [], // Items objects
  "topFavorites": [] // Items objects
}
```

## Installation

⚠️ Before starting, make sure you have completed all **Prerequisites** (Node.js, package manager, etc.)  
and created a `.env` file (from `.env.example`) with all required environment variables configured.

These steps are explained in the **Prerequisites** and **Configuration (env)** sections above.

⚠️ Without proper configuration, the application will not be able to connect to the database, storage, or other services.

Follow the steps below to install dependencies, run the development server, and build the project for production.

_Firstly: Install Dependencies_

Choose your preferred package manager:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

_Development Server_

Start the app in development mode with hot-reload:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

_Production Build_

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

_Preview Production Build_

Locally preview the production build (simulates deployment):

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

## Support

Thank you for choosing **AbstractDash**! If you need assistance such as installation, configuration or usage feel free to get in touch.

_Updates_

Stay tuned for upcoming releases and enhancements. Keeping your copy up to date ensures you always enjoy the latest features and improvements.
