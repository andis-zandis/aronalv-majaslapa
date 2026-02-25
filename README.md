<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arona Print | Poligrāfija</title>
    <!-- Clean, modern font -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --sage: #94a684;    /* The Green */
            --brown: #7c6a58;   /* The Brown */
            --beige: #f8f5f0;   /* Light Beige Background */
            --dark: #2d2a26;    /* Text color */
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body { 
            font-family: 'Montserrat', sans-serif; 
            background-color: var(--beige); 
            color: var(--dark); 
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px 10%;
            background: white;
        }

        .logo { font-size: 22px; font-weight: 700; letter-spacing: 1px; color: var(--dark); text-decoration: none; }
        .logo span { color: var(--sage); }

        nav ul { display: flex; list-style: none; gap: 30px; }
        nav ul li a { text-decoration: none; color: var(--dark); font-size: 14px; font-weight: 600; transition: 0.3s; }
        nav ul li a:hover { color: var(--sage); }

        /* Hero Section */
        .hero {
            display: flex;
            align-items: center;
            padding: 80px 10%;
            gap: 50px;
            background: white;
        }

        .hero-content { flex: 1; }
        .hero-content h1 { font-size: 50px; line-height: 1.1; margin-bottom: 20px; font-weight: 700; }
        .hero-content p { font-size: 18px; margin-bottom: 30px; color: #666; font-weight: 300; }

        .hero-image { 
            flex: 1.2; 
            height: 450px; 
            background-image: url('https://images.unsplash.com/photo-1563089145-599997674d42?auto=format&fit=crop&w=1200&q=80'); 
            background-size: cover;
            background-position: center;
            border-radius: 10px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .btn {
            background: var(--sage);
            color: white;
            padding: 18px 35px;
            text-decoration: none;
            font-weight: 600;
            border-radius: 5px;
            display: inline-block;
            transition: 0.3s;
        }
        .btn:hover { background: var(--brown); transform: translateY(-2px); }

        /* Services Section */
        .services {
            padding: 100px 10%;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
        }

        .card {
            background: white;
            padding: 40px;
            border-radius: 10px;
            border-bottom: 4px solid var(--beige);
            transition: 0.3s;
        }

        .card:hover { border-bottom-color: var(--sage); transform: translateY(-5px); }
        .card h3 { margin-bottom: 15px; font-size: 20px; }
        .card p { font-size: 15px; color: #777; }

        /* Contact Section */
        .contact {
            padding: 100px 10%;
            background: var(--beige);
            display: flex;
            gap: 100px;
        }

        .contact-info { flex: 1; }
        .contact-info h2 { font-size: 36px; margin-bottom: 30px; }
        .contact-info p { margin-bottom: 15px; font-size: 16px; }
        .contact-info strong { color: var(--brown); display: block; font-size: 12px; text-transform: uppercase; margin-bottom: 5px; }

        .contact-form { flex: 1; background: white; padding: 40px; border-radius: 10px; }
        input, textarea { width: 100%; padding: 15px; margin-bottom: 15px; border: 1px solid #eee; background: #fafafa; border-radius: 5px; }
        .submit-btn { background: var(--brown); color: white; border: none; padding: 15px; width: 100%; cursor: pointer; font-weight: 600; border-radius: 5px; }

        footer { padding: 50px; text-align: center; font-size: 14px; color: #999; }

        @media (max-width: 900px) {
            .hero, .services, .contact { flex-direction: column; grid-template-columns: 1fr; padding: 50px 5%; }
            .hero-content h1 { font-size: 36px; }
        }
    </style>
</head>
<body>

    <nav>
        <a href="#" class="logo">Arona<span>Print</span></a>
        <ul>
            <li><a href="#">Produkcija</a></li>
            <li><a href="#">Par mums</a></li>
            <li><a href="#">Kontakti</a></li>
        </ul>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>Kvalitatīva druka Jūsu biznesam.</h1>
            <p>Mēs nodrošinām pilna servisa poligrāfijas pakalpojumus, sākot no iepakojuma dizaina līdz lielformāta ofseta drukai.</p>
            <a href="#" class="btn">Saņemt piedāvājumu</a>
        </div>
        <div class="hero-image"></div>
    </header>

    <section class="services">
        <div class="card">
            <h3>Kartona stendi</h3>
            <p>Pielāgoti tirdzniecības vietu risinājumi, kas izceļ Jūsu produktu.</p>
        </div>
        <div class="card">
            <h3>Iepakojums</h3>
            <p>Izturīgas un estētiskas kartona kastes jebkura veida produkcijai.</p>
        </div>
        <div class="card">
            <h3>Ofseta druka</h3>
            <p>Augstākās kvalitātes druka lielām tirāžām, katalogiem un reklāmai.</p>
        </div>
    </section>

    <section class="contact">
        <div class="contact-info">
            <h2>Sazināsimies</h2>
            <p><strong>Adrese</strong> Celtnieku 5A, Olaine, LV-2114</p>
            <p><strong>Tālrunis</strong> (+371) 294-511-50</p>
            <p><strong>E-pasts</strong> info@arona.lv</p>
            <p><strong>Darba laiks</strong> P.-Pk. 9:00 - 17:30</p>
        </div>
        <div class="contact-form">
            <input type="text" placeholder="Jūsu vārds">
            <input type="email" placeholder="E-pasts">
            <textarea rows="4" placeholder="Kā mēs varam palīdzēt?"></textarea>
            <button class="submit-btn">Nosūtīt ziņu</button>
        </div>
    </section>

    <footer>
        &copy; 2025 ARONA PRINT | OLAINES POLIGRĀFIJAS FIRMA
    </footer>

</body>
</html>
