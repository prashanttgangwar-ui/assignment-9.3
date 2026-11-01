## 1. Aim

To create a complete responsive landing page using CSS Grid and Flexbox that works properly on mobile, tablet, and desktop screens.

## 2. Objectives

- Create a website header and navigation bar.
- Design a hero section with text, buttons, and an image.
- Add six feature cards.
- Use CSS Grid for the main page and card layouts.
- Use Flexbox for navigation, hero alignment, and card content.
- Make the website responsive using media queries.
- Convert multiple columns into a single-column layout on mobile.
- Test the webpage on different screen sizes.

## 3. Project Structure

Create the following files:

```text
Assignment-9.3/
├── index.html
├── style.css
└── screenshots/
    ├── mobile.png
    ├── tablet.png
    └── desktop.png
```

## 4. HTML Code — index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta
        name="description"
        content="A responsive landing page built with CSS Grid and Flexbox."
    >

    <title>NovaSpace | Responsive Landing Page</title>

    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header and Navigation -->
    <header class="site-header">
        <div class="navbar container">

            <a href="#home" class="logo">
                Nova<span>Space</span>
            </a>

            <nav class="nav-links" aria-label="Main navigation">
                <a href="#home">Home</a>
                <a href="#features">Features</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>
            </nav>

            <a href="#features" class="nav-button">Get Started</a>

        </div>
    </header>

    <main>

        <!-- Hero Section -->
        <section class="hero container" id="home">

            <div class="hero-content">
                <p class="eyebrow">BUILD SOMETHING AMAZING</p>

                <h1>
                    Turn Your Ideas Into
                    <span>Digital Experiences</span>
                </h1>

                <p class="hero-description">
                    Discover a smarter way to organize your work,
                    manage projects, and bring your creative ideas
                    to life with modern digital tools.
                </p>

                <div class="hero-actions">
                    <a href="#features" class="button button-primary">
                        Explore Features
                    </a>

                    <a href="#about" class="button button-secondary">
                        Learn More
                    </a>
                </div>

                <div class="hero-stats">
                    <div>
                        <strong>120+</strong>
                        <span>Projects Created</span>
                    </div>

                    <div>
                        <strong>95%</strong>
                        <span>User Satisfaction</span>
                    </div>

                    <div>
                        <strong>24/7</strong>
                        <span>Access Anywhere</span>
                    </div>
                </div>
            </div>

            <div class="hero-visual">
                <img
                    src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=1200&q=85"
                    alt="Laptop displaying a web development workspace"
                    width="1200"
                    height="800"
                >

                <div class="floating-card">
                    <span class="success-icon">✓</span>
                    <div>
                        <strong>Project Updated</strong>
                        <p>Your progress is looking great!</p>
                    </div>
                </div>
            </div>

        </section>

        <!-- Features Section -->
        <section class="features-section" id="features">
            <div class="container">

                <div class="section-heading">
                    <p class="eyebrow">OUR FEATURES</p>

                    <h2>Everything You Need to Grow</h2>

                    <p>
                        Powerful features designed to make your
                        workflow simple, organized, and productive.
                    </p>
                </div>

                <div class="features-grid">

                    <!-- Feature 1 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-purple">01</div>

                        <div class="feature-content">
                            <h3>Smart Dashboard</h3>

                            <p>
                                View your projects, tasks, and progress
                                in one organized workspace.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <!-- Feature 2 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-blue">02</div>

                        <div class="feature-content">
                            <h3>Team Collaboration</h3>

                            <p>
                                Work together, share ideas, and keep
                                everyone connected to the same goals.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <!-- Feature 3 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-green">03</div>

                        <div class="feature-content">
                            <h3>Task Management</h3>

                            <p>
                                Organize your daily tasks and focus
                                on the work that matters most.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <!-- Feature 4 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-orange">04</div>

                        <div class="feature-content">
                            <h3>Progress Tracking</h3>

                            <p>
                                Monitor project milestones and
                                understand how your work is progressing.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <!-- Feature 5 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-pink">05</div>

                        <div class="feature-content">
                            <h3>Secure Workspace</h3>

                            <p>
                                Keep your project information organized
                                with security-conscious design.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                    <!-- Feature 6 -->
                    <article class="feature-card">
                        <div class="feature-icon icon-yellow">06</div>

                        <div class="feature-content">
                            <h3>Responsive Design</h3>

                            <p>
                                Access your workspace through a layout
                                that adapts to different screen sizes.
                            </p>

                            <a href="#about" class="feature-link">
                                Learn more →
                            </a>
                        </div>
                    </article>

                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="about-section container" id="about">

            <div class="about-image">
                <img
                    src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=1200&q=85"
                    alt="Team members collaborating on a project"
                    width="1200"
                    height="800"
                    loading="lazy"
                >
            </div>

            <div class="about-content">
                <p class="eyebrow">WHY NOVASPACE?</p>

                <h2>Designed for the Way You Work</h2>

                <p>
                    NovaSpace represents a modern approach to organizing
                    ideas and projects. Its clean interface helps users
                    focus on important tasks without unnecessary clutter.
                </p>

                <ul class="benefits-list">
                    <li>✓ Simple and user-friendly interface</li>
                    <li>✓ Flexible layouts for different devices</li>
                    <li>✓ Organized and easy-to-read content</li>
                    <li>✓ Consistent design and spacing</li>
                </ul>

                <a href="#contact" class="button button-primary">
                    Get Started Today
                </a>
            </div>

        </section>

        <!-- Call to Action -->
        <section class="cta-section" id="contact">
            <div class="container cta-content">
                <div>
                    <p class="eyebrow">YOUR NEXT STEP</p>

                    <h2>Ready to Build Something Great?</h2>

                    <p>
                        Start exploring a better way to manage your
                        ideas and creative projects.
                    </p>
                </div>

                <a href="mailto:hello@example.com" class="button cta-button">
                    Contact Us
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="site-footer">
        <div class="container footer-content">

            <a href="#home" class="logo">
                Nova<span>Space</span>
            </a>

            <p>
                &copy; 2026 NovaSpace. Created for Assignment 9.3.
            </p>

            <a href="#home" class="back-to-top">Back to top ↑</a>

        </div>
    </footer>

