# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Layout with Flexbox and Grid</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }
        
        /* Navigation Bar */
        nav {
            background-color: #333;
            color: #fff;
            display: flex;
            justify-content: space-between;
            padding: 1rem;
        }
        
        nav ul {
            list-style: none;
            display: flex;
            margin: 0;
            padding: 0;
        }
        
        nav ul li {
            margin: 0 1rem;
        }
        
        nav ul li a {
            color: #fff;
            text-decoration: none;
        }
        
        /* Main Content Layout */
        .container {
            display: grid;
            grid-template-columns: 1fr 3fr;
            gap: 1rem;
            padding: 1rem;
        }
        
        .sidebar {
            background-color: #f4f4f4;
            padding: 1rem;
        }
        
        .content {
            background-color: #fff;
            padding: 1rem;
            border: 1px solid #ddd;
        }
        
        /* Media Queries */
        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            nav {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 0.5rem 0;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <div class="logo">Logo</div>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Content Layout -->
    <div class="container">
        <aside class="sidebar">
            <h2>Sidebar</h2>
            <p>This is the sidebar content.</p>
        </aside>
        
        <section class="content">
            <h1>Main Content</h1>
            <p>This is the main content area.</p>
        </section>
    </div>

</body>
</html>

This setup ensures that the webpage is responsive and adapts to different screen sizes, providing a good user experience across mobile, tablet, and desktop devices.
