cat > platremo-readme.html << 'EOF'
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PLATREMO.HUB - Professional Automation Hub</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: #0f1419;
            color: #f5f5f5;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            line-height: 1.6;
            padding: 40px 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
        }
        
        header {
            display: flex;
            align-items: center;
            gap: 30px;
            margin-bottom: 60px;
            border-bottom: 2px solid #1a2332;
            padding-bottom: 40px;
        }
        
        .logo {
            width: 120px;
            height: 120px;
            flex-shrink: 0;
        }
        
        .header-text h1 {
            font-size: 48px;
            font-weight: 700;
            color: #f5f5f5;
            margin-bottom: 10px;
        }
        
        .header-text p {
            font-size: 18px;
            color: #d4a574;
            font-weight: 500;
        }
        
        h2 {
            font-size: 32px;
            color: #f5f5f5;
            margin: 50px 0 30px;
            padding-top: 40px;
            border-top: 1px solid #1a2332;
        }
        
        .section {
            margin-bottom: 50px;
        }
        
        .agent-card {
            background: #1a2332;
            border-left: 4px solid #d4a574;
            padding: 30px;
            margin: 30px 0;
            border-radius: 8px;
        }
        
        .agent-card h3 {
            color: #d4a574;
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .agent-card p {
            color: #e0e0e0;
            margin-bottom: 15px;
            font-size: 16px;
        }
        
        .features {
            list-style: none;
            margin: 15px 0;
        }
        
        .features li {
            padding: 8px 0;
            padding-left: 20px;
            position: relative;
            color: #d4a574;
        }
        
        .features li:before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #9d1f44;
            font-weight: bold;
        }
        
        .results {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .result-item {
            background: #0f1419;
            border: 1px solid #1a2332;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
        }
        
        .result-item .number {
            font-size: 32px;
            font-weight: 700;
            color: #d4a574;
        }
        
        .result-item .label {
            font-size: 14px;
            color: #aaa;
            margin-top: 10px;
        }
        
        .workflow {
            background: #1a2332;
            padding: 30px;
            border-radius: 8px;
            margin: 30px 0;
            text-align: center;
            font-size: 18px;
            font-weight: 600;
            color: #d4a574;
            letter-spacing: 2px;
        }
        
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .pricing-card {
            background: #1a2332;
            border: 2px solid #1a2332;
            padding: 40px;
            border-radius: 8px;
            transition: all 0.3s ease;
        }
        
        .pricing-card:hover {
            border-color: #d4a574;
            transform: translateY(-5px);
        }
        
        .pricing-card h3 {
            color: #d4a574;
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .price {
            font-size: 42px;
            font-weight: 700;
            color: #9d1f44;
            margin: 20px 0;
        }
        
        .pricing-card ul {
            list-style: none;
            margin: 20px 0;
        }
        
        .pricing-card li {
            padding: 10px 0;
            border-bottom: 1px solid #0f1419;
            color: #d4a574;
        }
        
        .cta-button {
            background: #d4a574;
            color: #0f1419;
            border: none;
            padding: 15px 40px;
            font-size: 16px;
            font-weight: 700;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 20px;
            width: 100%;
        }
        
        .cta-button:hover {
            background: #a67c52;
            transform: translateY(-2px);
        }
        
        .cta-button.secondary {
            background: transparent;
            border: 2px solid #9d1f44;
            color: #9d1f44;
        }
        
        .cta-button.secondary:hover {
            background: #9d1f44;
            color: #f5f5f5;
        }
        
        footer {
            margin-top: 80px;
            padding-top: 40px;
            border-top: 2px solid #1a2332;
            text-align: center;
            color: #aaa;
        }
        
        .founder-bio {
            background: #1a2332;
            padding: 30px;
            border-left: 4px solid #9d1f44;
            border-radius: 8px;
            margin: 40px 0;
        }
        
        .founder-bio h3 {
            color: #9d1f44;
            margin-bottom: 15px;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- HEADER WITH LOGO -->
        <header>
            <svg class="logo" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <!-- Background circle -->
                <circle cx="100" cy="100" r="95" fill="none" stroke="#1a2332" stroke-width="2"/>
                
                <!-- P Letter -->
                <g transform="translate(50, 40)">
                    <!-- Vertical line of P -->
                    <line x1="20" y1="20" x2="20" y2="100" stroke="#d4a574" stroke-width="8" stroke-linecap="round"/>
                    <!-- Curved top of P -->
                    <path d="M 20 20 Q 60 20 60 50 Q 60 80 20 80" stroke="#d4a574" stroke-width="8" stroke-linecap="round" fill="none"/>
                </g>
                
                <!-- Hub circle in center-bottom -->
                <circle cx="100" cy="130" r="15" fill="#9d1f44"/>
                <circle cx="100" cy="130" r="8" fill="none" stroke="#d4a574" stroke-width="2"/>
                
                <!-- Connecting lines (flow) -->
                <line x1="70" y1="100" x2="85" y2="125" stroke="#d4a574" stroke-width="2" opacity="0.6"/>
                <line x1="130" y1="100" x2="115" y2="125" stroke="#d4a574" stroke-width="2" opacity="0.6"/>
            </svg>
            
            <div class="header-text">
                <h1>PLATREMO.HUB</h1>
                <p>Professional Automation Management Hub</p>
                <p style="font-size: 14px; color: #aaa; margin-top: 10px;">By Adrian Povestca</p>
            </div>
        </header>
        
        <!-- INTRODUCTION -->
        <section class="section">
            <h2>What is PLATREMO?</h2>
            <p>PLATREMO automates your customer communication through intelligent AI agents. We help businesses respond to customers faster, smarter, and in any language.</p>
            <p style="margin-top: 15px; color: #d4a574; font-weight: 500;">Mission: Transform customer communication through intelligent automation.</p>
        </section>
        
        <!-- AGENTS -->
        <section class="section">
            <h2>Our Agents</h2>
            
            <div class="agent-card">
                <h3>MIRI - Customer Support AI</h3>
                <p>Understands customer intent. Routes urgent issues. Provides instant responses.</p>
                
                <p style="font-weight: 600; margin-top: 20px;">Features:</p>
                <ul class="features">
                    <li>Intent detection (support, sales, billing, complaints)</li>
                    <li>Urgency assessment (low/medium/high)</li>
                    <li>Smart routing to right team</li>
                    <li>Multi-language support</li>
                    <li>24/7 availability</li>
                </ul>
                
                <p style="font-weight: 600; margin-top: 20px; color: #9d1f44;">Results:</p>
                <div class="results">
                    <div class="result-item">
                        <div class="number">80%</div>
                        <div class="label">Faster Response</div>
                    </div>
                    <div class="result-item">
                        <div class="number">90%</div>
                        <div class="label">Customer Satisfaction</div>
                    </div>
                    <div class="result-item">
                        <div class="number">40+h</div>
                        <div class="label">Saved Per Week</div>
                    </div>
                </div>
            </div>
            
            <div class="agent-card">
                <h3>M.ARI - Email Automation</h3>
                <p>Reads your emails. Categorizes automatically. Sends contextual replies.</p>
                
                <p style="font-weight: 600; margin-top: 20px;">Features:</p>
                <ul class="features">
                    <li>Email categorization (5 types)</li>
                    <li>Language detection (EN/RO/DE/RU)</li>
                    <li>Urgency detection (smart routing)</li>
                    <li>Context-aware replies</li>
                    <li>Human review for complex cases</li>
                    <li>Full audit trail</li>
                </ul>
                
                <p style="font-weight: 600; margin-top: 20px; color: #9d1f44;">Results:</p>
                <div class="results">
                    <div class="result-item">
                        <div class="number">2m</div>
                        <div class="label">Email Response</div>
                    </div>
                    <div class="result-item">
                        <div class="number">95%</div>
                        <div class="label">Accuracy</div>
                    </div>
                    <div class="result-item">
                        <div class="number">0</div>
                        <div class="label">Training Needed</div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- HOW IT WORKS -->
        <section class="section">
            <h2>How It Works</h2>
            <div class="workflow">
                Gmail → Fetch → Analyze → Decide → Generate → Send → Track
            </div>
            <p>6-step workflow that processes customer communication in minutes, not hours. Everything is logged and trackable.</p>
        </section>
        
        <!-- PRICING -->
        <section class="section">
            <h2>Pricing</h2>
            
            <div class="pricing-grid">
                <div class="pricing-card">
                    <h3>STARTER</h3>
                    <div class="price">$99<span style="font-size: 18px;">/month</span></div>
                    <ul>
                        <li>✓ MIRI only</li>
                        <li>✓ Up to 100 emails/week</li>
                        <li>✓ 24h support</li>
                        <li>✓ Email support</li>
                    </ul>
                    <button class="cta-button">Start Free Trial</button>
                </div>
                
                <div class="pricing-card">
                    <h3>PRO</h3>
                    <div class="price">$199<span style="font-size: 18px;">/month</span></div>
                    <ul>
                        <li>✓ MIRI + M.ARI</li>
                        <li>✓ Up to 500 emails/week</li>
                        <li>✓ Multi-language (EN/RO/DE/RU)</li>
                        <li>✓ Priority support</li>
                    </ul>
                    <button class="cta-button">Start Free Trial</button>
                </div>
                
                <div class="pricing-card">
                    <h3>ENTERPRISE</h3>
                    <div class="price">Custom</div>
                    <ul>
                        <li>✓ Unlimited everything</li>
                        <li>✓ Custom integrations</li>
                        <li>✓ Dedicated support</li>
                        <li>✓ SLA guarantee</li>
                    </ul>
                    <button class="cta-button secondary">Contact Sales</button>
                </div>
            </div>
        </section>
        
        <!-- FOUNDER -->
        <section class="section">
            <div class="founder-bio">
                <h3>About the Founder</h3>
                <p><strong>Adrian Povestca</strong> is building the future of customer automation. PLATREMO.HUB brings together 20+ years of combined experience in AI, customer support, and automation.</p>
                <p style="margin-top: 15px;">Part of the CompanyMind ecosystem, alongside MIRI Customer Support AI.</p>
            </div>
        </section>
        
        <!-- CTA -->
        <section class="section" style="text-align: center; margin: 80px 0;">
            <h2>Ready to Automate?</h2>
            <p style="font-size: 18px; margin: 20px 0;">Join forward-thinking companies automating customer communication.</p>
            <button class="cta-button" style="max-width: 300px; margin: 30px auto;">Book a Demo</button>
        </section>
        
        <!-- FOOTER -->
        <footer>
            <p>PLATREMO.HUB © 2026 by Adrian Povestca</p>
            <p style="margin-top: 10px; font-size: 12px;">Professional Automation • Intelligent Responses • Global Language Support</p>
        </footer>
    </div>
</body>
</html>
EOF