</body>
</html>
```

## 5. CSS Code — style.css

```css
/* =====================================
   1. Global Styles
===================================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: #20263a;
    background-color: #ffffff;
    line-height: 1.7;
    min-width: 0;
}

a {
    color: inherit;
    text-decoration: none;
}

img {
    display: block;
    max-width: 100%;
    height: auto;
}

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding-left: 16px;
    padding-right: 16px;
}

h1,
h2,
h3,
p {
    overflow-wrap: break-word;
}

:focus-visible {
    outline: 3px solid #8b72f5;
    outline-offset: 4px;
}

/* =====================================
   2. Header and Navbar
   Flexbox Layout
===================================== */

.site-header {
    background-color: #ffffff;
    border-bottom: 1px solid #ececf4;
}

.navbar {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 16px;
    padding-top: 18px;
    padding-bottom: 18px;
}

.logo {
    font-size: 25px;
    font-weight: 800;
    color: #20263a;
    letter-spacing: -1px;
    white-space: nowrap;
}

.logo span {
    color: #7255e8;
}

.nav-links {
    display: flex;
    flex-wrap: wrap;
    gap: 10px 20px;
}

.nav-links a {
    color: #647087;
    font-size: 14px;
    transition: color 0.2s ease;
}

.nav-links a:hover {
    color: #7255e8;
}

.nav-button {
    display: inline-block;
    padding: 10px 18px;
    border-radius: 8px;
    background-color: #7255e8;
    color: #ffffff;
    font-size: 14px;
    font-weight: 700;
}

