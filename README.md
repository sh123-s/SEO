# SEO
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Marketing Suite - AI, SEO & Web Performance Tools</title>
    <meta name="description" content="Comprehensive digital marketing toolkit featuring AI content tools, website performance optimizers, and professional SEO solutions. Enhance your online presence with our all-in-one marketing suite.">
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --background-color: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--background-color);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 2rem;
            text-align: center;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        .search-section {
            margin: 2rem 0;
            text-align: center;
        }

        .search-input {
            width: 100%;
            max-width: 600px;
            padding: 1rem;
            border: 2px solid #ddd;
            border-radius: 50px;
            font-size: 1.1rem;
        }

        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .tool-card {
            background: white;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .tool-card:hover {
            transform: translateY(-5px);
        }

        .tool-card h3 {
            color: var(--primary-color);
            margin-bottom: 1rem;
        }

        .tool-card p {
            color: #666;
            margin-bottom: 1.5rem;
        }

        .tool-button {
            background-color: var(--secondary-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .tool-button:hover {
            background-color: #2980b9;
        }

        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }
            
            header {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Digital Marketing Suite Pro</h1>
        <p>All-in-One Solution for Content, SEO & Web Performance</p>
    </header>

    <div class="container">
        <div class="search-section">
            <input type="text" class="search-input" placeholder="Search tools...">
        </div>

        <!-- AI & Content Tools Section -->
        <section class="tool-section">
            <h2>AI & Content Tools</h2>
            <div class="tools-grid">
                <div class="tool-card">
                    <h3>AI Content Generator</h3>
                    <p>Generate high-quality content using advanced GPT-4 technology</p>
                    <textarea placeholder="Enter your prompt..." rows="3"></textarea>
                    <button class="tool-button">Generate Content</button>
                </div>
                <!-- Add more AI tools here -->
            </div>
        </section>

        <!-- Website & Performance Tools Section -->
        <section class="tool-section">
            <h2>Website Performance Tools</h2>
            <div class="tools-grid">
                <div class="tool-card">
                    <h3>Website Speed Analyzer</h3>
                    <p>Test your website loading speed and get optimization suggestions</p>
                    <input type="url" placeholder="Enter website URL">
                    <button class="tool-button">Analyze Now</button>
                </div>
                <!-- Add more performance tools here -->
            </div>
        </section>

        <!-- SEO & Digital Marketing Tools Section -->
        <section class="tool-section">
            <h2>SEO & Marketing Tools</h2>
            <div class="tools-grid">
                <div class="tool-card">
                    <h3>Keyword Research Tool</h3>
                    <p>Find high-ranking keywords for your SEO strategy</p>
                    <input type="text" placeholder="Enter seed keyword">
                    <button class="tool-button">Find Keywords</button>
                </div>
                <!-- Add more SEO tools here -->
            </div>
        </section>
    </div>

    <script>
        // Search functionality
        const searchInput = document.querySelector('.search-input');
        searchInput.addEventListener('input', filterTools);

        function filterTools() {
            const searchTerm = searchInput.value.toLowerCase();
            document.querySelectorAll('.tool-card').forEach(card => {
                const text = card.textContent.toLowerCase();
                card.style.display = text.includes(searchTerm) ? 'block' : 'none';
            });
        }

        // Tool interaction examples
        document.querySelectorAll('.tool-button').forEach(button => {
            button.addEventListener('click', function() {
                const toolName = this.parentElement.querySelector('h3').textContent;
                alert(`Processing ${toolName} request...`);
                // Add actual API calls or functionality here
            });
        });
    </script>
</body>
</html>
