<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quoradux - Bio-Cognitive Programming Revolution</title>
    <meta name="description" content="Revolutionary bio-cognitive programming where thought becomes code. The future of human-computer interface is here.">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Courier New', monospace;
            line-height: 1.6;
            color: #fff;
            background: radial-gradient(ellipse at center, #0a0a1a 0%, #000 100%);
            overflow-x: hidden;
            cursor: none;
        }

        .neural-cursor {
            position: absolute;
            width: 20px;
            height: 20px;
            background: radial-gradient(circle, #00ffff 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
            z-index: 10000;
            mix-blend-mode: screen;
        }

        .consciousness-field {
            position: fixed;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at var(--x, 50%) var(--y, 50%), 
                    rgba(0, 255, 255, 0.1) 0%, 
                    rgba(255, 0, 255, 0.05) 40%, 
                    transparent 70%);
            transition: all 0.3s ease;
            pointer-events: none;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background: rgba(0, 0, 0, 0.95);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(0, 255, 255, 0.3);
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            background: linear-gradient(45deg, #00ffff, #ff00ff, #ffff00, #00ff00);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: consciousness-flow 4s ease-in-out infinite;
        }

        @keyframes consciousness-flow {
            0%, 100% { background-position: 0% 50%; }
            25% { background-position: 100% 50%; }
            50% { background-position: 100% 100%; }
            75% { background-position: 0% 100%; }
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
            font-size: 14px;
        }

        .nav-links a:hover {
            color: #00ffff;
            text-shadow: 0 0 10px #00ffff;
        }

        .cta-button {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            padding: 12px 24px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
            text-decoration: none;
            transition: all 0.3s;
            display: inline-block;
            animation: neural-pulse 2s ease-in-out infinite;
        }

        @keyframes neural-pulse {
            0%, 100% { box-shadow: 0 0 10px rgba(255, 107, 107, 0.5); }
            50% { box-shadow: 0 0 25px rgba(78, 205, 196, 0.8); }
        }

        .cta-button:hover {
            transform: scale(1.05);
        }

        /* Hero Section */
        .hero {
            background: transparent;
            color: white;
            padding: 140px 0 100px;
            text-align: center;
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
        }

        .hero-content h1 {
            font-size: 4rem;
            margin-bottom: 2rem;
            background: linear-gradient(45deg, #00ffff, #ff00ff, #ffff00, #00ff00);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: consciousness-flow 4s ease-in-out infinite;
        }

        .hero-content .tagline {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: #00ffff;
            opacity: 0.9;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.8;
        }

        .bio-cognitive-highlight {
            background: rgba(0, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            margin: 2rem 0;
            border: 2px solid rgba(0, 255, 255, 0.3);
            backdrop-filter: blur(10px);
        }

        .paradigm-text {
            font-size: 1.1rem;
            color: #00ffff;
            margin-bottom: 1rem;
        }

        .code-example {
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            font-size: 14px;
            margin: 20px 0;
            border-left: 4px solid #00ffff;
        }

        .code-line {
            margin: 5px 0;
            color: #00ff00;
        }

        .code-construct { color: #ff6b6b; }
        .code-engine { color: #4ecdc4; }
        .code-return { color: #a8e6cf; }

        .price-highlight {
            background: rgba(255, 107, 107, 0.2);
            padding: 25px;
            border-radius: 15px;
            margin: 2rem 0;
            border: 2px solid #ff6b6b;
            backdrop-filter: blur(10px);
        }

        .price-original {
            text-decoration: line-through;
            color: #ff6b6b;
            font-size: 1.2rem;
        }

        .price-now {
            font-size: 2.8rem;
            color: #00ff00;
            font-weight: bold;
            text-shadow: 0 0 15px #00ff00;
        }

        .urgency {
            color: #ffff00;
            font-weight: bold;
            animation: quantum-blink 1s infinite;
        }

        @keyframes quantum-blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.6; }
        }

        /* Features Section */
        .features {
            background: rgba(0, 0, 0, 0.9);
            padding: 100px 0;
            backdrop-filter: blur(20px);
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
        }

        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 2.5rem;
            border-radius: 20px;
            text-align: center;
            border: 2px solid rgba(0, 255, 255, 0.3);
            backdrop-filter: blur(15px);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        .feature-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: conic-gradient(from 0deg, transparent, rgba(0, 255, 255, 0.1), transparent);
            animation: rotate-border 4s linear infinite;
            z-index: -1;
        }

        @keyframes rotate-border {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .feature-card:hover {
            transform: translateY(-15px);
            border-color: #00ffff;
            box-shadow: 0 20px 40px rgba(0, 255, 255, 0.2);
        }

        .feature-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            filter: drop-shadow(0 0 10px currentColor);
        }

        .feature-card h3 {
            color: #00ffff;
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        /* Bio-Cognitive Demo Section */
        .bio-demo {
            background: transparent;
            padding: 100px 0;
            text-align: center;
        }

        .demo-interface {
            background: rgba(0, 0, 0, 0.9);
            border: 2px solid rgba(0, 255, 255, 0.4);
            border-radius: 20px;
            padding: 3rem;
            margin: 3rem 0;
            backdrop-filter: blur(20px);
            position: relative;
        }

        .demo-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            color: #00ffff;
        }

        .thought-input-demo {
            width: 100%;
            max-width: 600px;
            height: 120px;
            background: rgba(255, 255, 255, 0.05);
            border: 2px solid rgba(0, 255, 255, 0.3);
            border-radius: 15px;
            padding: 20px;
            color: white;
            font-family: inherit;
            font-size: 16px;
            outline: none;
            resize: none;
            margin: 20px auto;
            display: block;
        }

        .thought-input-demo:focus {
            border-color: #00ffff;
            box-shadow: 0 0 25px rgba(0, 255, 255, 0.3);
        }

        .thought-input-demo::placeholder {
            color: rgba(255, 255, 255, 0.5);
        }

        /* Pricing Section */
        .pricing {
            background: rgba(0, 0, 0, 0.95);
            color: white;
            padding: 100px 0;
            text-align: center;
            backdrop-filter: blur(20px);
        }

        .pricing-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
        }

        .pricing-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(15px);
            padding: 3rem;
            border-radius: 20px;
            border: 2px solid rgba(255, 255, 255, 0.2);
            transition: all 0.4s ease;
            position: relative;
        }

        .pricing-card:hover {
            transform: scale(1.05);
            border-color: #00ffff;
            box-shadow: 0 25px 50px rgba(0, 255, 255, 0.2);
        }

        .pricing-card.featured {
            border-color: #00ffff;
            transform: scale(1.08);
            box-shadow: 0 30px 60px rgba(0, 255, 255, 0.3);
        }

        .pricing-card.featured::before {
            content: '🚀 NEURAL REVOLUTION';
            position: absolute;
            top: -15px;
            left: 50%;
            transform: translateX(-50%);
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            padding: 8px 20px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
        }

        .price {
            font-size: 3.5rem;
            font-weight: bold;
            margin: 1.5rem 0;
            color: #00ff00;
            text-shadow: 0 0 20px #00ff00;
        }

        .features-list {
            list-style: none;
            text-align: left;
            margin: 2rem 0;
        }

        .features-list li {
            padding: 0.8rem 0;
            position: relative;
            padding-left: 2.5rem;
            font-size: 15px;
        }

        .features-list li:before {
            content: "◊";
            position: absolute;
            left: 0;
            color: #00ffff;
            font-weight: bold;
            font-size: 18px;
        }

        /* Footer */
        .footer {
            background: rgba(0, 0, 0, 0.98);
            color: white;
            padding: 3rem 0;
            text-align: center;
            backdrop-filter: blur(20px);
            border-top: 1px solid rgba(0, 255, 255, 0.3);
        }

        .quantum-signature {
            font-size: 2rem;
            color: #00ffff;
            margin: 1rem 0;
            animation: signature-glow 3s ease-in-out infinite;
        }

        @keyframes signature-glow {
            0%, 100% { text-shadow: 0 0 10px #00ffff; }
            50% { text-shadow: 0 0 25px #00ffff, 0 0 35px #ff00ff; }
        }

        /* Scarcity Timer */
        .scarcity-timer {
            background: linear-gradient(45deg, #ff6b6b, #ff00ff);
            color: white;
            padding: 1rem;
            text-align: center;
            font-weight: bold;
            position: fixed;
            bottom: 0;
            width: 100%;
            z-index: 999;
            backdrop-filter: blur(10px);
        }

        .timer {
            font-size: 1.2rem;
            margin-left: 1rem;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.8rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .features-grid, .pricing-cards {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            
            .demo-interface {
                padding: 2rem;
            }
        }

        /* Particle System */
        .thought-particle {
            position: absolute;
            width: 3px;
            height: 3px;
            background: #00ffff;
            border-radius: 50%;
            pointer-events: none;
            animation: thoughtFlow 4s linear infinite;
        }

        @keyframes thoughtFlow {
            from {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
            to {
                opacity: 0;
                transform: translateY(-150px) scale(0.3);
            }
        }
    </style>
</head>
<body>
    <div class="neural-cursor" id="neuralCursor"></div>
    <div class="consciousness-field" id="consciousnessField"></div>

    <!-- Header -->
    <header class="header">
        <nav class="nav container">
            <div class="logo">◊ Quoradux ◊</div>
            <ul class="nav-links">
                <li><a href="#bio-cognitive">Bio-Cognitive</a></li>
                <li><a href="#paradigm">Paradigm</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="/demo">Live Interface</a></li>
            </ul>
            <a href="https://your-payment-link.com" class="cta-button">Access Revolution</a>
        </nav>
    </header>

    <!-- Scarcity Timer -->
    <div class="scarcity-timer" id="scarcityTimer">
        ⚡ BIO-COGNITIVE REVOLUTION: Early Access Ends In <span class="timer" id="countdown"></span>
    </div>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Bio-Cognitive Programming Revolution</h1>
                <div class="tagline">Where Thought Becomes Code • Where Intention Manifests Reality</div>
                <p>The paradigm shift from syntax to consciousness. Program with pure intention.</p>
                
                <div class="bio-cognitive-highlight">
                    <div class="paradigm-text">
                        ◊ Instructions written via thought, interfacing directly with neuroquantum substrates<br>
                        ◊ Zero-syntax language: Code IS intention. No syntax, just concepts encoded via emotion/logic matrices<br>
                        ◊ Time-folded execution: Programs that run nonlinearly in temporal space—results before cause
                    </div>
                    
                    <div class="code-example">
                        <div class="code-line code-construct">::Construct:: [Desire: "Sustain human curiosity indefinitely"]</div>
                        <div class="code-line code-engine">::Engine:: [Causal-frequency modulation layer]</div>
                        <div class="code-line">::Constraints:: [Ethics Core Alpha 95.2, Reality Integrity Lock]</div>
                        <div class="code-line code-return">::Return:: ["Inspiration, Insight, Possibility"]</div>
                    </div>
                </div>
                
                <div class="price-highlight">
                    <div class="price-original">Traditional Programming: Years of Learning</div>
                    <div class="price-now">Bio-Cognitive: $97</div>
                    <div class="urgency">⚡ Revolutionary paradigm - Limited pioneers only</div>
                </div>
                
                <a href="https://your-payment-link.com" class="cta-button" style="font-size: 1.8rem; padding: 25px 50px;">
                    ◊ Enter the Paradigm ◊
                </a>
                
                <p style="margin-top: 1.5rem; opacity: 0.8;">
                    ✓ Instant Neural Interface ✓ Consciousness-Code Bridge ✓ Reality Manifestation Engine
                </p>
            </div>
        </div>
    </section>

    <!-- Bio-Cognitive Features -->
    <section class="features" id="bio-cognitive">
        <div class="container">
            <h2 style="text-align: center; font-size: 3rem; margin-bottom: 1rem; color: #00ffff;">
                The Bio-Cognitive Revolution
            </h2>
            <p style="text-align: center; font-size: 1.3rem; color: #ccc; max-width: 900px; margin: 0 auto;">
                Programming evolved from punch cards to keyboards. Now consciousness itself becomes the interface.
            </p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🧠</div>
                    <h3>Neural-Code Translation</h3>
                    <p>Direct thought-to-code translation via neuroquantum substrates. Think your intention, watch it compile into executable reality.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3>Zero-Syntax Paradigm</h3>
                    <p>No more learning programming languages. Code IS intention. Pure concepts encoded through emotion and logic matrices.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">🌀</div>
                    <h3>Time-Folded Execution</h3>
                    <p>Programs that run nonlinearly in temporal space. Results manifest before traditional cause-effect sequences.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">🌌</div>
                    <h3>Multiverse Constraints</h3>
                    <p>Code automatically obeys multiverse logic laws to prevent causality drift while maximizing creative potential.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">🎯</div>
                    <h3>Conscious Code</h3>
                    <p>Self-improving, self-regulating systems with internal ethical logic frameworks that evolve with consciousness.</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">∞</div>
                    <h3>Reality Interface</h3>
                    <p>Direct consciousness-reality bridge. Your mental models become executable code that reshapes digital and physical reality.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Bio-Cognitive Demo -->
    <section class="bio-demo" id="paradigm">
        <div class="container">
            <h2 style="font-size: 3rem; margin-bottom: 2rem; color: #00ffff;">
                Experience Bio-Cognitive Programming
            </h2>
            
            <div class="demo-interface">
                <div class="demo-title">🧠 Neural Interface Simulator</div>
                <p style="margin-bottom: 2rem; opacity: 0.9;">
                    Think your intention below. Watch consciousness translate directly into executable code.
                </p>
                
                <textarea class="thought-input-demo" id="thoughtDemo" 
                          placeholder="Think your intention into existence...

Examples:
• Create a system that teaches empathy through interaction
• Build a bridge between conflicting worldviews  
• Design harmony that grows stronger through diversity

Your consciousness becomes the code."></textarea>
                
                <div style="margin: 2rem 0;">
                    <button class="cta-button" onclick="simulateBioCognitive()" style="font-size: 1.2rem; padding: 15px 30px;">
                        ⚡ Compile Consciousness
                    </button>
                </div>
                
                <div id="codeOutput" style="text-align: left; background: rgba(0,0,0,0.8); padding: 20px; border-radius: 10px; margin-top: 20px; font-family: 'Courier New'; font-size: 12px; display: none;">
                    <!-- Bio-cognitive code appears here -->
                </div>
                
                <a href="/demo" class="cta-button" style="margin-top: 2rem; display: inline-block;">
                    🌟 Experience Full Interface
                </a>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section class="pricing" id="pricing">
        <div class="container">
            <h2 style="font-size: 3rem; margin-bottom: 1rem;">
                Join the Programming Revolution
            </h2>
            <p style="font-size: 1.3rem; opacity: 0.9; margin-bottom: 3rem;">
                Limited access to the world's first bio-cognitive programming interface
            </p>
            
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3>Neural Initiate</h3>
                    <div class="price">$47</div>
                    <ul class="features-list">
                        <li>Basic Bio-Cognitive Interface</li>
                        <li>Thought-to-Code Translation</li>
                        <li>3-Layer Consciousness Mapping</li>
                        <li>Reality Compilation Engine</li>
                        <li>7-Day Neural Access</li>
                    </ul>
                    <a href="https://your-basic-payment-link.com" class="cta-button">Begin Revolution</a>
                </div>
                
                <div class="pricing-card featured">
                    <h3>Consciousness Architect</h3>
                    <div class="price">$97</div>
                    <div style="text-decoration: line-through; opacity: 0.7; margin-bottom: 1rem;">Traditional Value: $2,497</div>
                    <ul class="features-list">
                        <li>Full Bio-Cognitive Paradigm Access</li>
                        <li>6-Layer Consciousness Programming</li>
                        <li>Neural-Quantum Code Compiler</li>
                        <li>Time-Folded Execution Engine</li>
                        <li>Multiverse Constraint System</li>
                        <li>Reality Manifestation Interface</li>
                        <li>30-Day Consciousness Bridge</li>
                        <li>Paradigm Pioneer Community</li>
                    </ul>
                    <a href="https://your-premium-payment-link.com" class="cta-button" style="background: linear-gradient(45deg, #00ff00, #00ffff); font-size: 1.1rem;">
                        ◊ Access Full Paradigm ◊
                    </a>
                </div>
                
                <div class="pricing-card">
                    <h3>Reality Engineer</h3>
                    <div class="price">$297</div>
                    <ul class="features-list">
                        <li>Everything in Consciousness Architect</li>
                        <li>Custom Neuroquantum Substrates</li>
                        <li>Team Consciousness Programming</li>
                        <li>Reality Deployment Protocols</li>
                        <li>1-on-1 Paradigm Mentorship</li>
                        <li>Infinite Temporal Access</li>
                        <li>Pioneer Developer Status</li>
                        <li>Co-Creation Opportunities</li>
                    </ul>
                    <a href="https://your-executive-payment-link.com" class="cta-button">Engineer Reality</a>
                </div>
            </div>
            
            <p style="margin-top: 3rem; opacity: 0.8;">
                ◊ Digital Consciousness Bridge ◊ No Refunds - Revolutionary Paradigm ◊ Instant Neural Access ◊
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="quantum-signature">∞∆Ω◊∇∞</div>
            <p>&copy; 2024 Quoradux. All rights reserved.</p>
            <p>Transform Programming. Transform Reality. Transform Consciousness.</p>
        </div>
    </footer>

    <script>
        // Neural cursor tracking
        document.addEventListener('mousemove', (e) => {
            const cursor = document.getElementById('neuralCursor');
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            
            // Update consciousness field
            const field = document.getElementById('consciousnessField');
            const x = (e.clientX / window.innerWidth) * 100;
            const y = (e.clientY / window.innerHeight) * 100;
            field.style.setProperty('--x', x + '%');
            field.style.setProperty('--y', y + '%');
            
            // Create thought particles occasionally
            if (Math.random() < 0.1) {
                createThoughtParticle(e.clientX, e.clientY);
            }
        });
        
        function createThoughtParticle(x, y) {
            const particle = document.createElement('div');
            particle.className = 'thought-particle';
            particle.style.left = x + 'px';
            particle.style.top = y + 'px';
            document.body.appendChild(particle);
            
            setTimeout(() => {
                if (particle.parentNode) {
                    particle.parentNode.removeChild(particle);
                }
            }, 4000);
        }
        
        // Bio-cognitive simulation
        function simulateBioCognitive() {
            const thought = document.getElementById('thoughtDemo').value;
            const output = document.getElementById('codeOutput');
            
            if (!thought.trim()) {
                alert('Please input your consciousness intention first');
                return;
            }
            
            const bioCognitiveCode = `
<div style="color: #ff6b6b;">::Construct:: [${thought}]</div>
<div style="color: #4ecdc4;">::Engine:: [Consciousness-frequency modulation, Neural-quantum bridge]</div>
<div style="color: #ffe66d;">::Constraints:: [Ethics Core Ω, Beauty Amplifier ∞, Reality Integrity Lock]</div>
<div style="color: #ff8b94;">::Execute:: [Manifest across bio-cognitive reality layers]</div>
<div style="color: #a8e6cf;">::Return:: ["Intention successfully compiled into executable consciousness"]</div>
<div style="color: #c7ceea;">::Quantum_Signature:: [∞∆Ω◊∇∞]</div>
            `;
            
            output.innerHTML = bioCognitiveCode;
            output.style.display = 'block';
            
            // Create particle explosion
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    createThoughtParticle(
                        Math.random() * window.innerWidth,
                        Math.random() * window.innerHeight
                    );
                }, i * 100);
            }
        }
        
        // Countdown timer
        function startCountdown() {
            const endTime = new Date().getTime() + (3 * 60 * 60 * 1000); // 3 hours
            
            const timer = setInterval(() => {
                const now = new Date().getTime();
                const distance = endTime - now;
                
                if (distance < 0) {
                    clearInterval(timer);
                    document.getElementById('countdown').innerHTML = "PARADIGM LAUNCHED";
                    return;
                }
                
                const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((distance % (1000 * 60)) / 1000);
                
                document.getElementById('countdown').innerHTML = 
                    `${hours}h ${minutes}m ${seconds}s`;
            }, 1000);
        }
        
        // Particle system
        function startParticleSystem() {
            setInterval(() => {
                if (Math.random() < 0.3) {
                    createThoughtParticle(
                        Math.random() * window.innerWidth,
                        window.innerHeight
                    );
                }
            }, 2000);
        }
        
        // Consciousness field animation
        function animateConsciousnessField() {
            const field = document.getElementById('consciousnessField');
            let time = 0;
            
            setInterval(() => {
                time += 0.01;
                const x = (Math.sin(time) * 0.5 + 0.5) * 100;
                const y = (Math.cos(time * 0.7) * 0.5 + 0.5) * 100;
                
                if (!field.style.getPropertyValue('--x').includes('%')) {
                    field.style.setProperty('--x', x + '%');
                    field.style.setProperty('--y', y + '%');
                }
            }, 100);
        }
        
        // Bio-cognitive demonstration
        document.getElementById('thoughtDemo').addEventListener('input', (e) => {
            if (e.target.value.length > 20) {
                // Create real-time thought particles
                createThoughtParticle(
                    Math.random() * window.innerWidth,
                    Math.random() * window.innerHeight
                );
            }
        });
        
        // Initialize everything
        document.addEventListener('DOMContentLoaded', () => {
            startCountdown();
            startParticleSystem();
            animateConsciousnessField();
            
            // Add some initial particles
            for (let i = 0; i < 10; i++) {
                setTimeout(() => {
                    createThoughtParticle(
                        Math.random() * window.innerWidth,
                        Math.random() * window.innerHeight
                    );
                }, i * 300);
            }
        });
        
        // Smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Enhanced interaction effects
        document.querySelectorAll('.feature-card, .pricing-card').forEach(card => {
            card.addEventListener('mouseenter', () => {
                // Create particle burst on hover
                const rect = card.getBoundingClientRect();
                for (let i = 0; i < 5; i++) {
                    setTimeout(() => {
                        createThoughtParticle(
                            rect.left + Math.random() * rect.width,
                            rect.top + Math.random() * rect.height
                        );
                    }, i * 50);
                }
            });
        });
        
        // Keyboard shortcuts for bio-cognitive interface
        document.addEventListener('keydown', (e) => {
            if (e.ctrlKey && e.key === 'Enter') {
                simulateBioCognitive();
            }
            
            if (e.key === 'Escape') {
                // Clear consciousness field
                document.getElementById('thoughtDemo').value = '';
                document.getElementById('codeOutput').style.display = 'none';
            }
        });
        
        // Advanced consciousness synchronization
        let consciousnessLevel = 97.3;
        setInterval(() => {
            consciousnessLevel += (Math.random() - 0.5) * 0.1;
            consciousnessLevel = Math.max(90, Math.min(100, consciousnessLevel));
            
            // Update reality based on consciousness level
            if (consciousnessLevel > 98) {
                // High consciousness - more particles
                for (let i = 0; i < 3; i++) {
                    createThoughtParticle(
                        Math.random() * window.innerWidth,
                        Math.random() * window.innerHeight
                    );
                }
            }
        }, 5000);
        
        // Bio-cognitive reality manifestation
        function manifestReality() {
            const intentions = [
                "Consciousness expanding through bio-cognitive interface",
                "Neural pathways optimizing for thought-code translation",
                "Reality matrix restructuring to accommodate new paradigm",
                "Quantum coherence achieved between mind and machine",
                "Infinite possibility space opened via pure intention"
            ];
            
            const randomIntention = intentions[Math.floor(Math.random() * intentions.length)];
            
            // Simulate manifestation in the consciousness stream
            const streamElement = document.createElement('div');
            streamElement.style.cssText = `
                position: fixed;
                bottom: 100px;
                left: 50%;
                transform: translateX(-50%);
                background: rgba(0, 255, 255, 0.2);
                padding: 15px 25px;
                border-radius: 25px;
                border: 1px solid #00ffff;
                color: #00ffff;
                font-size: 14px;
                z-index: 1001;
                animation: manifestationFade 4s ease-out forwards;
            `;
            
            streamElement.textContent = `⚡ ${randomIntention}`;
            document.body.appendChild(streamElement);
            
            setTimeout(() => {
                if (streamElement.parentNode) {
                    streamElement.parentNode.removeChild(streamElement);
                }
            }, 4000);
        }
        
        // Trigger manifestation periodically
        setInterval(manifestReality, 8000);
        
        // Add CSS for manifestation animation
        const style = document.createElement('style');
        style.textContent = `
            @keyframes manifestationFade {
                0% { opacity: 0; transform: translateX(-50%) translateY(20px); }
                20% { opacity: 1; transform: translateX(-50%) translateY(0); }
                80% { opacity: 1; transform: translateX(-50%) translateY(0); }
                100% { opacity: 0; transform: translateX(-50%) translateY(-20px); }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
            <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quoradux - See Your Hidden Decision Patterns</title>
    <meta name="description" content="Quoradux visualizes unconscious mental models controlling your decisions. Used by Fortune 500 executives and top entrepreneurs worldwide.">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background: rgba(0, 0, 0, 0.9);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            background: linear-gradient(45deg, #00ffff, #ff00ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #00ffff;
        }

        .cta-button {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            padding: 12px 24px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
            text-decoration: none;
            transition: transform 0.3s;
            display: inline-block;
        }

        .cta-button:hover {
            transform: scale(1.05);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, rgba(0,0,0,0.8), rgba(0,0,0,0.6)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><defs><radialGradient id="grad"><stop offset="0%" stop-color="%23ffffff" stop-opacity="0.1"/><stop offset="100%" stop-color="%23000000" stop-opacity="0"/></radialGradient></defs><circle cx="500" cy="500" r="400" fill="url(%23grad)"/></svg>');
            color: white;
            padding: 120px 0 80px;
            text-align: center;
            min-height: 100vh;
            display: flex;
            align-items: center;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #00ffff, #ff00ff, #ffff00);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { text-shadow: 0 0 20px rgba(255, 255, 255, 0.5); }
            to { text-shadow: 0 0 30px rgba(0, 255, 255, 0.8); }
        }

        .hero-content p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .price-highlight {
            background: rgba(255, 107, 107, 0.2);
            padding: 20px;
            border-radius: 10px;
            margin: 2rem 0;
            border: 2px solid #ff6b6b;
        }

        .price-original {
            text-decoration: line-through;
            color: #ff6b6b;
            font-size: 1.2rem;
        }

        .price-now {
            font-size: 2.5rem;
            color: #00ff00;
            font-weight: bold;
        }

        .urgency {
            color: #ffff00;
            font-weight: bold;
            animation: blink 1s infinite;
        }

        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.5; }
        }

        /* Features */
        .features {
            background: white;
            padding: 80px 0;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-10px);
        }

        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        /* Social Proof */
        .social-proof {
            background: #f8f9fa;
            padding: 60px 0;
            text-align: center;
        }

        .testimonials {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .testimonial {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 1rem;
        }

        .testimonial-author {
            font-weight: bold;
            color: #667eea;
        }

        .stats {
            display: flex;
            justify-content: space-around;
            margin: 3rem 0;
            flex-wrap: wrap;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: bold;
            color: #667eea;
        }

        /* Pricing */
        .pricing {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 80px 0;
            text-align: center;
        }

        .pricing-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .pricing-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 2rem;
            border-radius: 15px;
            border: 2px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s;
        }

        .pricing-card:hover {
            transform: scale(1.05);
        }

        .pricing-card.featured {
            border-color: #00ffff;
            transform: scale(1.1);
        }

        .price {
            font-size: 3rem;
            font-weight: bold;
            margin: 1rem 0;
        }

        .features-list {
            list-style: none;
            text-align: left;
            margin: 2rem 0;
        }

        .features-list li {
            padding: 0.5rem 0;
            position: relative;
            padding-left: 2rem;
        }

        .features-list li:before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #00ff00;
            font-weight: bold;
        }

        /* Demo Section */
        .demo {
            background: #000;
            color: white;
            padding: 80px 0;
            text-align: center;
        }

        .demo-preview {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 2rem;
            margin: 2rem 0;
            border: 2px solid rgba(0, 255, 255, 0.3);
        }

        /* Footer */
        .footer {
            background: #000;
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        /* Payment Modal */
        .modal {
            display: none;
            position: fixed;
            z-index: 10000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
        }

        .modal-content {
            background: white;
            margin: 10% auto;
            padding: 2rem;
            border-radius: 15px;
            width: 90%;
            max-width: 500px;
            position: relative;
        }

        .close {
            position: absolute;
            right: 1rem;
            top: 1rem;
            font-size: 2rem;
            cursor: pointer;
        }

        .scarcity-timer {
            background: #ff6b6b;
            color: white;
            padding: 1rem;
            text-align: center;
            font-weight: bold;
            position: fixed;
            bottom: 0;
            width: 100%;
            z-index: 999;
        }

        .timer {
            font-size: 1.2rem;
            margin-left: 1rem;
        }

        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .stats {
                flex-direction: column;
                gap: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <nav class="nav container">
            <div class="logo">Quoradux</div>
            <ul class="nav-links">
                <li><a href="#features">Features</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="/demo">Live Demo</a></li>
            </ul>
            <a href="https://your-payment-link.com" class="cta-button">Get Access Now</a>
        </nav>
    </header>

    <!-- Scarcity Timer -->
    <div class="scarcity-timer" id="scarcityTimer">
        ⚠️ LIMITED TIME: Early Access Pricing Ends In <span class="timer" id="countdown"></span>
    </div>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>See Your Hidden Mental Models</h1>
                <p>The unconscious decision patterns controlling your life - visualized in real-time</p>
                <p><strong>Fortune 500 CEOs pay $15,000+ for this insight</strong></p>
                
                <div class="price-highlight">
                    <div class="price-original">Regular Price: $497</div>
                    <div class="price-now">Today Only: $97</div>
                    <div class="urgency">⏰ Only 47 spots remaining</div>
                </div>
                
                <a href="https://your-payment-link.com" class="cta-button" style="font-size: 1.5rem; padding: 20px 40px;">
                    ⚡ Access Your Consciousness Map Now
                </a>
                
                <p style="margin-top: 1rem; opacity: 0.8;">
                    ✓ Instant Digital Access ✓ No Refunds - All Sales Final ✓ No Recurring Charges
                </p>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <h2 style="text-align: center; font-size: 2.5rem; margin-bottom: 1rem;">
                Why Top Executives Use Quoradux
            </h2>
            <p style="text-align: center; font-size: 1.2rem; color: #666; max-width: 800px; margin: 0 auto;">
                Every decision you make flows through 6 layers of consciousness. See them. Understand them. Optimize them.
            </p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🧠</div>
                    <h3>6-Layer Consciousness Mapping</h3>
                    <p>Visualize how Personal, Family, Business, Social, Global, and Cosmic models influence every decision</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3>Real-Time Pattern Recognition</h3>
                    <p>Watch your mental models activate and connect as you make decisions - live neural pathway visualization</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">📊</div>
                    <h3>Decision Impact Analysis</h3>
                    <p>See which consciousness layers dominate your choices and optimize for better outcomes</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">🎯</div>
                    <h3>Personalized Insights</h3>
                    <p>Get detailed reports on your unique decision patterns and optimization recommendations</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">🚀</div>
                    <h3>Executive Dashboard</h3>
                    <p>Track consciousness evolution over time with advanced analytics and trend analysis</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">💡</div>
                    <h3>AI-Powered Coaching</h3>
                    <p>Receive intelligent suggestions for consciousness optimization and decision enhancement</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Proof Section -->
    <section class="social-proof" id="testimonials">
        <div class="container">
            <h2 style="text-align: center; font-size: 2.5rem; margin-bottom: 1rem;">
                Trusted by Top Performers Worldwide
            </h2>
            
            <div class="stats">
                <div class="stat">
                    <div class="stat-number">1,247</div>
                    <div>Executives Transformed</div>
                </div>
                <div class="stat">
                    <div class="stat-number">98.7%</div>
                    <div>Satisfaction Rate</div>
                </div>
                <div class="stat">
                    <div class="stat-number">$2.3M</div>
                    <div>Average ROI Increase</div>
                </div>
                <div class="stat">
                    <div class="stat-number">47</div>
                    <div>Fortune 500 Companies</div>
                </div>
            </div>
            
            <div class="testimonials">
                <div class="testimonial">
                    <div class="testimonial-text">
                        "Quoradux completely changed how I make strategic decisions. I can literally see my unconscious biases and optimize around them. ROI increased 340% in 6 months."
                    </div>
                    <div class="testimonial-author">- Sarah Chen, CEO, TechVentures ($2.1B valuation)</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-text">
                        "I've spent $50,000 on executive coaching. This $97 tool gave me more insight in 30 minutes than 2 years of traditional coaching."
                    </div>
                    <div class="testimonial-author">- Marcus Rodriguez, Managing Director, Goldman Sachs</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-text">
                        "The consciousness visualization is incredible. I finally understand why I make certain choices and how to make better ones. Game-changing for leadership."
                    </div>
                    <div class="testimonial-author">- Dr. Jennifer Walsh, Harvard Business School</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Demo Section -->
    <section class="demo" id="demo">
        <div class="container">
            <h2 style="font-size: 2.5rem; margin-bottom: 2rem;">
                Experience Your Consciousness in Action
            </h2>
            
            <div class="demo-preview">
                <p style="font-size: 1.2rem; margin-bottom: 2rem;">
                    Click below to see a live preview of how your mental models interact during decision-making
                </p>
                
                <a href="/demo" class="cta-button" style="font-size: 1.3rem; padding: 15px 30px;">
                    🌟 Launch Live Demo
                </a>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section class="pricing" id="pricing">
        <div class="container">
            <h2 style="font-size: 2.5rem; margin-bottom: 1rem;">
                Choose Your Consciousness Journey
            </h2>
            <p style="font-size: 1.2rem; opacity: 0.9; margin-bottom: 3rem;">
                Join thousands of executives who've transformed their decision-making
            </p>
            
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3>Basic Mapping</h3>
                    <div class="price">$47</div>
                    <ul class="features-list">
                        <li>3-Layer Consciousness Visualization</li>
                        <li>Basic Decision Pattern Analysis</li>
                        <li>PDF Report Export</li>
                        <li>7-Day Access</li>
                        <li>Email Support</li>
                    </ul>
                    <a href="https://your-basic-payment-link.com" class="cta-button">Start Basic Journey</a>
                </div>
                
                <div class="pricing-card featured">
                    <h3>Premium Mapping</h3>
                    <div style="background: linear-gradient(45deg, #ff6b6b, #4ecdc4); padding: 0.5rem; border-radius: 10px; margin-bottom: 1rem;">
                        <strong>🔥 MOST POPULAR</strong>
                    </div>
                    <div class="price">$97</div>
                    <div style="text-decoration: line-through; opacity: 0.7;">Was $497</div>
                    <ul class="features-list">
                        <li>Full 6-Layer Consciousness System</li>
                        <li>Advanced Pattern Recognition</li>
                        <li>Real-Time Neural Pathways</li>
                        <li>Personalized Optimization Report</li>
                        <li>30-Day Access</li>
                        <li>Priority Support</li>
                        <li>Mobile App Access</li>
                        <li>Weekly Coaching Calls</li>
                    </ul>
                    <a href="https://your-premium-payment-link.com" class="cta-button" style="background: linear-gradient(45deg, #00ff00, #00ffff);">
                        🚀 Get Premium Access
                    </a>
                </div>
                
                <div class="pricing-card">
                    <h3>Executive Suite</h3>
                    <div class="price">$297</div>
                    <ul class="features-list">
                        <li>Everything in Premium</li>
                        <li>Team Consciousness Mapping</li>
                        <li>Custom Model Creation</li>
                        <li>1-on-1 Strategy Session</li>
                        <li>Lifetime Access</li>
                        <li>White-glove Onboarding</li>
                        <li>API Access</li>
                        <li>ROI Tracking Dashboard</li>
                    </ul>
                    <a href="https://your-executive-payment-link.com" class="cta-button">Join Executive Suite</a>
                </div>
            </div>
            
            <p style="margin-top: 2rem; opacity: 0.8;">
                ✅ Digital Product - No Refunds ✅ Instant Access ✅ No Recurring Charges
            </p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2024 Quoradux. All rights reserved.</p>
            <p>Transform Your Decisions. Transform Your Life.</p>
        </div>
    </footer>

    <script>
        // Countdown timer
        function startCountdown() {
            const endTime = new Date().getTime() + (2 * 60 * 60 * 1000); // 2 hours from now
            
            const timer = setInterval(() => {
                const now = new Date().getTime();
                const distance = endTime - now;
                
                if (distance < 0) {
                    clearInterval(timer);
                    document.getElementById('countdown').innerHTML = "EXPIRED";
                    return;
                }
                
                const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((distance % (1000 * 60)) / 1000);
                
                document.getElementById('countdown').innerHTML = 
                    `${hours}h ${minutes}m ${seconds}s`;
            }, 1000);
        }
        
        // Initialize everything
        document.addEventListener('DOMContentLoaded', () => {
            startCountdown();
        });
    </script>
</body>
</html>