.nav-button:hover {
    background-color: #5b40cb;
}

/* =====================================
   3. Hero Section
   CSS Grid for Main Layout
===================================== */

.hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: 36px;
    align-items: center;
    padding-top: 56px;
    padding-bottom: 64px;
}

.hero-content {
    min-width: 0;
}

.eyebrow {
    color: #7255e8;
    font-size: 12px;
    font-weight: 800;
    letter-spacing: 1.8px;
    margin-bottom: 12px;
}

.hero h1 {
    font-size: clamp(34px, 7vw, 60px);
    line-height: 1.12;
    letter-spacing: -2px;
    margin-bottom: 20px;
}

.hero h1 span {
    color: #7255e8;
}

.hero-description {
    max-width: 540px;
    color: #68738a;
    font-size: 16px;
    margin-bottom: 26px;
}

.hero-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    align-items: center;
}

.button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 12px 20px;
    border-radius: 8px;
    font-size: 14px;
    font-weight: 700;
    transition: background-color 0.2s ease;
}

.button-primary {
    background-color: #7255e8;
    color: #ffffff;
}

.button-primary:hover {
    background-color: #5b40cb;
}

.button-secondary {
    background-color: #f0edff;
    color: #6045cf;
}

.button-secondary:hover {
    background-color: #e5dfff;
}

.hero-stats {
    display: flex;
    flex-wrap: wrap;
    gap: 22px;
    margin-top: 34px;
}

.hero-stats div {
    display: flex;
    flex-direction: column;
    min-width: 0;
}

.hero-stats strong {
    font-size: 21px;
    line-height: 1.4;
}

.hero-stats span {
    color: #7a8498;
    font-size: 11px;
}

.hero-visual {
    position: relative;
    min-width: 0;
}

.hero-visual > img {
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 18px;
}

.floating-card {
    display: flex;
    align-items: center;
    gap: 12px;
    position: relative;
    margin: -22px 12px 0;
    padding: 15px;
    border-radius: 12px;
    background-color: #ffffff;
    box-shadow: 0 8px 30px rgba(32, 38, 58, 0.12);
}

.success-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-shrink: 0;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background-color: #dcfce7;
    color: #15803d;
    font-weight: 800;
}

.floating-card strong {
    display: block;
    font-size: 13px;
}

.floating-card p {
    color: #7a8498;
    font-size: 12px;
}

/* =====================================
   4. Features Section
   CSS Grid for Cards
===================================== */

.features-section {
    padding: 64px 0;
    background-color: #f7f8fc;
}

.section-heading {
    max-width: 650px;
    margin: 0 auto 36px;
    text-align: center;
}

.section-heading h2 {
    font-size: clamp(27px, 5vw, 40px);
    line-height: 1.2;
    letter-spacing: -1px;
    margin-bottom: 14px;
}

.section-heading > p:last-child {
    color: #68738a;
    font-size: 15px;
}

.features-grid {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    gap: 18px;
}

.feature-card {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 18px;
    min-width: 0;
    padding: 24px;
    background-color: #ffffff;
    border: 1px solid #e9eaf2;
    border-radius: 14px;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.feature-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 28px rgba(32, 38, 58, 0.08);
}

.feature-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    width: 48px;
    height: 48px;
    border-radius: 12px;
    font-size: 15px;
    font-weight: 800;
}

.icon-purple {
    color: #7255e8;
    background-color: #eee9ff;
}

.icon-blue {
    color: #2563eb;
    background-color: #dbeafe;
}

.icon-green {
    color: #15803d;
    background-color: #dcfce7;
}

.icon-orange {
    color: #c2410c;
    background-color: #ffedd5;
}

.icon-pink {
    color: #be185d;
    background-color: #fce7f3;
}

.icon-yellow {
    color: #a16207;
    background-color: #fef3c7;
}

.feature-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    flex: 1;
    width: 100%;
    min-width: 0;
}

