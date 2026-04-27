# Ex01 Portfolio
## Date: 27.04.2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aaron | Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header class="container">
        <h1>Aaron H</h1>
        <p class="subtitle">Computer Science Engineering Student</p>
        <div class="links">
            <a href="https://github.com/aaronwrites" target="_blank" rel="noopener noreferrer">GitHub</a>
            <a href="#projects">Projects</a>
            <a href="#skills">Skills</a>
        </div>
    </header>

    <main class="container">

        <section id="projects">
            <h2>Projects</h2>

            <article class="project">
                <div class="project-header">
                    <h3>MindVault</h3>
                    <div class="project-links">
                        <a href="https://mindvault-oz42.onrender.com" target="_blank" rel="noopener noreferrer">Live</a>
                        <span class="separator">/</span>
                        <a href="https://github.com/aaronwrites/bookmarkManager" target="_blank"
                            rel="noopener noreferrer">GitHub</a>
                    </div>
                </div>
                <p>A smart bookmarking tool that fetches metadata previews, enables flexible organization with tags, and
                    offers fast search capabilities.</p>
                <ul class="bullet-list">
                    <li>Integrated Cheerio for web scraping to fetch bookmark metadata.</li>
                    <li>Developed bookmark sharing via unique links.</li>
                    <li>Implemented optimistic UI updates using Tanstack Query.</li>
                </ul>
                <div class="tags">
                    <span>React</span>
                    <span>TypeScript</span>
                    <span>TailwindCSS</span>
                    <span>Node.js</span>
                    <span>MongoDB</span>
                </div>
            </article>

            <article class="project">
                <div class="project-header">
                    <h3>KanbanIt</h3>
                    <div class="project-links">
                        <a href="https://github.com/aaronwrites/kanbanit-app" target="_blank"
                            rel="noopener noreferrer">GitHub</a>
                    </div>
                </div>
                <p>A Kanban-style task manager with drag-and-drop functionality, task sorting, and due date tracking.
                </p>
                <ul class="bullet-list">
                    <li>Implemented JWT authentication for secure user login.</li>
                    <li>Developed drag-and-drop functionality for seamless task updates.</li>
                    <li>Built a date-based task filter for organizing tasks by week.</li>
                </ul>
                <div class="tags">
                    <span>HTML</span>
                    <span>CSS</span>
                    <span>JavaScript</span>
                    <span>Express.js</span>
                    <span>MongoDB</span>
                </div>
            </article>

            <article class="project">
                <div class="project-header">
                    <h3>PokeFinder</h3>
                    <div class="project-links">
                        <a href="https://github.com/aaronwrites/pokeFinder" target="_blank"
                            rel="noopener noreferrer">GitHub</a>
                    </div>
                </div>
                <p>A simple React project done with focus on UI design and implementing features like pagination and
                    debounced search.</p>
                <div class="tags">
                    <span>React</span>
                    <span>Recoil</span>
                    <span>PokeAPI</span>
                </div>
            </article>
        </section>

        <section id="skills">
            <h2>Skills</h2>
            <div class="skills-grid">
                <div class="skill-group">
                    <h4>Languages</h4>
                    <p>HTML, CSS, JavaScript, TypeScript</p>
                </div>
                <div class="skill-group">
                    <h4>Libraries & Frameworks</h4>
                    <p>NextJS, React, TailwindCSS, Motion, Node.js, Express.js</p>
                </div>
                <div class="skill-group">
                    <h4>Databases & ORMs</h4>
                    <p>MongoDB, PostgreSQL, Prisma</p>
                </div>
                <div class="skill-group">
                    <h4>Cloud & Deployment</h4>
                    <p>AWS, Vercel, Render</p>
                </div>
            </div>
        </section>

        <section id="education">
            <h2>Education</h2>
            <article class="edu-item">
                <div class="edu-header">
                    <h3>Saveetha Engineering College</h3>
                    <span class="date">Expected 2027</span>
                </div>
                <p>BE Computer Science and Engineering</p>
            </article>
        </section>

        <section id="certifications">
            <h2>Certifications</h2>
            <ul class="simple-list">
                <li>AWS Certified Cloud Practitioner</li>
                <li>Red Hat Certified System Administrator</li>
            </ul>
        </section>

    </main>

    <footer class="container">
        <p>&copy; 2026 Aaron H</p>
    </footer>
</body>

</html>

