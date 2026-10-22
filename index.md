Here is the complete solution for Assignment 3.4 — Semantic HTML & Accessibility, featuring the non-semantic <div>-based code ("Before") and the converted semantic code ("After").

Step 1: The Non-Semantic HTML Code ("Before")
Save this non-semantic code as before.html to demonstrate the unorganized structure:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Webpage (Before)</title>
</head>
<body>

    <!-- Header / Navigation -->
    <div id="header">
        <div id="logo">My Tech Blog</div>
        <div id="menu">
            <a href="#">Home</a>
            <a href="#">Articles</a>
            <a href="#">About</a>
        </div>
    </div>

    <!-- Main Content Area -->
    <div id="content">
        <div class="post">
            <div class="post-title">Understanding Semantic HTML</div>
            <img src="https://via.placeholder.com/400x200">
            <div class="post-body">
                Semantic HTML provides meaning to web pages, making them accessible to screen readers and search engines.
            </div>
        </div>

        <!-- Sidebar -->
        <div id="sidebar">
            <div class="sidebar-title">Recent Posts</div>
            <div>- Introduction to CSS</div>
            <div>- JavaScript Basics</div>
        </div>
    </div>

    <!-- Footer -->
    <div id="footer">
        <div>© 2026 My Tech Blog. All rights reserved.</div>
    </div>

</body>
</html>
Step 2: The Semantic HTML Code ("After")
Save this updated code as index.html (or after.html). It replaces structural <div> elements with standard semantic tags (<header>, <nav>, <main>, <article>, <aside>, and <footer>) and adds required accessibility attributes:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Tech Blog - Semantic HTML</title>
</head>
<body>

    <!-- Header containing logo and primary navigation -->
    <header>
        <h1>My Tech Blog</h1>
        <nav aria-label="Primary Navigation">
            <a href="#home">Home</a> | 
            <a href="#articles">Articles</a> | 
            <a href="#about">About</a>
        </nav>
    </header>

    <hr>

    <!-- Main Content Area -->
    <main>
        <!-- Main Article Section -->
        <section id="articles">
            <article>
                <h2>Understanding Semantic HTML</h2>
                <img src="https://via.placeholder.com/400x200" 
                     alt="Illustration showing semantic HTML layout components like header, main, section, and footer" 
                     width="400" 
                     height="200">
                <p>
                    Semantic HTML provides meaning to web pages, making them accessible to screen readers, 
                    improving SEO, and ensuring clean, readable code structure.
                </p>
            </article>
        </section>

        <hr>

        <!-- Sidebar / Secondary Content -->
        <aside>
            <h3>Recent Posts</h3>
            <ul>
                <li><a href="#">Introduction to CSS</a></li>
                <li><a href="#">JavaScript Basics</a></li>
            </ul>
        </aside>
    </main>

    <hr>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2026 My Tech Blog. All rights reserved.</p>
    </footer>

</body>
</html>
Key Requirements Checklist Met:
Semantic Elements: Uses <header>, <nav>, <main>, <section>, <article>, <aside>, and <footer>.

Navigation: Menu links are encapsulated within <nav>.

Main Content Container: Primary page content resides within <main>.

Heading Hierarchy: Clear header structure using <h1>, <h2>, and <h3>.

Accessibility & Alt Text: Added meaningful alt text to images and aria-label to the navigation menu.

Submission Requirements
HTML Files: Submit both your before.html and updated after.html files.

Screenshots: Take a screenshot of the browser DOM structure / page rendering for both files to submit as the "Before and After" comparison.