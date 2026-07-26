<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kyle Watson | Interactive Narrative Portfolio</title>
    <style>
        :root {
            --bg-color: #0f1117;
            --card-bg: #1a1d26;
            --accent-color: #74c0fc;
            --text-color: #e6e8ee;
            --text-muted: #9aa0a6;
            --border-color: #2e3440;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            padding-bottom: 60px;
        }

        header {
            background-color: rgba(15, 17, 23, 0.95);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border-color);
            backdrop-filter: blur(8px);
        }

        nav {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.2rem 2rem;
        }

        .nav-logo {
            font-weight: bold;
            font-size: 1.2rem;
            color: var(--accent-color);
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        .nav-links a {
            color: var(--text-color);
            text-decoration: none;
            font-size: 0.95rem;
            transition: color 0.2s ease;
        }

        .nav-links a:hover {
            color: var(--accent-color);
        }

        main {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1.5rem;
        }

        section {
            margin-bottom: 4rem;
            scroll-margin-top: 5rem;
        }

        h1, h2, h3 {
            color: #ffffff;
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        .subtitle {
            color: var(--accent-color);
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        h2 {
            font-size: 1.8rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
        }

        p {
            margin-bottom: 1rem;
            color: var(--text-color);
        }

        .card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 1.8rem;
            margin-top: 1rem;
        }

        .reflection-box {
            background-color: rgba(116, 192, 252, 0.05);
            border-left: 4px solid var(--accent-color);
            padding: 1rem;
            margin-top: 1rem;
            border-radius: 0 4px 4px 0;
        }

        .btn {
            display: inline-block;
            background-color: var(--accent-color);
            color: #0f1117;
            padding: 0.6rem 1.2rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 1rem;
            transition: background-color 0.2s ease;
        }

        .btn:hover {
            background-color: #5ca0d3;
        }

        footer {
            text-align: center;
            color: var(--text-muted);
            font-size: 0.85rem;
            margin-top: 4rem;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="nav-logo">Kyle Watson</div>
            <ul class="nav-links">
                <li><a href="#statement">Statement</a></li>
                <li><a href="#twine">Twine Game</a></li>
                <li><a href="#rpg">RPG Handbook</a></li>
                <li><a href="#gdd">Game Design Document</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- HERO TITLE -->
        <section>
            <h1>Interactive Narrative Portfolio</h1>
            <p class="subtitle">CS 3305 &bull; Interactive Narrative Games Design</p>
        </section>

        <!-- PROFESSIONAL STATEMENT -->
        <section id="statement">
            <h2>Professional Statement</h2>
            <div class="card">
                <p>Welcome to my interactive narrative portfolio. As a game designer and developer with a foundation in Computer Science, my goal is to bridge systemic design with rich, choice-driven storytelling. Throughout this course, I have explored how structural rules, player agency, and atmospheric worldbuilding intersect to create engaging player experiences.</p>
                
                <p>My creative focus centers around dark fantasy, investigative mystery, and systemic player choice. I am particularly drawn to mechanics where player decisions aren't merely binary moral dilemmas, but tactical and personal trade-offs—such as managing physical or psychological impulses in high-stakes environments. Drawing inspiration from rich, atmospheric survival narratives and tactical tabletop RPGs, my goal is to craft immersive worlds where players feel both empowered and challenged by the consequences of their actions.</p>

                <p>My technical background allows me to construct logical narrative trees and implement dynamic state tracking (using tools like Twine's Harlowe macros, flags, and variables). Whether scripting mechanical locking systems in a digital text adventure or balancing character attributes for a tabletop RPG handbook section, I approach game design as both an art and a software discipline. Moving forward, I aim to continue developing games that prioritize deep narrative reactivity and memorable worldbuilding.</p>
            </div>
        </section>

        <!-- TWINE INTERACTIVE FICTION -->
        <section id="twine">
            <h2>Twine Interactive Fiction</h2>
            <div class="card">
                <h3>Star Chaser</h3>
                <p><em>Star Chaser</em> is a steampunk, fantasy-investigative interactive text adventure built in Twine. Players take on the role of Elizabeth, a gunslinger traveling alongside a party of unique companions—a Minotaur, a Kobold, and a Tabaxi—on a quest to confront the enigmatic Wishmaker and reclaim their lost "sparks." The game features branching paths, environment inspection, inventory/blueprint mechanics, and an "Impulse" system where player emotional restraint directly dictates the narrative outcome.</p>

                <div class="reflection-box">
                    <p><strong>Reflection &amp; Process:</strong> Developing <em>Star Chaser</em> allowed me to experiment with conditional logic (variables tracking blueprints, keys, and impulse choices) to create a sense of true agency. Balancing atmospheric prose with clear mechanical choices reinforced my goal of designing narratives where the player’s psychological choices dictate both immediate interactions and the ultimate trajectory of the story.</p>
                </div>

                <!-- Link to play your game (e.g. starchaser.html or external link) -->
                <a href="starchaser.html" class="btn" target="_blank">Play Star Chaser</a>
            </div>
        </section>

        <!-- RPG HANDBOOK SECTION -->
        <section id="rpg">
            <h2>RPG Handbook Section</h2>
            <div class="card">
                <h3>Tabletop RPG Module: "The Wishmaker's Spark"</h3>
                <p>This handbook section provides tabletop players and Game Masters with a modular class and environmental ruleset centered around magical "sparks"—the core essence of a character's creative and vital energy. Designed for tabletop campaigns, this document introduces stats for steampunk artificer mechanisms, rules for handling lost sparks, and unique archetype options for fantasy races navigating industrial environments.</p>

                <div class="reflection-box">
                    <p><strong>Reflection &amp; Process:</strong> Designing this RPG ruleset challenged me to translate narrative concepts into clear, balanced game mechanics for a tabletop audience. Writing for both players and Game Masters refined my ability to write concise technical documentation while maintaining evocative thematic flavor.</p>
                </div>

                <a href="#" class="btn">View Handbook PDF</a>
            </div>
        </section>

        <!-- GAME DESIGN DOCUMENT -->
        <section id="gdd">
            <h2>Game Design Document (GDD)</h2>
            <div class="card">
                <h3>Star Chaser: High-Concept Game Design Document</h3>
                <p>This comprehensive Game Design Document outlines the full vision for <em>Star Chaser</em> as an expanded interactive visual novel/RPG hybrid. The document details core gameplay loops, party management systems, emotional impulse mechanics, character biographies, audio/visual mood boards, and complete passage flowcharts for the city of Vanderwall and the Trading Guild sanctum.</p>

                <div class="reflection-box">
                    <p><strong>Reflection &amp; Process:</strong> Authoring this GDD was an essential exercise in production planning and game architecture. It forced me to map out technical scope, player pathways, and mechanical dependencies prior to implementation, bridging my computer science workflow with creative narrative planning.</p>
                </div>

                <a href="#" class="btn">View GDD PDF</a>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Kyle Watson &bull; Portfolio created for Interactive Narrative Games</p>
    </footer>

</body>
</html>