.feature-content h3 {
    font-size: 18px;
    margin-bottom: 8px;
}

.feature-content p {
    color: #68738a;
    font-size: 14px;
    margin-bottom: 18px;
}

.feature-link {
    margin-top: auto;
    color: #7255e8;
    font-size: 13px;
    font-weight: 800;
}

.feature-link:hover {
    color: #4f35bc;
}

/* =====================================
   5. About Section
===================================== */

.about-section {
    display: grid;
    grid-template-columns: minmax(0, 1fr);
    align-items: center;
    gap: 36px;
    padding-top: 64px;
    padding-bottom: 64px;
}

.about-image {
    min-width: 0;
}

.about-image img {
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 16px;
}

.about-content {
    min-width: 0;
}

.about-content h2 {
    font-size: clamp(28px, 5vw, 42px);
    line-height: 1.2;
    letter-spacing: -1px;
    margin-bottom: 18px;
}

.about-content > p:not(.eyebrow) {
    color: #68738a;
    font-size: 15px;
    margin-bottom: 20px;
}

.benefits-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
    list-style: none;
    margin-bottom: 26px;
}

.benefits-list li {
    color: #455168;
    font-size: 14px;
}

/* =====================================
   6. Call to Action Section
===================================== */

.cta-section {
    padding: 44px 0;
    background-color: #f0edff;
}

.cta-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 24px;
}

.cta-content h2 {
    font-size: clamp(26px, 5vw, 36px);
    line-height: 1.25;
    margin-bottom: 12px;
}

.cta-content p:not(.eyebrow) {
    color: #68738a;
    font-size: 14px;
}

.cta-button {
    background-color: #7255e8;
    color: #ffffff;
    flex-shrink: 0;
}

.cta-button:hover {
    background-color: #5b40cb;
}

/* =====================================
   7. Footer
===================================== */

.site-footer {
    padding: 24px 0;
    background-color: #20263a;
    color: #ffffff;
}

.footer-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 14px;
}

.footer-content p {
    color: #c5cbd8;
    font-size: 12px;
}

.back-to-top {
    color: #d5ccff;
    font-size: 13px;
}

/* =====================================
   8. Tablet Breakpoint
   600px and above
===================================== */

