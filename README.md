<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Annihilator-Jack | Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #8a2be2;
            --secondary: #9370db;
            --dark: #121212;
            --light: #e0e0e0;
            --gradient: linear-gradient(135deg, #8a2be2, #9370db);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--dark);
            color: var(--light);
            min-height: 100vh;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .container {
            max-width: 800px;
            width: 100%;
            background: rgba(20, 20, 30, 0.8);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }

        .container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 100%;
            height: 100%;
            background: var(--gradient);
            transform: rotate(30deg);
            opacity: 0.05;
            z-index: -1;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
            background: var(--gradient);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            position: relative;
            display: inline-block;
        }

        h1::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 5px;
            height: 20px;
            background: var(--gradient);
            border-radius: 0 0 5px 5px;
        }

        .tagline {
            font-size: 1.2rem;
            color: #aaa;
            margin-bottom: 20px;
        }

        .emoji {
            font-size: 2.5rem;
            display: inline-block;
            margin-right: 10px;
            vertical-align: middle;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .section {
            margin-bottom: 30px;
            padding: 20px;
            border-radius: 15px;
            background: rgba(25, 25, 35, 0.6);
            transition: transform 0.3s ease;
            border-left: 5px solid var(--primary);
        }

        .section:hover {
            transform: translateY(-5px);
        }

        h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            color: var(--secondary);
        }

        h2 i {
            margin-right: 10px;
            color: var(--primary);
        }

        .interest-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }

        .interest-item {
            background: rgba(30, 30, 45, 0.6);
            padding: 10px;
            border-radius: 8px;
            text-align: center;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .interest-item:hover {
            background: var(--primary);
            transform: scale(1.05);
        }

        .interest-item i {
            font-size: 2rem;
            margin-bottom: 10px;
            display: block;
            color: var(--secondary);
        }

        .interest-item span {
            display: block;
            font-size: 0.9rem;
        }

        .collaboration {
            background: rgba(30, 30, 45, 0.6);
            padding: 20px;
            border-radius: 15px;
            margin-top: 20px;
            text-align: center;
        }

        .reach-me {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .reach-item {
            display: flex;
            align-items: center;
            background: rgba(30, 30, 45, 0.6);
            padding: 10px 20px;
            border-radius: 50px;
            transition: all 0.3s ease;
        }

        .reach-item:hover {
            background: var(--primary);
            transform: translateY(-5px);
        }

        .reach-item i {
            margin-right: 10px;
            font-size: 1.5rem;
            color: var(--secondary);
        }

        .footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(138, 43, 226, 0.3);
            color: #aaa;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .interest-grid {
                grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            }
            
            .reach-me {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1><span class="emoji"><i class="fas fa-user"></i></span> Annihilator-Jack</h1>
            <p class="tagline">Cybersecurity enthusiast & Python developer</p>
        </header>

        <div class="section">
            <h2><i class="fas fa-robot"></i> My Interests</h2>
            <div class="interest-grid">
                <div class="interest-item">
                    <i class="fas fa-desktop"></i>
                    <span>PC Building</span>
                </div>
                <div class="interest-item">
                    <i class="fab fa-python"></i>
                    <span>Python</span>
                </div>
                <div class="interest-item">
                    <i class="fas fa-shield-alt"></i>
                    <span>Cyber Security</span>
                </div>
                <div class="interest-item">
                    <i class="fas fa-code"></i>
                    <span>Software Engineering</span>
                </div>
            </div>
        </div>

        <div class="section">
            <h2><i class="fas fa-graduation-cap"></i> Currently Learning</h2>
            <p style="font-size: 1.2rem; margin-top: 15px; color: var(--light);">
                <i class="fab fa-python"></i> Python Programming
            </p>
        </div>

        <div class="section">
            <h2><i class="fas fa-hands-helping"></i> Open to Collaboration</h2>
            <p style="font-size: 1.2rem; margin-top: 15px;">
                I'm looking for opportunities to collaborate on security research, Python projects, and open-source contributions.
            </p>
        </div>

        <div class="section collaboration">
            <h2><i class="fas fa-envelope"></i> Reach Me</h2>
            <p style="font-size: 1.2rem; margin-top: 15px;">
                Feel free to reach out if you're interested in collaborating or have any questions.
            </p>
            <div class="reach-me">
                <a href="mailto:contact@annihilatorjack.com" class="reach-item">
                    <i class="fas fa-envelope"></i>
                    <span>Email</span>
                </a>
                <a href="https://github.com/Annihilator-Jack" class="reach-item" target="_blank">
                    <i class="fab fa-github"></i>
                    <span>GitHub</span>
                </a>
                <a href="https://linkedin.com/in/annihilator-jack" class="reach-item" target="_blank">
                    <i class="fab fa-linkedin"></i>
                    <span>LinkedIn</span>
                </a>
            </div>
        </div>

        <div class="footer">
            <p>Made with <i class="fas fa-heart" style="color: var(--secondary);"></i> for the cybersecurity community</p>
        </div>
    </div>

    <script>
        // Add animation to interests
        document.addEventListener('DOMContentLoaded', function() {
            const interestItems = document.querySelectorAll('.interest-item');
            
            interestItems.forEach(item => {
                item.addEventListener('mouseover', function() {
                    this.style.transform = 'scale(1.05)';
                    this.style.boxShadow = '0 0 15px rgba(138, 43, 226, 0.5)';
                });
                
                item.addEventListener('mouseout', function() {
                    this.style.transform = 'scale(1)';
                    this.style.boxShadow = 'none';
                });
            });
        });
    </script>
</body>
</html>