```

styles.css
```
:root {
    --bg-color: #fcfcfc;
    --text-primary: #111111;
    --text-secondary: #555555;
    --border-color: #e5e5e5;
    --accent-color: #000000;
    --hover-bg: #f5f5f5;
    --font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}

@media (prefers-color-scheme: dark) {
    :root {
        --bg-color: #111111;
        --text-primary: #f5f5f5;
        --text-secondary: #a3a3a3;
        --border-color: #2a2a2a;
        --accent-color: #ffffff;
        --hover-bg: #1f1f1f;
    }
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-family);
    background-color: var(--bg-color);
    color: var(--text-primary);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

a {
    color: var(--accent-color);
    text-decoration: none;
    transition: color 0.15s ease, opacity 0.15s ease;
}

a:hover {
    text-decoration: underline;
}

.container {
    max-width: 650px;
    margin: 0 auto;
    padding: 2rem 1.5rem;
}

header {
    margin-top: 4rem;
    margin-bottom: 4rem;
}

h1 {
    font-size: 2rem;
    font-weight: 600;
    letter-spacing: -0.03em;
    margin-bottom: 0.25rem;
}

.subtitle {
    color: var(--text-secondary);
    font-size: 1.1rem;
    margin-bottom: 1.5rem;
    font-weight: 400;
}

.links {
    display: flex;
    gap: 1.25rem;
    font-size: 0.95rem;
    font-weight: 500;
}

section {
    margin-bottom: 3.5rem;
}

h2 {
    font-size: 1.25rem;
    font-weight: 600;
    margin-bottom: 1.5rem;
    padding-bottom: 0.5rem;
    border-bottom: 1px solid var(--border-color);
    letter-spacing: -0.01em;
}

h3 {
    font-size: 1.1rem;
    font-weight: 500;
    letter-spacing: -0.01em;
}

.project {
    margin-bottom: 2.5rem;
}

.project:last-child {
    margin-bottom: 0;
}

.project-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 0.5rem;
}

.project-links {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.85rem;
}

.separator {
    color: var(--text-secondary);
}

.project p {
    color: var(--text-secondary);
    font-size: 0.95rem;
    margin-bottom: 1rem;
    line-height: 1.5;
}

.bullet-list {
    list-style-type: none;
    margin-bottom: 1rem;
}

.bullet-list li {
    font-size: 0.9rem;
    color: var(--text-secondary);
    margin-bottom: 0.4rem;
    padding-left: 1rem;
    position: relative;
}

.bullet-list li::before {
    content: "—";
    position: absolute;
    left: 0;
    color: var(--border-color);
}

.tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

.tags span {
    font-size: 0.75rem;
    padding: 0.2rem 0.6rem;
    background-color: var(--hover-bg);
    border: 1px solid var(--border-color);
    border-radius: 4px;
    color: var(--text-primary);
}

.skills-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
}

@media (min-width: 600px) {
    .skills-grid {
        grid-template-columns: 1fr 1fr;
    }
}

.skill-group h4 {
    font-size: 0.95rem;
    font-weight: 500;
    margin-bottom: 0.25rem;
}

.skill-group p {
    font-size: 0.9rem;
    color: var(--text-secondary);
}

.edu-item {
    margin-bottom: 1.5rem;
}

.edu-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 0.25rem;
}

.date {
    font-size: 0.85rem;
    color: var(--text-secondary);
}

.edu-item p {
    font-size: 0.95rem;
    color: var(--text-primary);
}

.meta-info {
    font-size: 0.9rem !important;
    color: var(--text-secondary) !important;
    margin-top: 0.25rem;
}

.simple-list {
    list-style-type: none;
}

.simple-list li {
    font-size: 0.95rem;
    margin-bottom: 0.5rem;
    color: var(--text-primary);
}

footer {
    text-align: left;
    color: var(--text-secondary);
    font-size: 0.85rem;
    margin-top: 4rem;
    margin-bottom: 2rem;
    padding-top: 2rem;
    border-top: 1px solid var(--border-color);
}

```

## OUTPUT
<img width="1912" height="1188" alt="Screenshot 2026-04-27 at 1 54 12 PM" src="https://github.com/user-attachments/assets/9fd51b16-7cd7-49ec-8be6-523e3145cd8a" />
<img width="1912" height="1188" alt="Screenshot 2026-04-27 at 1 54 14 PM" src="https://github.com/user-attachments/assets/3c44a29f-d452-4357-90d3-c1758ff6bbb9" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
