# front-end-using-html-templates
front-end using html templates
Internship Task 2 – Vite + Nunjucks Setup
Project Overview:
This project recreates Internship Task 1 using a mandatory tech stack:
Nunjucks as the templating engine
Vite as the bundler
The final output is static HTML pages generated into the dist/ folder.
project-root/
│
├─ src/
│   ├─ templates/
│   │   ├─ layouts/
│   │   │   └─ base.njk
│   │   ├─ partials/
│   │   │   └─ navbar.njk
│   │   └─ pages/
│   │       ├─ index.njk
│   │       ├─ aboutus.njk
│   │       └─ contact.njk
│   │
│   └─ assets/
│       └─ css/
│           └─ style.css
│
├─ index.html          (Vite entry file)
├─ vite.config.js
├─ package.json
├─ dist/               (auto-generated)
└─ README.md
next install node js after installing .we run the commands

npm install - This creates the node_modules folder automatically.
npm run build -Compiles all .njk files,Copies CSS assets,Generates final HTML into dist/
npm run dev -Start Development Server
this will be the dist folder
dist/
│
├─ index.html
├─ aboutus.html
├─ contact.html
├─ assets/
│   └─ style.css
Notes:
CSS is copied to dist only when referenced from index.html
Bootstrap CDN does not get copied (CDN loads from internet)
Any change in templates requires re-running npm run build

Conclusion
This project strictly follows:
Required tech stack
Proper folder structure
Clean separation of templates and assets
Automatic build using Vite
