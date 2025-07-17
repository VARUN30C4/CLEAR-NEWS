
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Global News Hub</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Global News Hub</h1>
        <nav>
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('world')">World</a></li>
                <li><a href="#" onclick="showSection('technology')">Technology</a></li>
                <li><a href="#" onclick="showSection('sports')">Sports</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home" class="news-section active">
            <h2>Latest Headlines</h2>
            <div id="home-news" class="news-container"></div>
        </section>
        <section id="world" class="news-section">
            <h2>World News</h2>
            <div id="world-news" class="news-container"></div>
        </section>
        <section id="technology" class="news-section">
            <h2>Technology News</h2>
            <div id="technology-news" class="news-container"></div>
        </section>
        <section id="sports" class="news-section">
            <h2>Sports News</h2>
            <div id="sports-news" class="news-container"></div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Global News Hub. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
