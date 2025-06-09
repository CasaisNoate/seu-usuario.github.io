<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minhas Redes Sociais</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #001510);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            padding: 20px;
        }
        
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            width: 100%;
            max-width: 500px;
            text-align: center;
        }
        
        .profile {
            margin-bottom: 30px;
            animation: fadeIn 1s ease-out;
        }
        
        .profile img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid rgba(255, 255, 255, 0.3);
            object-fit: cover;
            margin-bottom: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .profile h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }
        
        .profile p {
            font-size: 1.1rem;
            opacity: 0.9;
            max-width: 80%;
            margin: 0 auto;
        }
        
        .links {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .link-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 18px;
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            animation: slideUp 0.5s ease-out;
            animation-fill-mode: both;
        }
        
        .link-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.15);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
        }
        
        .link-card i {
            font-size: 2.5rem;
            width: 60px;
            text-align: center;
            margin-right: 20px;
        }
        
        .link-content {
            text-align: left;
            flex-grow: 1;
        }
        
        .link-content h2 {
            font-size: 1.4rem;
            margin-bottom: 5px;
        }
        
        .link-content p {
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .link-card:nth-child(1) { animation-delay: 0.2s; }
        .link-card:nth-child(2) { animation-delay: 0.4s; }
        .link-card:nth-child(3) { animation-delay: 0.6s; }
        .link-card:nth-child(4) { animation-delay: 0.8s; }
        
        .youtube { color: #FF0000; }
        .twitch { color: #9146FF; }
        .instagram { 
            background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .discord { color: #5865F2; }
        
        footer {
            margin-top: 20px;
            font-size: 0.9rem;
            opacity: 0.7;
            animation: fadeIn 2s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { 
                opacity: 0;
                transform: translateY(30px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @media (max-width: 600px) {
            .profile img {
                width: 120px;
                height: 120px;
            }
            
            .profile h1 {
                font-size: 2rem;
            }
            
            .link-card i {
                font-size: 2rem;
            }
            
            .link-content h2 {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="profile">
            <img src="https://s10.aconvert.com/convert/p3r68-cdx67/adrxw-8c6d8.png">
            <h1>Minhas Redes</h1>
            <p>Conecte-se comigo através das minhas plataformas preferidas</p>
        </div>
        
        <div class="links">
            <a href="https://www.youtube.com/@Casais_2023" target="_blank" class="link-card">
                <i class="fab fa-youtube youtube"></i>
                <div class="link-content">
                    <h2>YouTube</h2>
                    <p>Assista meus vídeos e tutoriais</p>
                </div>
            </a>
            
            <a href="https://www.twitch.tv/casais2023" target="_blank" class="link-card">
                <i class="fab fa-twitch twitch"></i>
                <div class="link-content">
                    <h2>Twitch</h2>
                    <p>Me acompanhe nas minhas lives</p>
                </div>
            </a>
            
            <a href="https://www.instagram.com/francisco_casais15/profilecard/?igsh=Nm12cWR3ZGNrYnNo" target="_blank" class="link-card">
                <i class="fab fa-instagram instagram"></i>
                <div class="link-content">
                    <h2>Instagram</h2>
                    <p>Fotos e stories do meu dia a dia</p>
                </div>
            </a>
            
            <a href="https://discord.gg/xh6SfDmBnx" target="_blank" class="link-card">
                <i class="fab fa-discord discord"></i>
                <div class="link-content">
                    <h2>Discord</h2>
                    <p>Entre na minha comunidade</p>
                </div>
            </a>
        </div>
        
        <footer>
            © 2023 Minhas Redes Sociais - Conecte-se comigo
        </footer>
    </div>
</body>
</html>
