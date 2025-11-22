    <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Iron Pulse Gym</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#ff6b6b;
      --dark:#0f1724;
      --muted:#667085;
      --card:#0b1220;
      --glass: rgba(255,255,255,0.04);
      --radius:12px;
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,#071225 0%, #071826 100%);color:#e6eef8;line-height:1.45}
    .container{max-width:1100px;margin:0 auto;padding:28px}

    /* navbar */
    header{backdrop-filter: blur(6px);}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 0}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#ff9a6b);display:flex;align-items:center;justify-content:center;font-weight:700;color:#111}
    nav ul{display:flex;gap:18px;list-style:none;margin:0;padding:0}
    nav a{color:var(--muted);text-decoration:none;font-weight:500}
    .cta{background:var(--accent);color:#081018;padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:700}

    /* hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:32px;align-items:center;padding:56px 0}
    .hero h1{font-size:34px;margin:0 0 10px;color:#fff}
    .hero p{color:var(--muted);margin:0 0 20px}
    .hero .actions{display:flex;gap:12px}
    .btn{padding:12px 18px;border-radius:10px;text-decoration:none;font-weight:600}
    .btn-primary{background:var(--accent);color:#081018}
    .btn-outline{border:1px solid rgba(255,255,255,0.06);color:var(--muted)}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:14px;border:1px solid rgba(255,255,255,0.03)}

    /* features */
    .features{display:flex;gap:12px;margin-top:18px}
    .feature{flex:1;padding:12px;border-radius:10px;background:var(--glass);text-align:center}
    .feature strong{display:block;font-size:18px;color:#fff}
    .feature span{color:var(--muted);font-size:14px}

    /* classes & pricing */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin:36px 0}
    .class-card{background:linear-gradient(180deg,#071525 0%, #081827 100%);padding:18px;border-radius:14px;border:1px solid rgba(255,255,255,0.03)}
    .class-card h3{margin:0 0 8px}
    .price{font-weight:700;color:var(--accent)}

    /* testimonials */
    .testimonials{display:flex;gap:12px}
    .testimonial{flex:1;background:var(--card);padding:16px;border-radius:12px}

    /* contact */
    form{display:grid;gap:10px}
    input,textarea,select{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:12px;border-radius:8px;color:#e6eef8}
    input::placeholder{color:rgba(230,238,248,0.4)}
    .footer{margin-top:44px;padding:18px 0;border-top:1px solid rgba(255,255,255,0.03);color:var(--muted)}

    @media(max-width:880px){
      .hero{grid-template-columns:1fr;}
      .grid{grid-template-columns:repeat(2,1fr)}
    }
    @media(max-width:560px){
      nav ul{display:none}
      .grid{grid-template-columns:1fr}
      .container{padding:18px}
      .logo{width:40px;height:40px}
      .hero h1{font-size:26px}
    }

  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo">IP</div>
        <div>
          <div style="font-weight:700">Iron Pulse Gym</div>
          <div style="font-size:12px;color:var(--muted)">Strength • Conditioning • Community</div>
        </div>
      </div>
      <nav>
        <ul>
          <li><a href="#classes">Classes</a></li>
          <li><a href="#trainers">Trainers</a></li>
          <li><a href="#pricing">Pricing</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <a class="cta" href="#pricing">Start Free Trial</a>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div>
        <h1>Build strength. Move better. Feel unstoppable.</h1>
        <p>Join Iron Pulse — a modern training space focused on strength, mobility, and results. Programs for beginners to advanced athletes, friendly community, and certified coaches.</p>
        <div class="actions">
          <a class="btn btn-primary" href="#contact">Book Trial</a>
          <a class="btn btn-outline" href="#classes">View Classes</a>
        </div>

        <div class="card" style="margin-top:18px;max-width:620px">
          <div class="features">
            <div class="feature"><strong>100+</strong><span>Machines & equipment</span></div>
            <div class="feature"><strong>Certified</strong><span>Coaches & trainers</span></div>
            <div class="feature"><strong>Flexible</strong><span>Timings & plans</span></div>
          </div>
        </div>
      </div>

      <aside class="card">
        <div style="height:220px;border-radius:10px;background:linear-gradient(135deg,#10223a,#0b2b43);display:flex;align-items:center;justify-content:center;font-size:22px;color:var(--muted)">Hero image</div>
        <div style="display:flex;justify-content:space-between;margin-top:14px;align-items:center">
          <div>
            <div style="font-size:12px;color:var(--muted)">Next Class</div>
            <div style="font-weight:700">Strength & Conditioning — 6:30 PM</div>
          </div>
          <a class="btn btn-primary" href="#signup">Join</a>
        </div>
      </aside>
    </section>

    <section id="classes">
      <h2 style="margin:0 0 12px">Popular Classes</h2>
      <div class="grid">
        <div class="class-card">
          <h3>Strength Training</h3>
          <p style="color:var(--muted);margin:6px 0">Barbell programming, technique work, progressive overload for gains.</p>
          <div class="price">₹1500 / month</div>
        </div>
        <div class="class-card">
          <h3>Functional Fitness</h3>
          <p style="color:var(--muted);margin:6px 0">Metabolic conditioning, bodyweight skills, mobility flow.</p>
          <div class="price">₹1300 / month</div>
        </div>
        <div class="class-card">
          <h3>Personal Training</h3>
          <p style="color:var(--muted);margin:6px 0">1-on-1 coaching, personalized plans, fast progress.</p>
          <div class="price">₹2500 / month</div>
        </div>
      </div>
    </section>

    <section id="trainers">
      <h2 style="margin:0 0 12px">Meet Our Trainers</h2>
      <div class="testimonials">
        <div class="testimonial">
          <strong>Rohit Kumar</strong>
          <div style="font-size:13px;color:var(--muted);margin:6px 0">Head Coach — Strength & Power</div>
          <p style="margin:0;color:var(--muted)">10+ years coaching experience with focus on safe technique and athletic performance.</p>
        </div>
        <div class="testimonial">
          <strong>Asha Verma</strong>
          <div style="font-size:13px;color:var(--muted);margin:6px 0">Functional & Mobility Coach</div>
          <p style="margin:0;color:var(--muted)">Specialist in movement quality, corrective exercise, and injury prevention.</p>
        </div>
      </div>
    </section>

    <section id="pricing" style="margin-top:28px">
      <h2 style="margin:0 0 12px">Pricing Plans</h2>
      <div class="grid">
        <div class="class-card">
          <h3>Basic</h3>
          <p style="color:var(--muted);margin:6px 0">Access to gym floor & equipment</p>
          <div class="price">₹999 / month</div>
        </div>
        <div class="class-card">
          <h3>Standard</h3>
          <p style="color:var(--muted);margin:6px 0">Includes group classes & open gym</p>
          <div class="price">₹1499 / month</div>
        </div>
        <div class="class-card">
          <h3>Pro</h3>
          <p style="color:var(--muted);margin:6px 0">Includes 1 personal session / week</p>
          <div class="price">₹2499 / month</div>
        </div>
      </div>
    </section>

    <section id="contact" style="margin-top:28px">
      <h2 style="margin:0 0 12px">Contact & Signup</h2>
      <div class="card">
        <form action="#" onsubmit="event.preventDefault();alert('Thanks! We will contact you.')">
          <div style="display:flex;gap:10px">
            <input type="text" placeholder="Full name" style="flex:1" required>
            <input type="email" placeholder="Email" style="flex:1" value="sukhpreet3258@gmail.com">
          </div>
          <input type="text" placeholder="Phone (optional)">
          <select>
            <option>Interested in: Basic</option>
            <option>Standard</option>
            <option>Pro</option>
          </select>
          <textarea rows="4" placeholder="Message (goals, experience)"></textarea>
          <div style="display:flex;gap:10px;justify-content:flex-end">
            <button class="btn btn-outline" type="reset">Reset</button>
            <button class="btn btn-primary" type="submit">Send Request</button>
          </div>
        </form>
      </div>
    </section>

    <footer class="footer">
      <div style="display:flex;justify-content:space-between;align-items:center;gap:18px;flex-wrap:wrap">
        <div>© 2025 Iron Pulse Gym — Designed with ❤️</div>
        <div style="color:var(--muted)">Address: Jamshedpur • Phone: +91-XXXXXXXXXX</div>
      </div>
    </footer>
  </main>

</body>
</html>
