<div align="center">

  <!-- Logo -->
  <a href="https://s-cms.dev" target="_blank" rel="noopener">
    <img src="LOGO_URL_HERE.svg" alt="Smart CMS" height="84">
  </a>

  <!-- Name -->
  <h1 style="margin:16px 0 8px; font-size:34px;">Smart CMS</h1>

  <!-- Tagline -->
  <p style="margin:0 0 12px; font-size:16px;">
    <strong>Simple. Strong. Smart.</strong>
  </p>

  <!-- Short intro -->
  <p style="max-width:720px; margin:0 auto 14px; line-height:1.6;">
    A modern modular CMS for building both simple and custom websites with independent, reusable blocks.
    Built on Laravel&nbsp;11 and Filament, optimized for speed, flexibility, and developer happiness.
  </p>

  <!-- Badges -->
  <p>
    <a href="https://github.com/s-cms/blob/main/LICENSE">
      <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg">
    </a>
    <img alt="PHP 8.3+" src="https://img.shields.io/badge/PHP-8.3%2B-8892BF.svg">
    <img alt="Laravel 12" src="https://img.shields.io/badge/Laravel-12-FF2D20.svg">
    <img alt="Filament 4" src="https://img.shields.io/badge/Filament-4-16A34A.svg">
    <img alt="Tailwind CSS 4" src="https://img.shields.io/badge/Tailwind-4-06B6D4.svg">
    <a href="https://github.com/s-cms/stargazers">
      <img alt="GitHub stars" src="https://img.shields.io/github/stars/s-cms?style=social">
    </a>
  </p>

  <!-- Quick nav -->
  <p>
    <a href="#installation"><b>Install</b></a> •
    <a href="#key-features"><b>Features</b></a> •
    <a href="#technology-stack"><b>Tech stack</b></a> •
    <a href="#quick-start"><b>Quick start</b></a> •
    <a href="#contact--support"><b>Support</b></a> •
    <a href="https://github.com/s-cms/issues"><b>Issues</b></a>
  </p>

  <!-- Divider -->
  <img src="https://img.shields.io/badge/- -white.svg" alt="" width="0" height="12"><br>
</div>

It was born out of years of experience working with popular CMS platforms and the frustration of repeatedly rewriting the same things. Smart CMS offers a clean, scalable architecture with reusable page blocks, unlimited layout templates, customizable content sections, dynamic SEO controls, and much more — all without needing to touch code.

---

## 🧩 Key Features

- 🧱 **Modular template system**  
  Define and reuse an unlimited number of layout templates for static pages, sections, categories, or even entire content modules — all configurable from the admin panel, without code.

- 🔗 **Independent content blocks (Sections)**  
  Build websites from flexible, reusable sections like FAQ, sliders, or CTA blocks. Assign them globally or override per page with custom content.

- 📂 **Custom content types (Sections & Categories)**  
  Create dynamic content structures (e.g. Blog, Team, News, Products) with configurable layouts, fields, and SEO, without touching code.

- 🎨 **Flexible page rendering**  
  Each page, category, or section can have a unique design. Templates can be swapped or reused dynamically, depending on structure.

- ⚙️ **Developer-first architecture**  
  Built on Laravel 11 and Filament, optimized for speed, scalability, and extendability. Clean backend structure with logical defaults.

- 🛡 **Simple roles & admin UX**  
  One super admin + unlimited regular admins. Clean admin panel UI powered by Filament — fast and easy to navigate.

- 📈 **SEO-ready by default**  
  Built-in SEO controls for every page. Includes OpenGraph, structured data, and per-page script injection. Image optimization and lazy-loading included.

- 📬 **Form builder & notifications**  
  Create forms from the UI with no code. Receive responses via email and Telegram. Integrated notification logic for admin users.

- 🧱 **Scalable section inheritance**  
  Section content can be reused, overridden, or cloned automatically when customized — supporting both global and per-page variants.

- 🚀 **Future-ready extension system**  
  Extension store coming soon: install add-ons, plugins and modules directly from the admin panel (when server supports Composer).

---

## 🛠 Technology Stack

Smart CMS is built with a modern, developer-friendly tech stack:

- **Laravel 12** – robust PHP framework with clean architecture  
- **Filament** – powerful admin panel system with beautiful UI  
- **PHP 8.3+** – fast and modern backend language  
- **Tailwind CSS 4** – utility-first styling for front-end flexibility  
- **Alpine.js** – lightweight interactivity without complex JS frameworks  
- **MySQL / SQLite** – flexible database support  
- **Composer** – dependency management and upcoming plugin store  
- **Node.js & Vite** – modern frontend build process  
- **Docker (optional)** – fast deployment & local development

---

## 🚀 Installation

Smart CMS can be installed either as a developer package or as a ready-to-use standalone system.

### 🧑‍💻 For Developers (Composer-based)

```bash
composer create-project laravel/laravel your-project-directory
```

1. Open `composer.json` and change:
   ```json
   "minimum-stability": "dev"
   ```

2. Configure `.env` database connection  
   (supports **SQLite** or **MySQL**)

3. Require Smart CMS Kit:

```bash
composer require smart-cms/kit ^1.0
```

4. Run the installer:

```bash
php artisan kit:install
```

5. Create the admin panel endpoint:

```bash
php artisan filament:panel
# Example: enter "admin" → your panel will be at /admin
```

6. Register the plugin inside `App\Providers\Filament\AdminPanelProvider`:

```php
->plugins([
    \SmartCms\Kit\KitPlugin::make(),
])
```

7. Link storage and build assets:

```bash
php artisan storage:link
npm install && npm run build
```

8. Create admin user:

```bash
php artisan make:admin
```

9. Run development servers:

```bash
php artisan serve     # Laravel dev server
npm run dev           # Vite development mode
```

---

### 📦 For Users (non-developers)

Smart CMS will be available as:

- 🔧 A **standalone archive** to upload and deploy on shared hosting  
- 🐳 A **Docker-based version** for instant local development or production  
- 📁 Supports **SQLite or MySQL** out of the box

---

## ⚡ Quick Start

Once installed, you can access the admin panel and start building immediately.

### 🔐 Admin login

- **URL:** `/admin`
- **Email:** set during `php artisan make:admin`
- **Password:** set during `php artisan make:admin`

> If you're using the prebuilt archive or Docker version, the default credentials will be provided in the installation instructions.

### 🧪 Local development

```bash
php artisan serve     # Launch Laravel's dev server
npm run dev           # Run frontend build in watch mode (Vite)
```

Smart CMS is ready to use immediately after installation — no additional configuration required.

---

## 🪪 License

Smart CMS is open-source software licensed under the [MIT license](LICENSE).

---

## 📬 Contact & Support

- 🌐 Website: [https://s-cms.dev](https://s-cms.dev)
- 💬 Telegram (support): *coming soon*
- 📩 Email: support@s-cms.dev
- 🐛 Report issues: [GitHub Issues](https://github.com/s-cms/issues)
