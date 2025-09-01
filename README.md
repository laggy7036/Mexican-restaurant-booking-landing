# Mexican-restaurant-booking-landing
Initial mexican Resturant booking page, First ever coding project 

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>La Vida Mexicana - Authentic Cuisine</title>
  <style>
    :root{
      --red:#e63946;
      --sun:#f4a261;
      --green:#2a9d8f;
      --yellow:#f8c102;
      --ink:#fff;
    }

    body{
      margin:0;
      font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color:var(--ink);
      background:url('https://www.transparenttextures.com/patterns/mexican-fabric.png') repeat;
      background-color:#c0392b; /* fallback red */
      line-height:1.6;
    }

    h1,h2,h3{
      font-family:Georgia, 'Times New Roman', serif;
      text-transform:uppercase;
    }

    header{
      text-align:center;
      padding:40px 20px;
      background:rgba(0,0,0,0.4);
    }
    header h1{
      margin:0; font-size:2.8rem; color:var(--yellow);
    }
    header p{ margin:6px 0 0; font-size:1.2rem; color:var(--sun); }

    .divider{
      height:20px;
      background:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="120" height="20" viewBox="0 0 120 20"><path d="M0 10l10-10 10 10 10-10 10 10 10-10 10 10 10-10 10 10 10-10 10 10" fill="%23f8c102"/></svg>')
        repeat-x center/120px 20px;
      margin:30px 0;
    }

    .hero{
      text-align:center;
      padding:100px 20px;
      background:rgba(0,0,0,0.6);
    }
    .hero h2{ font-size:2.5rem; color:var(--yellow); }
    .hero p{ font-size:1.2rem; max-width:600px; margin:0 auto 30px; color:#fff; }
    .cta{
      background:linear-gradient(90deg,var(--red),var(--sun));
      color:#fff; border:none; border-radius:6px; padding:14px 28px;
      font-weight:bold; cursor:pointer; transition:.3s;
    }
    .cta:hover{ background:linear-gradient(90deg,var(--sun),var(--green)); }

    .experience{
      text-align:center;
      max-width:800px;
      margin:60px auto;
      padding:30px;
      background:rgba(0,0,0,0.5);
      border-radius:10px;
    }
    .experience h2{ color:var(--yellow); margin-bottom:15px; }

    .booking{
      max-width:500px;
      margin:80px auto;
      padding:30px;
      background:rgba(0,0,0,0.5);
      border-radius:10px;
      text-align:center;
    }
    .booking h2{ color:var(--sun); margin-bottom:20px; }

    form{ text-align:left; }
    label{ display:block; margin:10px 0 5px; font-weight:bold; }
    input,select{
      width:100%; padding:10px; margin-bottom:15px;
      border:none; border-radius:6px;
    }
    input[type="submit"]{
      background:linear-gradient(90deg,var(--red),var(--sun));
      color:#fff; font-weight:bold; border:none; cursor:pointer;
      transition:.3s;
    }
    input[type="submit"]:hover{
      background:linear-gradient(90deg,var(--sun),var(--green));
    }

    footer{
      text-align:center; padding:25px 20px;
      background:rgba(0,0,0,0.6);
    }
    footer p{ margin:0; font-size:0.95rem; color:var(--yellow); }
  </style>
</head>
<body>

<header>
  <h1>La Vida Mexicana</h1>
  <p>Authentic Tacos • Cervezas • Tradition</p>
</header>

<div class="hero">
  <h2>Experience Mexico in Every Bite</h2>
  <p>Tacos, Cervezas & memories you’ll never forget. Real masa, real fire, real flavors.</p>
  <button class="cta" onclick="document.getElementById('booking').scrollIntoView({behavior:'smooth'})">
    Reserve Your Table
  </button>
</div>

<div class="divider"></div>

<section class="experience">
  <h2>The Authentic Mexican Experience</h2>
  <p>
    From nixtamalized tortillas pressed to order, to wood-kissed meats and salsas,
    our cocina honors tradition with uncompromising craft. Our bar curates agave spirits and crisp cervezas.
  </p>
</section>

<div class="divider"></div>

<section id="booking" class="booking">
  <h2>Book a Table</h2>
  <form>
    <label for="name">Name</label>
    <input type="text" id="name" required />

    <label for="email">Email</label>
    <input type="email" id="email" required />

    <label for="phone">Phone Number</label>
    <input type="tel" id="phone" required />

    <label for="date">Date</label>
    <input type="date" id="date" required />

    <label for="time">Time</label>
    <input type="time" id="time" required />

    <label for="guests">Number of Guests</label>
    <select id="guests" required>
      <option value="">Select…</option>
      <option>1</option><option>2</option><option>3</option>
      <option>4</option><option>5</option><option>6+</option>
    </select>

    <input type="submit" value="Reserve Now"/>
  </form>
</section>

<footer>
  <p>&copy; 2025 La Vida Mexicana — Crafted with heart, spice & tradition</p>
</footer>
