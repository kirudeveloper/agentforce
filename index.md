<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
    <title>AgentForce - Intelligent AI Agents</title>
    <meta http-equiv="Content-Security-Policy" content="upgrade-insecure-requests">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #3b82f6;
            --secondary-color: #1d4ed8;
            --background-color: #0f172a;
            --text-color: #e2e8f0;
            --card-background: #1e293b;
            --card-hover: #334155;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Space Grotesk', system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--background-color);
            letter-spacing: -0.02em;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 80px 0;
            text-align: center;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
            margin-bottom: 60px;
        }

        header h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            animation: fadeInUp 1s ease;
        }

        header p {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
            animation: fadeInUp 1s ease 0.2s;
        }

        .section {
            margin-bottom: 80px;
            animation: fadeIn 1s ease;
        }

        h2 {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 30px;
            text-align: center;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .feature-card {
            background: var(--card-background);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease, background-color 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.3);
            background-color: var(--card-hover);
        }

        .feature-card i {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 20px;
        }

        .feature-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--text-color);
        }

        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .benefit-item {
            background: var(--card-background);
            padding: 25px;
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            transition: transform 0.3s ease, background-color 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .benefit-item:hover {
            transform: translateY(-3px);
            background-color: var(--card-hover);
        }

        .benefit-item i {
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .steps-container {
            max-width: 800px;
            margin: 40px auto;
        }

        .step-item {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
            padding: 20px;
            background: var(--card-background);
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .step-number {
            width: 40px;
            height: 40px;
            background: var(--primary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 20px;
        }

        .cta-section {
            text-align: center;
            padding: 60px 0;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            border-radius: 15px;
            margin: 40px 0;
        }

        .cta-button {
            display: inline-block;
            padding: 15px 40px;
            background: white;
            color: var(--primary-color);
            text-decoration: none;
            border-radius: 30px;
            font-weight: 600;
            margin-top: 20px;
            transition: transform 0.3s ease;
        }

        .cta-button:hover {
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 40px 0;
            background: var(--text-color);
            color: white;
            margin-top: 80px;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }
            .feature-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Welcome to AgentForce for Salesforce</h1>
            <p>24/7 Self-Service Appointment Booking Powered by AI</p>
        </div>
    </header>

    <div class="container">
        <div class="section">
            <h2>What is AgentForce?</h2>
            <p>AgentForce is a revolutionary AI-powered scheduling assistant that operates 24/7, enabling patients to book, reschedule, or cancel appointments at their convenience without any human intervention. Seamlessly integrated with Salesforce, it provides a hassle-free booking experience while maintaining efficient practice management.</p>
        </div>

        <div class="section">
            <h2>Key Features</h2>
            <div class="feature-grid">
                <div class="feature-card">
                    <i class="fas fa-clock"></i>
                    <h3>24/7 Availability</h3>
                    <p>Book, reschedule, or cancel appointments any time, day or night, without waiting for office hours.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-robot"></i>
                    <h3>AI-Powered Booking</h3>
                    <p>Smart AI assistant handles complex scheduling logic and patient preferences automatically.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-calendar-check"></i>
                    <h3>Instant Confirmation</h3>
                    <p>Receive immediate appointment confirmations and digital calendar invites.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-sync"></i>
                    <h3>Easy Rescheduling</h3>
                    <p>Self-service rescheduling with smart conflict resolution and waitlist management.</p>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>How It Works</h2>
            <div class="steps-container">
                <div class="step-item">
                    <div class="step-number">1</div>
                    <div>Patients access the booking portal 24/7</div>
                </div>
                <div class="step-item">
                    <div class="step-number">2</div>
                    <div>AI analyzes availability and patient preferences</div>
                </div>
                <div class="step-item">
                    <div class="step-number">3</div>
                    <div>Instant booking confirmation and reminders</div>
                </div>
                <div class="step-item">
                    <div class="step-number">4</div>
                    <div>Easy self-service rescheduling if needed</div>
                </div>
                <div class="step-item">
                    <div class="step-number">5</div>
                    <div>Automated follow-ups and feedback collection</div>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>Benefits</h2>
            <div class="benefits-grid">
                <div class="benefit-item">
                    <i class="fas fa-user-clock"></i>
                    <h3>24/7 Access</h3>
                    <p>Book anytime, anywhere</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-tasks"></i>
                    <h3>Full Control</h3>
                    <p>Manage appointments independently</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-check-circle"></i>
                    <h3>Zero Wait Time</h3>
                    <p>Instant booking process</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-calendar-alt"></i>
                    <h3>Flexible Scheduling</h3>
                    <p>Easy rescheduling options</p>
                </div>
            </div>
        </div>

        <div class="cta-section">
            <h2 style="color: white;">Experience 24/7 Self-Service Appointment Booking</h2>
            <p>Transform your practice with automated scheduling that never sleeps</p>
            <a href="#" class="cta-button">Get Started Now</a>
        </div>
    </div>

    <footer>
        <div class="container">
            <p>© 2025 AgentForce - Empowering 24/7 Self-Service Healthcare Scheduling</p>
        </div>
    </footer>
  <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DHr00000Df2UV',
				'GithubKiru',
				'https://ecloudsagentforce.my.site.com/ESWGithubKiru1745723634825',
				{
					scrt2URL: 'https://ecloudsagentforce.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://ecloudsagentforce.my.site.com/ESWGithubKiru1745723634825/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

</body>
  
</html>
