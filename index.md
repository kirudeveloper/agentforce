<!DOCTYPE html>
<html lang="en">
	<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
    <title>AgentForce - Intelligent AI Agents</title>
    <meta http-equiv="Content-Security-Policy" content="upgrade-insecure-requests">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #2563eb;
            --secondary-color: #1e40af;
            --background-color: #f8fafc;
            --text-color: #1e293b;
            --card-background: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--background-color);
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
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
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
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }

        .benefit-item:hover {
            transform: translateY(-3px);
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
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
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
            <p>Streamline Your Appointment Booking Process with Intelligent AI Assistance</p>
        </div>
    </header>

    <div class="container">
        <div class="section">
            <h2>What is AgentForce?</h2>
            <p>AgentForce is an intelligent AI-powered scheduling assistant that seamlessly integrates with Salesforce to revolutionize your appointment booking process. It combines advanced AI capabilities with Salesforce's robust platform to provide efficient and automated scheduling solutions.</p>
        </div>

        <div class="section">
            <h2>Key Features</h2>
            <div class="feature-grid">
                <div class="feature-card">
                    <i class="fas fa-calendar-check"></i>
                    <h3>Smart Scheduling</h3>
                    <p>Automatically finds optimal appointment slots based on staff availability and customer preferences.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-sync"></i>
                    <h3>Real-time Sync</h3>
                    <p>Seamlessly synchronizes with your Salesforce calendar and customer database in real-time.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-robot"></i>
                    <h3>AI-Powered Assistant</h3>
                    <p>Intelligent booking assistant that handles scheduling conflicts and manages appointment changes.</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-bell"></i>
                    <h3>Smart Notifications</h3>
                    <p>Automated reminders and confirmations to reduce no-shows and improve attendance rates.</p>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>How It Works</h2>
            <div class="steps-container">
                <div class="step-item">
                    <div class="step-number">1</div>
                    <div>Connect AgentForce with your Salesforce instance</div>
                </div>
                <div class="step-item">
                    <div class="step-number">2</div>
                    <div>Set up your team's availability and booking rules</div>
                </div>
                <div class="step-item">
                    <div class="step-number">3</div>
                    <div>Let AI handle appointment scheduling and management</div>
                </div>
                <div class="step-item">
                    <div class="step-number">4</div>
                    <div>Automated notifications keep everyone informed</div>
                </div>
                <div class="step-item">
                    <div class="step-number">5</div>
                    <div>Track and analyze booking patterns for optimization</div>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>Benefits</h2>
            <div class="benefits-grid">
                <div class="benefit-item">
                    <i class="fas fa-clock"></i>
                    <h3>Save Time</h3>
                    <p>Reduce manual scheduling effort</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-chart-line"></i>
                    <h3>Increase Efficiency</h3>
                    <p>Optimize appointment scheduling</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-smile"></i>
                    <h3>Happy Customers</h3>
                    <p>Improve booking experience</p>
                </div>
                <div class="benefit-item">
                    <i class="fas fa-analytics"></i>
                    <h3>Better Insights</h3>
                    <p>Track booking analytics</p>
                </div>
            </div>
        </div>

        <div class="cta-section">
            <h2 style="color: white;">Ready to Transform Your Appointment Booking Process?</h2>
            <p>Get started with AgentForce for Salesforce today and experience the future of intelligent scheduling.</p>
            <a href="#" class="cta-button">Schedule a Demo</a>
        </div>
    </div>

    <footer>
        <div class="container">
            <p>© 2025 AgentForce - Your Intelligent Scheduling Partner for Salesforce</p>
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
