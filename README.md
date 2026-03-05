<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pérola Nails | Studio de Beleza</title>
    <style>
        /* Estilos Gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #fdf6f6;
            color: #333;
            line-height: 1.6;
        }

        /* Cabeçalho */
        header {
            background-color: #fff;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #d4a373;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        nav a {
            margin-left: 20px;
            text-decoration: none;
            color: #555;
            font-weight: 500;
            transition: 0.3s;
        }

        nav a:hover {
            color: #d4a373;
        }

        /* Banner Principal */
        .hero {
            height: 60vh;
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), 
                        url('https://images.unsplash.com/photo-1604654894610-df4906821603?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 { font-size: 3rem; margin-bottom: 10px; }
        .hero p { font-size: 1.2rem; margin-bottom: 20px; }

        .btn-agendar {
            background-color: #d4a373;
            color: white;
            padding: 12px 30px;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn-agendar:hover { background-color: #bc8a5f; }

        /* Seção Catálogo */
        .container { padding: 4rem 10%; }
        h2 { text-align: center; margin-bottom: 3rem; color: #d4a373; }

        .catalogo {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .card:hover { transform: translateY(-5px); }

        .card-img {
            height: 200px;
            background-color: #eee;
            background-size: cover;
            background-position: center;
        }

        .card-content { padding: 20px; }
        .card-content h3 { margin-bottom: 10px; color: #444; }
        .card-content p { font-size: 0.9rem; color: #777; margin-bottom: 15px; }
        .price { font-weight: bold; color: #d4a373; font-size: 1.1rem; }

        /* Rodapé */
        footer {
            background-color: #333;
            color: white;
            padding: 3rem 10% 1rem;
            text-align: center;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 2rem;
            text-align: left;
        }

        .footer-bottom { border-top: 1px solid #444; padding-top: 1rem; font-size: 0.8rem; }
    </style>
</head>
<body>

    <header>
        <div class="logo">Pérola Nails</div>
        <nav>
            <a href="#inicio">Início</a>
            <a href="#catalogo">Serviços</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <section class="hero" id="inicio">
        <h1>Sua autoestima em boas mãos</h1>
        <p>Especialista em alongamentos e nail art personalizada.</p>
        <a href="https://wa.me/5500000000000" class="btn-agendar">AGENDAR HORÁRIO</a>
    </section>

    <section class="container" id="catalogo">
        <h2>Nosso Catálogo</h2>
        <div class="catalogo">
            
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1519014816548-bf5fe059798b?auto=format&fit=crop&w=500&q=60');"></div>
                <div class="card-content">
                    <h3>Pé e Mão Simples</h3>
                    <p>Cutilagem completa e esmaltação com marcas premium.</p>
                    <span class="price">R$ 50,00</span>
                </div>
            </div>

            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1632345031435-8727f6897d53?auto=format&fit=crop&w=500&q=60');"></div>
                <div class="card-content">
                    <h3>Alongamento em Gel</h3>
                    <p>Técnica de extensão com acabamento natural e duradouro.</p>
                    <span class="price">R$ 150,00</span>
                </div>
            </div>

            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1600007183319-8a03422030d9?auto=format&fit=crop&w=500&q=60');"></div>
                <div class="card-content">
                    <h3>Banho de Gel</h3>
                    <p>Fortalecimento da unha natural com camada protetora de gel.</p>
                    <span class="price">R$ 90,00</span>
                </div>
            </div>

            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1522337660859-02fbefca4702?auto=format&fit=crop&w=500&q=60');"></div>
                <div class="card-content">
                    <h3>Nail Art (Design)</h3>
                    <p>Desenhos feitos à mão, pedrarias e encapsuladas (por unha).</p>
                    <span class="price">A partir de R$ 5,00</span>
                </div>
            </div>

        </div>
    </section>

    <footer id="contato">
        <div class="footer-grid">
            <div>
                <h3>Sobre Nós</h3>
                <p>Há 5 anos transformando olhares e elevando a confiança através do cuidado com as mãos.</p>
            </div>
            <div>
                <h3>Endereço</h3>
                <p>Rua das Flores, 123<br>Bairro Estética - Cidade/UF</p>
            </div>
            <div>
                <h3>Horários</h3>
                <p>Terça a Sábado: 09h às 19h</p>
            </div>
        </div>
        <div class="footer-bottom">
            &copy; 2024 Pérola Nails - Todos os direitos reservados.
        </div>
    </footer>

</body>
</html>
