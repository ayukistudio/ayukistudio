<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AyukiDev | @AyukiDev</title>
    <style>
        :root {
            --primary: #6200EE;
            --secondary: #03DAC6;
            --background: #F2F2F7;
            --card: #FFFFFF;
            --text: #1C1C1E;
            --accent: #FF375F;
        }

        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            background: var(--background);
            color: var(--text);
            line-height: 1.6;
        }

        .glass {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 16px;
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.1);
        }

        .gradient-text {
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }

        .chip {
            display: inline-flex;
            align-items: center;
            background: var(--secondary);
            color: #000;
            padding: 4px 12px;
            border-radius: 100px;
            margin: 4px;
            font-size: 14px;
            font-weight: 500;
        }

        .pulse-button {
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 var(--accent); }
            70% { box-shadow: 0 0 0 10px rgba(0,0,0,0); }
            100% { box-shadow: 0 0 0 0 rgba(0,0,0,0); }
        }

        .coffee-animation {
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 16px;
        }

        .icon {
            width: 20px;
            height: 20px;
            vertical-align: middle;
            margin-right: 8px;
        }

        @media (max-width: 600px) {
            .glass {
                border-radius: 0;
            }
        }
    </style>
</head>
<body>
    <div style="padding: 40px; max-width: 800px; margin: auto;">
        <!-- Hero Section -->
        <div class="glass" style="padding: 32px; position: relative;">
            <div style="position: absolute; top: 10px; right: 10px; animation: float 5s ease-in-out infinite;">
                ☕
            </div>
            <h1 class="gradient-text" style="font-size: 2.5em; margin: 0;">Александр Егоренко</h1>
            <p style="margin: 8px 0;">@AyukiDev • Будущий ИИ инженер</p>
            <p style="margin: 8px 0; color: #888;">Ростов-на-Дону 🌆</p>
            <div style="margin-top: 24px;">
                <span class="chip">C#</span>
                <span class="chip">Python</span>
                <span class="chip">C</span>
                <span class="chip">VB.NET</span>
            </div>
        </div>

        <!-- About Section -->
        <div class="glass" style="margin-top: 24px; padding: 24px;">
            <h2 style="color: var(--primary); margin-top: 0;">О себе</h2>
            <p>☕ Зависимый от кофеина</p>
            <p>🤖 Мечтаю создавать интеллектуальные системы будущего</p>
            <p>🕹️ Тотемное животное: anykey’щик</p>
        </div>

        <!-- Projects Section -->
        <div class="glass" style="margin-top: 24px; padding: 24px;">
            <h2 style="color: var(--primary);">Проекты</h2>
            <div class="grid">
                <a href="https://ayukidev.pages.dev/" target="_blank" class="pulse-button" style="display: inline-block; padding: 12px 24px; background: var(--primary); color: white; text-decoration: none; border-radius: 8px;">
                    🌐 Персональный сайт
                </a>
                <a href="https://t.me/AyukiDev" target="_blank" style="display: inline-block; padding: 12px 24px; background: var(--secondary); color: #000; text-decoration: none; border-radius: 8px;">
                    💬 Telegram
                </a>
            </div>
        </div>

        <!-- Footer -->
        <div style="text-align: center; margin-top: 32px; color: #888; font-size: 0.9em;">
            <p>© 2023 AyukiDev | Сделано с ❤️ и 300% кофе</p>
        </div>
    </div>
</body>
</html>
