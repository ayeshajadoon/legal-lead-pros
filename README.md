# Landing Page Project

This is a responsive landing page built using HTML, CSS, and Bootstrap.

## Technologies Used
- HTML5
- CSS3
- Bootstrap 5.3.2

## Screen Breakpoints
The website is responsive and optimized for the following screen sizes:
- Desktop: 1920px, 1680px, 1600px, 1536px, 1440px, 1366px, 1280px, 1200px
- iPad Pro: 1024px
- iPad: 768px-820px
- Mobile: 0px-602px

## Project Structure
```
├── index.html
├── css/
│   └── style.css
└── images/
```

## Setup
1. Clone the repository
2. Open `index.html` in your browser

## Development
- Custom CSS is written in `css/style.css`
- Bootstrap is used for responsive grid system and components
- No inline CSS is used 

# Deploying to Vercel

This project is a static HTML/CSS website. To deploy it on Vercel, follow these steps:

## 1. Create a `vercel.json` file
Add the following configuration to the root of your project:

```json
{
  "version": 2,
  "public": true,
  "builds": [],
  "routes": [
    { "src": "/(.*)", "dest": "/index.html" }
  ]
}
```

This tells Vercel to serve `index.html` for all routes (good for single-page sites).

## 2. Deploying
- Push your code to a GitHub/GitLab/Bitbucket repository.
- Go to [Vercel](https://vercel.com/) and import your repository.
- Set the **Framework Preset** to **Other** (for static sites).
- Set the **Output Directory** to `.` (the root directory).
- Deploy!

## Notes
- All your assets (CSS, images, fonts) are referenced with relative paths, so no changes are needed.
- If you add more HTML files, you may want to adjust the `vercel.json` routes. 