@media (min-width: 600px) {

    .navbar {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        gap: 18px;
    }

    .hero {
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 28px;
        padding-top: 72px;
        padding-bottom: 76px;
    }

    .hero-stats {
        gap: 16px;
    }

    .features-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .feature-card {
        flex-direction: row;
        gap: 14px;
        padding: 20px;
    }

    .feature-icon {
        width: 42px;
        height: 42px;
    }

    .about-section {
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 30px;
    }

    .cta-content {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    .footer-content {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
    }
}

/* =====================================
   9. Desktop Breakpoint
   1024px and above
===================================== */

@media (min-width: 1024px) {

    .container {
        padding-left: 24px;
        padding-right: 24px;
    }

    .navbar {
        padding-top: 22px;
        padding-bottom: 22px;
    }

    .nav-links {
        gap: 30px;
    }

    .hero {
        gap: 60px;
        padding-top: 96px;
        padding-bottom: 100px;
    }

    .hero-visual > img {
        aspect-ratio: 5 / 4;
    }

    .features-section {
        padding: 88px 0;
    }

    .section-heading {
        margin-bottom: 48px;
    }

    .features-grid {
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 24px;
    }

    .feature-card {
        flex-direction: column;
        align-items: flex-start;
        padding: 28px;
        gap: 20px;
    }

    .feature-icon {
        width: 48px;
        height: 48px;
    }

    .about-section {
        gap: 64px;
        padding-top: 96px;
        padding-bottom: 96px;
    }

    .cta-section {
        padding: 60px 0;
    }
}

/* =====================================
   10. Small Mobile Screen
===================================== */

@media (max-width: 380px) {

    .container {
        padding-left: 12px;
        padding-right: 12px;
    }

    .hero {
        gap: 26px;
        padding-top: 40px;
        padding-bottom: 48px;
    }

    .hero h1 {
        letter-spacing: -1px;
    }

    .hero-actions {
        align-items: stretch;
        flex-direction: column;
    }

    .hero-actions .button {
        width: 100%;
    }

    .hero-stats {
        gap: 14px;
    }

    .hero-stats strong {
        font-size: 18px;
    }

    .feature-card {
        padding: 18px;
    }

    .floating-card {
        margin-left: 6px;
        margin-right: 6px;
    }
}
```

## 6. CSS Grid and Flexbox Explanation

### CSS Grid

CSS Grid is used to arrange content into rows and columns.

In this assignment, Grid is used for:

- The hero section on larger screens.
- The six feature cards.
- The about section containing an image and text.

Example:

```css
.features-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 24px;
}
```

This creates three equal-width columns on desktop screens.

### Flexbox

Flexbox is used to arrange elements along a row or column and align them.

In this assignment, Flexbox is used for:

- The navigation bar.
- Hero section buttons and statistics.
- Internal feature-card content.
- The call-to-action section.
- Footer alignment.

Example:

```css
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 16px;
}
```

This aligns the navigation elements and distributes space between them.

## 7. Responsive Layout

The webpage follows a mobile-first approach. Its default layout uses one column, and media queries introduce additional columns as the screen becomes wider.

| Screen size | Features layout | Hero layout |
|---|---|---|
| Mobile: below 600px | 1 column | 1 column |
| Tablet: 600px and above | 2 columns | 2 columns |
| Desktop: 1024px and above | 3 columns | 2 columns |

The layout also uses flexible spacing, responsive headings, and wrapping navigation links to avoid horizontal overflow.

## 8. Steps to Run the Project

1. Open Visual Studio Code.
2. Create a folder named `Assignment-9.3`.
3. Create `index.html` and `style.css`.
4. Paste the HTML code into `index.html`.
5. Paste the CSS code into `style.css`.
6. Save both files.
7. Install the Live Server extension if necessary.
8. Right-click `index.html`.
9. Select **Open with Live Server**.
10. Check that all sections and images appear correctly.

**Note:** The images use online Unsplash URLs, so an internet connection is required to load them.

## 9. Testing with Chrome DevTools

1. Open the webpage in Google Chrome.
2. Right-click the page and select **Inspect**.
3. Press `Ctrl + Shift + M` to open Device Mode.
4. Test the mobile layout at `375 × 812`.
5. Test the tablet layout at `768 × 1024`.
6. Test the desktop layout at `1440 × 900`.
7. Confirm that the feature cards change from one column to two and then three columns.
8. Check that navigation links do not overlap.
9. Confirm that images remain inside their containers.
10. Check that no unwanted horizontal scrollbar appears.

## 10. Screenshot Submission

Capture screenshots from the actual webpage using Chrome DevTools.

**Mobile screenshot**
- Viewport: `375 × 812`
- Verify the single-column layout.
- Save as `mobile.png`.

**Tablet screenshot**
- Viewport: `768 × 1024`
- Verify the two-column feature layout.
- Save as `tablet.png`.

**Desktop screenshot**
- Viewport: `1440 × 900`
- Verify the three-column feature layout.
- Save as `desktop.png`.

Place the screenshots inside the `screenshots` folder.

## 11. Result

A complete responsive landing page was created using HTML, CSS Grid, and Flexbox. The page contains a header, navigation bar, hero section, six feature cards, an about section, a call-to-action section, and a footer.

The layout adapts to mobile, tablet, and desktop screens using media queries.

## 12. Conclusion

This assignment demonstrates how CSS Grid and Flexbox can work together to build modern, responsive landing pages. Grid organizes the main page sections and card columns, while Flexbox handles navigation, alignment, spacing, and internal content layout. Media queries ensure that the design remains usable across different screen sizes.
```

