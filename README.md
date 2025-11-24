<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Compétences - Firas Ben Slimen</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #0f172a, #1e293b);
            color: #e2e8f0;
            min-height: 100vh;
            padding: 2rem;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .header {
            text-align: center;
            margin-bottom: 3rem;
        }

        .header h1 {
            font-size: 2.5rem;
            background: linear-gradient(45deg, #3b82f6, #8b5cf6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 0.5rem;
        }

        .header p {
            font-size: 1.1rem;
            color: #94a3b8;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 1rem;
            flex-wrap: wrap;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.5rem 1rem;
            background: rgba(30, 41, 59, 0.8);
            border-radius: 8px;
            transition: transform 0.3s ease;
        }

        .contact-item:hover {
            transform: translateY(-2px);
        }

        .contact-item a {
            color: #60a5fa;
            text-decoration: none;
        }

        .dashboard {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-bottom: 3rem;
        }

        @media (max-width: 768px) {
            .dashboard {
                grid-template-columns: 1fr;
            }
        }

        .card {
            background: rgba(30, 41, 59, 0.8);
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
        }

        .card h2 {
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            color: #3b82f6;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .skill-category {
            margin-bottom: 1.5rem;
        }

        .skill-category h3 {
            font-size: 1.1rem;
            margin-bottom: 1rem;
            color: #cbd5e1;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .skill-item {
            margin-bottom: 1rem;
        }

        .skill-info {
            display: flex;
            justify-content: between;
            margin-bottom: 0.5rem;
        }

        .skill-name {
            font-weight: 500;
        }

        .skill-level {
            color: #94a3b8;
            font-size: 0.9rem;
        }

        .progress-bar {
            height: 8px;
            background: rgba(100, 116, 139, 0.3);
            border-radius: 4px;
            overflow: hidden;
        }

        .progress {
            height: 100%;
            border-radius: 4px;
            transition: width 1s ease-in-out;
        }

        .level-advanced { background: linear-gradient(45deg, #10b981, #34d399); }
        .level-intermediate { background: linear-gradient(45deg, #3b82f6, #60a5fa); }
        .level-beginner { background: linear-gradient(45deg, #f59e0b, #fbbf24); }
        .level-learning { background: linear-gradient(45deg, #8b5cf6, #a78bfa); }

        .learning-section {
            background: linear-gradient(135deg, rgba(139, 92, 246, 0.1), rgba(59, 130, 246, 0.1));
            border: 1px solid rgba(139, 92, 246, 0.3);
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
        }

        .tech-item {
            background: rgba(15, 23, 42, 0.6);
            padding: 1rem;
            border-radius: 8px;
            text-align: center;
            transition: all 0.3s ease;
        }

        .tech-item:hover {
            background: rgba(30, 41, 59, 0.9);
            transform: scale(1.05);
        }

        .tech-icon {
            font-size: 2rem;
            margin-bottom: 0.5rem;
        }

        .tech-name {
            font-weight: 600;
            margin-bottom: 0.25rem;
        }

        .tech-status {
            font-size: 0.8rem;
            color: #94a3b8;
        }

        .nextjs { color: #000000; }
        .vuejs { color: #41b883; }
        .react-native { color: #61dafb; }
        .typescript { color: #3178c6; }

        .footer {
            text-align: center;
            margin-top: 3rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #94a3b8;
        }

        .highlight {
            color: #60a5fa;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>📊 Dashboard des Compétences</h1>
            <p>Firas Ben Slimen - Développeur Full-Stack</p>
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fab fa-linkedin"></i>
                    <a href="https://www.linkedin.com/in/firasbs25/" target="_blank">LinkedIn</a>
                </div>
                <div class="contact-item">
                    <i class="fab fa-github"></i>
                    <a href="https://github.com/Firasbs23" target="_blank">GitHub</a>
                </div>
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <span>+216 92 577 246</span>
                </div>
            </div>
        </div>

        <div class="dashboard">
            <!-- Compétences Actuelles -->
            <div class="card">
                <h2><i class="fas fa-star"></i> Compétences Maîtrisées</h2>
                
                <div class="skill-category">
                    <h3><i class="fab fa-js"></i> Frontend</h3>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">React.js</span>
                            <span class="skill-level">Avancé</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-advanced" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">JavaScript (ES6+)</span>
                            <span class="skill-level">Avancé</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-advanced" style="width: 85%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">HTML5 & CSS3</span>
                            <span class="skill-level">Avancé</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-advanced" style="width: 88%"></div>
                        </div>
                    </div>
                </div>

                <div class="skill-category">
                    <h3><i class="fas fa-server"></i> Backend</h3>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">Node.js</span>
                            <span class="skill-level">Intermédiaire</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-intermediate" style="width: 75%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">Express.js</span>
                            <span class="skill-level">Intermédiaire</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-intermediate" style="width: 70%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">MongoDB</span>
                            <span class="skill-level">Intermédiaire</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-intermediate" style="width: 65%"></div>
                        </div>
                    </div>
                </div>

                <div class="skill-category">
                    <h3><i class="fas fa-tools"></i> Outils & Autres</h3>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">Git & GitHub</span>
                            <span class="skill-level">Intermédiaire</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-intermediate" style="width: 80%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-info">
                            <span class="skill-name">MySQL</span>
                            <span class="skill-level">Débutant</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress level-beginner" style="width: 60%"></div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Technologies en Cours d'Apprentissage -->
            <div class="card learning-section">
                <h2><i class="fas fa-rocket"></i> En Cours d'Apprentissage</h2>
                <p style="margin-bottom: 1.5rem; color: #cbd5e1;">
                    Technologies modernes que je maîtrise actuellement pour devenir un développeur full-stack plus complet.
                </p>

                <div class="tech-grid">
                    <div class="tech-item">
                        <div class="tech-icon nextjs">
                            <i class="fab fa-react"></i>
                        </div>
                        <div class="tech-name">Next.js</div>
                        <div class="tech-status">En apprentissage</div>
                        <div class="progress-bar" style="margin-top: 0.5rem;">
                            <div class="progress level-learning" style="width: 40%"></div>
                        </div>
                        <p style="font-size: 0.8rem; margin-top: 0.5rem; color: #94a3b8;">
                            Framework React full-stack
                        </p>
                    </div>

                    <div class="tech-item">
                        <div class="tech-icon vuejs">
                            <i class="fab fa-vuejs"></i>
                        </div>
                        <div class="tech-name">Vue.js</div>
                        <div class="tech-status">Débutant</div>
                        <div class="progress-bar" style="margin-top: 0.5rem;">
                            <div class="progress level-learning" style="width: 25%"></div>
                        </div>
                        <p style="font-size: 0.8rem; margin-top: 0.5rem; color: #94a3b8;">
                            Framework JavaScript progressif
                        </p>
                    </div>

                    <div class="tech-item">
                        <div class="tech-icon react-native">
                            <i class="fab fa-react"></i>
                        </div>
                        <div class="tech-name">React Native</div>
                        <div class="tech-status">En exploration</div>
                        <div class="progress-bar" style="margin-top: 0.5rem;">
                            <div class="progress level-learning" style="width: 30%"></div>
                        </div>
                        <p style="font-size: 0.8rem; margin-top: 0.5rem; color: #94a3b8;">
                            Développement mobile cross-platform
                        </p>
                    </div>

                    <div class="tech-item">
                        <div class="tech-icon typescript">
                            <i class="fab fa-js-square"></i>
                        </div>
                        <div class="tech-name">TypeScript</div>
                        <div class="tech-status">En progression</div>
                        <div class="progress-bar" style="margin-top: 0.5rem;">
                            <div class="progress level-learning" style="width: 50%"></div>
                        </div>
                        <p style="font-size: 0.8rem; margin-top: 0.5rem; color: #94a3b8;">
                            JavaScript typé pour des applications plus robustes
                        </p>
                    </div>
                </div>

                <div style="margin-top: 1.5rem; padding: 1rem; background: rgba(15, 23, 42, 0.6); border-radius: 8px;">
                    <h4 style="color: #60a5fa; margin-bottom: 0.5rem;">
                        <i class="fas fa-bullseye"></i> Objectifs d'Apprentissage
                    </h4>
                    <ul style="color: #cbd5e1; font-size: 0.9rem; padding-left: 1.2rem;">
                        <li>Maîtriser Next.js pour le développement full-stack</li>
                        <li>Découvrir Vue.js comme alternative à React</li>
                        <li>Développer des applications mobiles avec React Native</li>
                        <li>Adopter TypeScript pour un code plus maintenable</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="footer">
            <p>🚀 <span class="highlight">En constante évolution</span> - Toujours à la recherche de nouveaux défis et opportunités d'apprentissage</p>
            <p style="margin-top: 0.5rem; font-size: 0.9rem;">
                "La seule limite à notre réalisation de demain sera nos doutes d'aujourd'hui." - Franklin D. Roosevelt
            </p>
        </div>
    </div>

    <script>
        // Animation des barres de progression
        document.addEventListener('DOMContentLoaded', function() {
            const progressBars = document.querySelectorAll('.progress');
            progressBars.forEach(bar => {
                const width = bar.style.width;
                bar.style.width = '0';
                setTimeout(() => {
                    bar.style.width = width;
                }, 100);
            });
        });
    </script>
</body>
</html>
