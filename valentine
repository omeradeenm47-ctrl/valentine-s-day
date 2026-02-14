<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>For Farzana ✈️💗</title>
    <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Quicksand:wght@400;500;600&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    
    <style>
        :root {
            /* LDR Palette: Soft Blush -> Peach -> Lavender */
            --bg-gradient: linear-gradient(180deg, #fff0f5 0%, #fff5f0 40%, #f3e5f5 100%);
            --primary: #9fa8da; /* Soft Periwinkle */
            --accent: #ff8fa3;  /* Warm Pink */
            --text-main: #5c5c8a;
            --text-light: #8e8ea8;
            --card-bg: rgba(255, 255, 255, 0.85);
            --bubble-sent: #e8eaf6;
            --bubble-rcvd: #ffffff;
            --shadow: 0 10px 30px rgba(159, 168, 218, 0.15);
        }

        * {
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            margin: 0;
            font-family: 'Quicksand', sans-serif;
            background: var(--bg-gradient);
            color: var(--text-main);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        h1, h2, h3 {
            margin: 0;
            font-family: 'Nunito', sans-serif;
            font-weight: 700;
        }

        /* --- BACKGROUND DECOR --- */
        .bg-heart {
            position: fixed;
            color: rgba(255, 143, 163, 0.15);
            z-index: -1;
            animation: floatBg 15s infinite ease-in-out;
            pointer-events: none;
        }
        @keyframes floatBg {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(10deg); }
        }

        /* --- LAYOUT --- */
        .section {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 2rem;
            position: relative;
            text-align: center;
        }

        .container {
            max-width: 500px;
            width: 100%;
        }

        /* --- CARDS --- */
        .card {
            background: var(--card-bg);
            backdrop-filter: blur(10px);
            padding: 2.5rem 2rem;
            border-radius: 30px;
            box-shadow: var(--shadow);
            border: 1px solid rgba(255,255,255,0.6);
            margin: 1rem 0;
            transition: transform 0.3s ease;
        }

        /* --- ANIMATIONS --- */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 1.2s cubic-bezier(0.2, 0.8, 0.2, 1), transform 1.2s cubic-bezier(0.2, 0.8, 0.2, 1);
        }
        .fade-in.visible { opacity: 1; transform: translateY(0); }

        .pulse { animation: pulse 2s infinite ease-in-out; }
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.8; }
            50% { transform: scale(1.1); opacity: 1; }
        }

        /* --- 4. CHAT BUBBLES --- */
        .chat-container {
            display: flex; flex-direction: column; gap: 15px; width: 100%;
            margin-top: 2rem;
        }
        .bubble {
            background: var(--bubble-rcvd);
            padding: 15px 20px;
            border-radius: 20px;
            border-bottom-left-radius: 4px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.03);
            align-self: flex-start;
            max-width: 85%;
            text-align: left;
            opacity: 0; transform: translateX(-20px);
            transition: all 0.6s ease;
        }
        .bubble.right {
            background: var(--bubble-sent);
            border-bottom-left-radius: 20px;
            border-bottom-right-radius: 4px;
            align-self: flex-end;
            text-align: right;
            transform: translateX(20px);
        }
        .bubble.visible { opacity: 1; transform: translateX(0); }

        /* --- BUTTONS --- */
        .btn-group { display: flex; gap: 15px; justify-content: center; margin-top: 2rem; }
        .btn {
            background: var(--accent); color: white; border: none;
            padding: 14px 32px; border-radius: 50px;
            font-size: 1.1rem; font-weight: 700; cursor: pointer;
            box-shadow: 0 5px 15px rgba(255, 143, 163, 0.3);
            transition: transform 0.2s;
            font-family: 'Nunito', sans-serif;
        }
        .btn:active { transform: scale(0.95); }
        .btn.secondary { background: white; color: var(--accent); border: 2px solid var(--accent); }

        /* --- 6. LOVE METER --- */
        .meter-wrapper {
            background: white; height: 25px; border-radius: 25px;
            margin-top: 20px; overflow: hidden;
            box-shadow: inset 0 2px 5px rgba(0,0,0,0.05);
            position: relative;
        }
        .meter-fill {
            height: 100%; width: 0%;
            background: linear-gradient(90deg, #ffccd5, #ff8fa3);
            transition: width 0.4s cubic-bezier(0.2, 0.8, 0.2, 1);
        }
        .tap-heart-btn {
            font-size: 3.5rem; cursor: pointer; margin: 10px 0;
            transition: transform 0.1s; display: inline-block;
        }
        .tap-heart-btn:active { transform: scale(0.8); }

        /* --- 8. PRESENCE (DOTS) --- */
        .dots-container {
            display: flex; justify-content: center; align-items: center;
            height: 100px; position: relative; width: 100%;
        }
        .dot {
            width: 18px; height: 18px; border-radius: 50%;
            background: var(--accent); position: absolute;
            transition: all 2s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .dots-container.visible .dot-left { left: 50%; transform: translateX(-50%); }
        .dots-container.visible .dot-right { right: 50%; transform: translateX(50%); }
        
        .dot-left { left: 20%; }
        .dot-right { right: 20%; }

        .merged-heart {
            position: absolute; font-size: 3rem; color: var(--accent);
            opacity: 0; transform: scale(0);
            transition: all 0.5s ease 1.8s; /* Wait for dots to merge */
        }
        .dots-container.visible .merged-heart { opacity: 1; transform: scale(1); animation: pulse 1.5s infinite; }

        /* --- HIDDEN CONTENT WRAPPER --- */
        #hidden-content { display: none; opacity: 0; transition: opacity 1s ease; }

    </style>
</head>
<body>

    <!-- Background Decor -->
    <div class="bg-heart" style="top: 10%; left: 5%; font-size: 4rem;">☁️</div>
    <div class="bg-heart" style="bottom: 20%; right: 5%; font-size: 6rem;">🤍</div>
    <div class="bg-heart" style="top: 40%; right: 15%; font-size: 3rem;">✨</div>

    <!-- 1️⃣ OPENING: Distance -->
    <section class="section" id="intro">
        <div class="container fade-in visible">
            <h2 style="font-size: 1.1rem; letter-spacing: 2px; text-transform: uppercase; color: var(--primary);">Distance</h2>
            <h1 style="font-size: 3rem; margin: 20px 0;">Miles apart... ✈️</h1>
            <p style="font-size: 1.3rem; color: var(--text-light);">But somehow still close 💗</p>
            <div style="margin-top: 50px; opacity: 0.6; animation: pulse 2s infinite;">↓</div>
        </div>
    </section>

    <!-- 2️⃣ GREETING -->
    <section class="section">
        <div class="container card fade-in">
            <h1 style="font-size: 2.2rem; margin-bottom: 15px;">Hey Farzana 🥺</h1>
            <p style="font-size: 1.2rem;">I made this because I miss you.</p>
            <div style="font-size: 2rem; margin-top: 15px;" class="pulse">💗</div>
        </div>
    </section>

    <!-- 3️⃣ QUESTION -->
    <section class="section" id="question">
        <div class="container card fade-in">
            <h2 style="font-size: 1.8rem; margin-bottom: 25px;">Will you be my<br>Valentine? ❤️</h2>
            <div class="btn-group">
                <button class="btn" onclick="unlockSite()">Yes 😚</button>
                <button class="btn secondary" onclick="unlockSite()">Always 💖</button>
            </div>
        </div>
    </section>

    <!-- HIDDEN CONTENT (Unlocks after Yes) -->
    <div id="hidden-content">
        
        <!-- 4️⃣ LDR MOMENTS -->
        <section class="section" style="padding-top: 4rem;">
            <div class="container">
                <h3 style="opacity: 0.6; margin-bottom: 20px;">US 💌</h3>
                <div class="chat-container">
                    <div class="bubble fade-in">Different places, same feelings 🌍</div>
                    <div class="bubble right fade-in">I still think of you every day 💭</div>
                    <div class="bubble fade-in">Distance didn't change how I feel...</div>
                    <div class="bubble right fade-in" style="font-weight: 600; color: var(--accent);">If anything, it made it stronger 💪</div>
                </div>
            </div>
        </section>

        <!-- 5️⃣ TIME & WAITING -->
        <section class="section">
            <div class="container fade-in">
                <div style="font-size: 3rem; margin-bottom: 20px;">⏳</div>
                <h2 style="font-size: 1.6rem;">Every day brings us closer.</h2>
                <p style="opacity: 0.7; margin-top: 10px;">Until we don't have to count anymore.</p>
            </div>
        </section>

        <!-- 6️⃣ LOVE METER -->
        <section class="section">
            <div class="container card fade-in">
                <h2 style="font-size: 1.5rem;">Fill the Heart</h2>
                <div class="tap-heart-btn" onclick="fillMeter(event)">💖</div>
                <div class="meter-wrapper">
                    <div class="meter-fill" id="love-bar"></div>
                </div>
                <p id="meter-text" style="margin-top: 15px; font-weight: 600; color: var(--accent);">Tap to send love</p>
            </div>
        </section>

        <!-- 7️⃣ REASSURANCE -->
        <section class="section">
            <div class="container fade-in" style="max-width: 600px;">
                <h1 style="font-size: 2rem; line-height: 1.6;">
                    I'm not going anywhere.<br>
                    You're not just a phase.<br>
                    <span style="color: var(--accent); background: white; padding: 0 10px; border-radius: 10px;">You're my choice.</span>
                </h1>
            </div>
        </section>

        <!-- 8️⃣ PRESENCE (DOTS) -->
        <section class="section">
            <div class="container fade-in">
                <div class="dots-container" id="dots-anim">
                    <div class="dot dot-left"></div>
                    <div class="merged-heart">❤️</div>
                    <div class="dot dot-right"></div>
                </div>
                <h2 style="margin-top: 30px;">Even from far away...</h2>
                <p>I'm still here.</p>
            </div>
        </section>

        <!-- 9️⃣ FINAL -->
        <section class="section" style="background: white; border-top-left-radius: 40px; border-top-right-radius: 40px; box-shadow: 0 -10px 40px rgba(0,0,0,0.05);">
            <div class="container fade-in">
                <h1 style="font-size: 3rem; color: var(--accent); margin-bottom: 20px;">Happy Valentine's<br>Day, Farzana ❤️</h1>
                <p style="font-size: 1.2rem; letter-spacing: 1px; opacity: 0.8;">Always yours.</p>
            </div>
        </section>

    </div>

    <script>
        // --- SCROLL ANIMATIONS ---
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    // Special trigger for dots
                    if(entry.target.querySelector('.dots-container')) {
                        entry.target.querySelector('.dots-container').classList.add('visible');
                    }
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

        // --- UNLOCK FUNCTION ---
        function unlockSite() {
            confetti({
                particleCount: 150,
                spread: 70,
                origin: { y: 0.6 },
                colors: ['#ff8fa3', '#9fa8da', '#ffffff']
            });

            const content = document.getElementById('hidden-content');
            content.style.display = 'block';
            
            setTimeout(() => {
                content.style.opacity = '1';
                // Trigger observers for new content
                document.querySelectorAll('#hidden-content .fade-in').forEach(el => observer.observe(el));
                
                // Smooth scroll
                content.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }, 100);
        }

        // --- LOVE METER ---
        let loveLevel = 0;
        const bar = document.getElementById('love-bar');
        const meterText = document.getElementById('meter-text');

        function fillMeter(e) {
            if (loveLevel >= 100) return;

            loveLevel += 15;
            if(loveLevel > 100) loveLevel = 100;
            
            bar.style.width = loveLevel + '%';
            
            // Floating mini heart effect
            const h = document.createElement('div');
            h.innerText = '💗';
            h.style.position = 'fixed';
            h.style.left = e.clientX + 'px';
            h.style.top = e.clientY + 'px';
            h.style.pointerEvents = 'none';
            h.style.animation = 'floatUp 1s forwards';
            document.body.appendChild(h);
            setTimeout(() => h.remove(), 1000);

            if (loveLevel === 100) {
                meterText.innerText = "My heart is full for you! ❤️";
                meterText.style.color = "#ff8fa3";
                confetti({ particleCount: 50, origin: { y: 0.7 } });
            }
        }

        // Add float animation dynamically
        const style = document.createElement('style');
        style.innerHTML = `
            @keyframes floatUp {
                0% { transform: translateY(0) scale(1); opacity: 1; }
                100% { transform: translateY(-60px) scale(1.5); opacity: 0; }
            }
        `;
        document.head.appendChild(style);

    </script>
</body>
</html>
