# 🚀 Oussama Mbarek - Portfolio

A clean, minimalist portfolio website built with **Astro** and **Tailwind CSS v4**. This modern portfolio showcases my work, experience, and skills as a Computer Science student and developer. Feel free to use it as a template for your own portfolio!

[![Astro](https://img.shields.io/badge/Astro-5.12.3-FF5D01?style=flat&logo=astro&logoColor=white)](https://astro.build)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1.11-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

## ✨ Features

- **🎨 Single Configuration File**: All content and styling managed through one simple TypeScript file
- **🌙 Dark Mode**: Built-in theme toggle for light/dark preferences
- **📱 Fully Responsive**: Mobile-first design that looks great on all devices
- **⚡ Lightning Fast**: Static site generation with Astro for optimal performance
- **🎯 Easy Customization**: No need to touch component code - just update the config
- **🔗 Social Links**: Integrated support for email, LinkedIn, Instagram, and GitHub
- **📄 CV Download**: Direct download link for your resume/CV
- **🖼️ Profile Image**: Customizable profile picture
- **💼 Project Showcase**: Display your work with descriptions, links, and tech stacks
- **🏢 Experience Section**: Timeline of your professional experience
- **🎓 Education Section**: Academic background and achievements
- **🛠️ Skills Display**: Highlight your technical skills
- **♿ Accessibility**: Semantic HTML and accessible components

## 🖥️ Tech Stack

- **[Astro](https://astro.build)** - Modern static site generator
- **[Tailwind CSS v4](https://tailwindcss.com)** - Utility-first CSS framework
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe configuration
- **[Tabler Icons](https://tabler.io/icons)** - Beautiful icon set
- **[IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono)** - Professional monospace font

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ installed on your machine
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/mbarekoussama/Oussama-Portfolio.git
   cd Oussama-Portfolio
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   
   Navigate to `http://localhost:4321` to see your portfolio

## 📁 Project Structure

```
/
├── public/
│   ├── favicon.svg          # Website favicon
│   ├── profile.png          # Profile image
│   └── oussama mbarek.pdf   # CV/Resume PDF
├── src/
│   ├── components/
│   │   ├── About.astro      # About section
│   │   ├── Education.astro  # Education section
│   │   ├── Experience.astro # Experience section
│   │   ├── Footer.astro     # Footer component
│   │   ├── Header.astro     # Header/navigation
│   │   ├── Hero.astro       # Hero/landing section
│   │   ├── Projects.astro   # Projects showcase
│   │   └── ThemeToggle.astro # Dark mode toggle
│   ├── pages/
│   │   └── index.astro      # Main page layout
│   └── config.ts            # **Site configuration**
├── astro.config.mjs         # Astro configuration
├── package.json
├── tsconfig.json
└── README.md
```

## ⚙️ Configuration

All content is managed through a single file: **`src/config.ts`**

### Basic Information

```typescript
export const siteConfig = {
  name: "Your Name",
  title: "Your Title/Role",
  description: "Brief description for SEO",
  accentColor: "#1d4ed8",  // Primary color used throughout the site
  profileImage: "/profile.png",
  cvUrl: "/your-cv.pdf",
  // ...
}
```

### Social Links

Add or remove any social links:

```typescript
social: {
  email: "your.email@example.com",
  linkedin: "https://linkedin.com/in/yourprofile",
  instagram: "https://instagram.com/yourhandle",
  github: "https://github.com/yourusername",
}
```

### Projects

Add your projects with descriptions, links, and tech stacks:

```typescript
projects: [
  {
    name: "Project Name",
    description: "Detailed description of your project",
    link: "https://project-url.com",
    skills: ["React", "Node.js", "MongoDB"],
  },
  // Add more projects...
]
```

### Experience

Showcase your work history:

```typescript
experience: [
  {
    company: "Company Name",
    title: "Job Title",
    dateRange: "Jan 2023 - Present",
    bullets: [
      "Achievement or responsibility",
      "Another achievement",
    ],
  },
]
```

### Education

Display your academic background:

```typescript
education: [
  {
    school: "University Name",
    degree: "Degree Name",
    dateRange: "2020 - 2024",
    achievements: [
      "Notable achievement",
      "Another achievement",
    ],
  },
]
```

## 🎨 Customization Guide

### 1. Update Your Information

Edit `src/config.ts` with your personal information, projects, experience, and education.

### 2. Add Your Images

- Replace `public/profile.png` with your profile photo
- Replace the CV PDF in `public/` with your own resume (keep the file extension as `.pdf`)
- Update the file names in `config.ts` if needed

### 3. Change the Accent Color

Modify the `accentColor` property in `config.ts`. Any valid CSS color works:
```typescript
accentColor: "#1d4ed8"  // Blue
accentColor: "#dc2626"  // Red
accentColor: "#059669"  // Green
```

### 4. Update Favicon

Replace `public/favicon.svg` with your own icon

### 5. Customize Components (Optional)

If you need deeper customization, you can modify the Astro components in `src/components/`. All components use Tailwind utility classes for styling.

## 📦 Available Commands

| Command           | Action                                       |
|-------------------|----------------------------------------------|
| `npm install`     | Install dependencies                         |
| `npm run dev`     | Start development server at `localhost:4321` |
| `npm run build`   | Build production site to `./dist/`          |
| `npm run preview` | Preview production build locally             |
| `npm run astro`   | Run Astro CLI commands                       |

## 🚀 Deployment

### Deploy to Vercel (Recommended)

1. Push your code to GitHub
2. Import your repository on [Vercel](https://vercel.com)
3. Vercel will auto-detect Astro and configure build settings
4. Click "Deploy"

### Deploy to Netlify

1. Push your code to GitHub
2. Import your repository on [Netlify](https://netlify.com)
3. Build command: `npm run build`
4. Publish directory: `dist`
5. Click "Deploy"

### Deploy to GitHub Pages

1. Update `astro.config.mjs` with your site URL
2. Follow the [Astro GitHub Pages deployment guide](https://docs.astro.build/en/guides/deploy/github/)

### Other Platforms

Astro supports deployment to most static hosting platforms. Check the [official deployment guide](https://docs.astro.build/en/guides/deploy/) for more options.

## 🔧 Development Tips

- **Hot Reload**: The development server automatically reloads when you save changes
- **Type Safety**: Use TypeScript in `config.ts` for autocomplete and type checking
- **Conditional Sections**: Remove entries from arrays in config to hide entire sections
- **Icons**: Use [Tabler Icons](https://tabler.io/icons) for consistency

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/mbarekoussama/Oussama-Portfolio/issues).

## 👤 Author

**Mbarek Oussama**

- GitHub: [@mbarekoussama](https://github.com/mbarekoussama)
- LinkedIn: [Oussama Mbarek](https://www.linkedin.com/in/oussama-mbarek)
- Email: mbarekoussama2004@gmail.com

## ⭐ Show Your Support

Give a ⭐️ if this project helped you!

---

Built with ❤️ using [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com)
