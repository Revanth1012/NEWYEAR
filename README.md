<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>NYE 2025 | Venigallas Nandanavanam</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Montserrat:wght@300;600&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            background: #050505;
            /* New Year Theme: Dark sky with shimmering gold stardust */
            background-image:
                radial-gradient(circle at 50% 50%, rgba(60, 45, 10, 0.4) 0%, transparent 80%),
                url('https://www.transparenttextures.com/patterns/stardust.png');
            color: white;
            font-family: 'Montserrat', sans-serif;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            text-align: center;
        }

        /* Gold Sparkle Animation */
        .spark {
            position: absolute;
            background: linear-gradient(#D4AF37, #FBF5B7);
            border-radius: 50%;
            pointer-events: none;
            animation: floatUp linear infinite;
        }

        @keyframes floatUp {
            0% { transform: translateY(110vh) scale(0); opacity: 0; }
            50% { opacity: 1; }
            100% { transform: translateY(-10vh) scale(1); opacity: 0; }
        }

        .invite-card {
            width: 88%;
            padding: 40px 20px;
            border: 1px solid rgba(212, 175, 55, 0.4);
            background: rgba(10, 10, 10, 0.7);
            backdrop-filter: blur(15px);
            border-radius: 30px;
            box-shadow: 0 0 50px rgba(0,0,0,1);
            position: relative;
            z-index: 10;
        }

        .label {
            font-size: 0.65rem;
            letter-spacing: 6px;
            color: #D4AF37;
            text-transform: uppercase;
            margin-bottom: 15px;
        }

        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 1.6rem;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        .main-title {
            font-size: 3.2rem;
            font-weight: 900;
            line-height: 1;
            margin: 15px 0;
            background: linear-gradient(135deg, #D4AF37 0%, #FBF5B7 50%, #AA771C 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }

        .event-details {
            font-size: 0.85rem;
            font-weight: 600;
            color: #eee;
            margin-bottom: 25px;
            letter-spacing: 1px;
        }

        .highlights {
            list-style: none;
            margin: 20px 0;
            padding: 20px 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .highlights li {
            font-size: 0.9rem;
            margin: 12px 0;
            font-weight: 300;
            letter-spacing: 2px;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .highlights li span {
            color: #D4AF37;
        }

        .btn-location {
            background: transparent;
            color: #D4AF37;
            border: 1px solid #D4AF37;
            padding: 14px 25px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.75rem;
            border-radius: 5px;
            display: inline-block;
            margin-top: 15px;
            transition: 0.3s;
            letter-spacing: 2px;
        }

        .footer {
            margin-top: 30px;
            font-size: 0.55rem;
            letter-spacing: 3px;
            opacity: 0.4;
            text-transform: uppercase;
        }
    </style>
</head>
<body>

    <div class="invite-card">
        <p class="label">New Year Celebration</p>
        <h1>Venigallas Nandanavanam</h1>
        <div class="main-title">2025</div>
       
        <p class="event-details">JOGIPET | DEC 31ST | 8:00 PM</p>

        <ul class="highlights">
            <li><span>✦</span> THAMBOLA NIGHT <span>✦</span></li>
            <li><span>✦</span> CLASSIC CARD GAMES <span>✦</span></li>
            <li><span>✦</span> BONFIRE <span>✦</span></li>
            <li><span>✦</span> COCKTAILS <span>✦</span></li>
            <li><span>✦</span> GRAND FARM DINNER <span>✦</span></li>
        </ul>

        <a href="https://maps.app.goo.gl/xLLmy5TMNxwEMMMM7" target="_blank" class="btn-location">NAVIGATE TO FARMHOUSE</a>

    </div>

    <script>
        function createSpark() {
            const spark = document.createElement('div');
            spark.className = 'spark';
            const size = Math.random() * 3 + 1 + 'px';
            spark.style.width = size;
            spark.style.height = size;
            spark.style.left = Math.random() * 100 + 'vw';
            spark.style.animationDuration = Math.random() * 2 + 3 + 's';
            document.body.appendChild(spark);
            setTimeout(() => spark.remove(), 5000);
        }
        setInterval(createSpark, 150);
    </script>

</body>
</html>
