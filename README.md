# ESTUDOPC
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>The Weeknd Music</title>
</head>
<body>

    <header>
        <h1>The Weeknd Music</h1>
    </header>

    <main>
        <h2>Latest Releases</h2>
        <div id="music-list"></div>
    </main>

    <footer>
        &copy; 2023 The Weeknd Music. All rights reserved.
    </footer>

    <script src="app.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
}

main {
    padding: 2em;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
    position: fixed;
    bottom: 0;
    width: 100%;
}
document.addEventListener("DOMContentLoaded", function() {
    const musicList = document.getElementById("music-list");

    // Example data (replace with actual data)
    const releases = [
        { title: "Blinding Lights", album: "After Hours", year: 2020 },
        { title: "Save Your Tears", album: "After Hours", year: 2020 },
        // Add more songs as needed
    ];

    // Render music list
    releases.forEach(release => {
        const releaseDiv = document.createElement("div");
        releaseDiv.innerHTML = `<strong>${release.title}</strong> - ${release.album} (${release.year})<br>`;
        musicList.appendChild(releaseDiv);
    });
});
