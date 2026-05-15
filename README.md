# Itskay Pickett Portfolio

A modern, responsive Angular 18 single-page application portfolio website for ItsKayPickett.com.

## Features

- 🎨 Modern, responsive design with gradient theming
- 📱 Mobile-first approach
- 🎥 YouTube video embedding support
- 🖼️ Image gallery with modal viewer
- 📧 Contact form
- ⚡ Built with Angular 18 (latest)
- 📦 Standalone components
- 🎯 Type-safe with strict TypeScript
- 🗺️ Clean path aliases for imports

## Pages

- **Home** - Hero section with call-to-action
- **Projects** - Portfolio of projects with tags
- **About** - Personal bio and skills
- **Community** - Community involvement and volunteer work
- **Interviews** - Media appearances with embedded videos
- **Artwork** - Image gallery with modal viewer
- **Contact** - Contact form for inquiries

## Getting Started

### Prerequisites

- Node.js 18+
- npm 9+

### Installation

```bash
git clone https://github.com/JohnBieniek/itskayPickett-portfolio.git
cd itskayPickett-portfolio
npm install
```

### Development

```bash
npm start
```

Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

### Production Build

```bash
npm run build:prod
```

The build artifacts will be stored in the `dist/` directory.

## Project Structure

```
src/
├── app/
│   ├── components/
│   │   ├── header/
│   │   └── footer/
│   ├── pages/
│   │   ├── home/
│   │   ├── projects/
│   │   ├── about/
│   │   ├── community/
│   │   ├── interviews/
│   │   ├── artwork/
│   │   └── contact/
│   ├── services/
│   ├── models/
│   ├── app.component.ts
│   ├── app.routes.ts
│   └── app.config.ts
├── assets/
├── styles.scss
├── index.html
└── main.ts
```

## Import Aliases

The project includes path aliases for cleaner imports:

```typescript
@app/*        // src/app/*
@components/* // src/app/components/*
@pages/*      // src/app/pages/*
@services/*   // src/app/services/*
@models/*     // src/app/models/*
@assets/*     // src/assets/*
```

## Customization

### Update Content

1. Edit component templates in `src/app/pages/`
2. Update styling in `styles.scss` and component styles
3. Add your images to `src/assets/`
4. Update social links in the footer component

### Add YouTube Videos

Update the `videoId` in the interviews component:

```typescript
interviews: Interview[] = [
  {
    id: 1,
    title: 'My Interview',
    videoId: 'YOUR_YOUTUBE_VIDEO_ID',
  },
];
```

### Add Images

1. Place images in `src/assets/`
2. Reference them in components:

```html
<img src="assets/my-image.jpg" alt="Description" />
```

## Technologies

- **Angular** 18
- **TypeScript** 5.4
- **RxJS** 7.8
- **SCSS** for styling
- **Standalone Components** (no NgModule required)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

MIT License - feel free to use this for your portfolio!

## Support

For issues or questions, please open an issue on GitHub.
