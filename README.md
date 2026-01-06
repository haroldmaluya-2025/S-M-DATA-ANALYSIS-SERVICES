<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>S & M Data Analysis Services</title>
<style>
:root{
  --primary:#00c6ff;
  --secondary:#f9ca24;
  --dark:#0b132b;
  --light:#ffffff;
  --glass:rgba(255,255,255,0.08);
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Segoe UI, Arial, sans-serif;
}

body{
  background:linear-gradient(135deg,#1d2671,#cb446f);
  color:white;
  scroll-behavior:smooth;
}

/* HEADER */
header{
  position:sticky;
  top:0;
  z-index:1000;
  background:rgba(150, 37, 167, 0.6);
  backdrop-filter:blur(10px);
  padding:15px 40px;
  display:flex;
  justify-content:space-between;
  align-items:center;
}

.logo{
  display:flex;
  align-items:center;
  gap:15px;
}

.logo img{
  height:80px;
}

.logo span{
  font-size:30px;
  font-weight:bold;
}

nav a{
  color:white;
  text-decoration:none;
  margin-left:25px;
  font-size:16px;
}

nav a:hover{
  color:var(--secondary);
}

/* HERO */
.hero{
  min-height:10vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  padding:1px;
}

.hero h1{
  font-size:30px;
  margin-bottom:10px;
  animation:fadeUp 1s ease;
}

.hero p{
  font-size:15px;
  max-width:75x;
  margin:auto;
  line-height:1.7;
  animation:fadeUp 1.5s ease;
}

.hero button{
  margin-top:30px;
  padding:10px 40px;
  font-size:16px;
  border:none;
  border-radius:40px;
  background:var(--secondary);
  cursor:pointer;
  animation:fadeUp 1s ease;
}

.hero button:hover{
  background:#ffd32a;
}

/* SECTIONS */
section{
  padding:100px 20px;
}

h2{
  text-align:center;
  margin-bottom:50px;
  font-size:34px;
}

/* SERVICES */
.services{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:30px;
  max-width:1100px;
  margin:auto;
}

.card{
  background:var(--glass);
  padding:30px;
  border-radius:18px;
  text-align:center;
  transition:transform .2s;
}

.card:hover{
  transform:translateY(-8px);
}

.card h3{
  color:var(--secondary);
  margin-bottom:30px;
}

/* GET STARTED BUTTON */
.get-started-wrap {
  text-align: center;
  margin-top: 40px;
}

.get-started-btn {
  background: #f9ca24;
  padding: 14px 40px;
  border-radius: 30px;
  font-weight: bold;
  text-decoration: none;
  color: #000;
}

/* PRICING SECTION */
.pricing-section {
  padding: 100px 20px;
  text-align: center;
  background: linear-gradient(135deg, #2c2f8f, #7b2f6b);
  color: #fff;
}

.pricing-sub {
  margin-bottom: 50px;
  opacity: 0.9;
}

.pricing-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 30px;
  max-width: 1100px;
  margin: auto;
}

.pricing-card {
  background: rgba(255,255,255,0.12);
  padding: 35px;
  border-radius: 20px;
  backdrop-filter: blur(10px);
}

.pricing-card h3 {
  font-size: 24px;
  margin-bottom: 10px;
}

.price {
  font-size: 32px;
  font-weight: bold;
  color: #f9ca24;
}

.tag {
  margin-bottom: 20px;
  opacity: 0.9;
}

.pricing-card ul {
  list-style: none;
  padding: 0;
  margin-bottom: 30px;
}

.pricing-card ul li {
  margin: 10px 0;
}

.pricing-btn {
  display: inline-block;
  padding: 12px 28px;
  background: #f9ca24;
  border-radius: 25px;
  color: #000;
  text-decoration: none;
  font-weight: bold;
}
.gcash-section {
  padding: 80px 20px;
  text-align: center;
  background: linear-gradient(135deg, #3a2d8f, #8e3c6d);
  animation: fadeUp 1s ease;
}

.gcash-card {
  max-width: 420px;
  margin: 30px auto;
  padding: 30px;
  background: rgba(255,255,255,0.15);
  border-radius: 20px;
  backdrop-filter: blur(10px);
  animation: glow 2.5s infinite;
}

.gcash-number {
  display: inline-block;
  margin: 10px 0;
  font-size: 1.6rem;
  font-weight: bold;
  color: #ffd43b;
  text-decoration: none;
}

@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes glow {
  0% { box-shadow: 0 0 0 rgba(255,212,59,0.4); }
  50% { box-shadow: 0 0 35px rgba(255,212,59,0.9); }
  100% { box-shadow: 0 0 0 rgba(255,212,59,0.4); }
}

html {
  scroll-behavior: smooth;
}

/* POPULAR CARD */
.popular {
  border: 2px solid #f9ca24;
  transform: scale(1.05);
}

.badge {
  display: inline-block;
  background: #f9ca24;
  color: #000;
  padding: 6px 14px;
  border-radius: 20px;
  font-size: 12px;
  margin-bottom: 10px;
}

/* ABOUT */
/* ABOUT SECTION – ANIMATED BACKGROUND */
.about-animated {
  position: relative;
  padding: 120px 20px;
  overflow: hidden;
  background: linear-gradient(
    120deg,
    #2e2a7b,
    #6a3f8c,
    #b0426b
  );
  background-size: 300% 300%;
  animation: gradientMove 12s ease infinite;
  color: #fff;
}

/* Floating glow overlay */
.about-animated::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(
    circle,
    rgba(255,255,255,0.12) 0%,
    rgba(255,255,255,0.03) 40%,
    transparent 70%
  );
  animation: glowFloat 18s linear infinite;
}

/* Content animation */
.about-content {
  position: relative;
  max-width: 1000px;
  margin: auto;
  text-align: center;
  animation: fadeUp 1.4s ease forwards;
}

.about-content h2 {
  font-size: 42px;
  margin-bottom: 25px;
}

.about-content p {
  font-size: 18px;
  line-height: 1.8;
  opacity: 0.95;
}

/* KEYFRAMES */
@keyframes gradientMove {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

@keyframes glowFloat {
  0% { transform: translate(0, 0); }
  50% { transform: translate(40px, 40px); }
  100% { transform: translate(0, 0); }
}

@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
/* === ANIMATED AUTOMATION BACKGROUND === */

#contact {
  position: relative;
  padding: px 10px;
  text-align: center;
  color: #fff;
  background: linear-gradient(135deg, #3d41b6, #a31484);
  overflow: auto;
}

/* Moving grid */


/* Floating light waves */
#contact::after {
  content: "";
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 30% 40%, rgba(255,255,255,0.18), transparent 45%),
    radial-gradient(circle at 70% 60%, rgba(255,255,255,0.15), transparent 50%);
  animation: glowMove 18s ease-in-out infinite alternate;
}

/* Keep content above animation */
#contact > * {
  position: relative;
  z-index: 1;
}

/* Animations */
@keyframes gridMove {
  from {
    background-position: 0 0;
  }
  to {
    background-position: 600px 600px;
  }
}

@keyframes glowMove {
  from {
    transform: translateY(-20px);
  }
  to {
    transform: translateY(20px);
  }
}
#contact form {
  max-width: 500px;
  margin: auto;
}
#contact input,
#contact textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border-radius: 8px;
  border: 1px solid #ccc;
}

#contact button {
  background: #f9ca24;
  border: none;
  padding: 12px 30px;
  border-radius: 10px;
  font-weight: bold;
  cursor: pointer;
}
form{
  background:var(--glass);
  padding:20px;
  border-radius:10px;
}

input, textarea{
  width:100%;
  padding:110px;
  margin-bottom:15px;
  border:none;
  border-radius:10px;
}

form button{
  width:50%;
  padding:10px;
  border:none;
  border-radius:20px;
  background:var(--secondary);
  font-size:20px;
}

.info{
  line-height:2;
}

iframe{
  width:50%;
  height:300px;
  border-radius:20px;
  margin-top:10px;
  border:none;
}

/* FOOTER */
footer{
  background:#000;
  padding:20px;
  text-align:center;
  font-size:14px;
}

/* ANIMATION */
@keyframes fadeUp{
  from{opacity:0; transform:translateY(30px);}
  to{opacity:1; transform:translateY(0);}
}

/* MOBILE */
@media(max-width:800px){
  header{
    flex-direction:column;
    gap:15px;
  }
  nav{
    display:flex;
    gap:15px;
  }
  .hero h1{
    font-size:34px;
  }
  .contact{
    grid-template-columns:1fr;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">
    <img src="logo.png.png" alt="S & M Data Analysis Services">
    <span>S & M DATA ANALYSIS SERVICES</span>
  </div>
  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero" id="home">
  <div>
    <img src="logo.png.png" >
    <h1>Expert Data Solutions for Smarter Decisions</h1>
    <p>
      S AND M Data Analysis Services is a Cebu-based Filipino sole proprietorship
      delivering software development, automation, and geographical data solutions
      that empower organizations through data-driven insights.
    </p>
    <button onclick="document.getElementById('contact').scrollIntoView()">Contact Us</button>
  </div>
</section>

<section id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div class="card">
      <h3>Software Development</h3>
      <p>Custom business systems and applications tailored to your needs.</p>
    </div>
    <div class="card">
      <h3>Data Analysis</h3>
      <p>Transforming raw data into meaningful insights.</p>
    </div>
    <div class="card">
      <h3>Geographical Data Solutions</h3>
      <p>GIS mapping, spatial analysis, and location intelligence.</p>
    </div>
    <div class="card">
      <h3>Automation & Manufacturing Support</h3>
      <p>Digital tools to improve productivity and operational efficiency.</p>
</div>


</section>
<section id="pricing" class="pricing-section">

  <h2>Our Packages</h2>
  <p class="pricing-sub">Choose the plan that fits your needs</p>

  <div class="pricing-grid">
 <!-- STARTED -->
    <div class="pricing-card">
      <h3>Started</h3>
      <p class="price">PHP 99</p>
      <p class="tag">Ideal for Beginners</p>
      <ul>
        <li>✔ Basic website setup</li>
        <li>✔ Simple contact form</li>
        <li>✔ Mobile-friendly design</li>
        <li>✔ Email support</li>
      </ul>
      <a href="#gcash-payment" class="pricing-btn">Choose Started</a>
    </div>
    <!-- PLUS -->
    <div class="pricing-card">
      <h3>Plus</h3>
      <p class="price">PHP 299</p>
      <p class="tag">Best for Average Users</p>
      <ul>
        <li>✔ Everything in Started</li>
        <li>✔ Data analysis setup</li>
        <li>✔ Google Maps integration</li>
        <li>✔ Priority support</li>
      </ul>
  <a href="#gcash-payment" class="pricing-btn">Choose Plus</a>
    </div>
    <!--TURBO -->
    <div class="pricing-card popular">
      <span class="badge">Most Popular</span>
      <h3>Turbo</h3>
      <p class="price">PHP 499</p>
      <p class="tag">Best Value Package</p>
      <ul>
  <li>✔ Everything in Plus</li>
  <li>✔ Automation tools</li>
 <li>✔ Advanced analytics</li>
  <li>✔ Priority + consultation</li>
</ul>
   <a href="#gcash-payment" class="pricing-btn">Choose Turbo</a>
    </div>
  </div>
</section>
<section id="gcash-payment" class="gcash-section">
  <h2>Pay via GCash</h2>
  <p class="gcash-amount">Selected Package</p>

  <div class="gcash-card">
    <p><strong>GCash Number</strong></p>
    <a href="tel:09639025445" class="gcash-number">
      0963 902 5445
    </a>
<p><strong>Account Name</strong></p>
<p>Ryu Samryoung</p>
<p class="note">
 Please send the exact amount and include your name in the message.
</p>
</div>
</section>
<section id="about" class="about-animated">
  <div class="about-content">
    <h2>About Us</h2>
    <p>
      Based in Agujo, Daanbantayan, Cebu, S AND M Data Analysis Services
      is committed to innovation, quality, and continuous improvement.
      We support businesses and communities by providing reliable,
      modern, and efficient digital solutions that drive sustainable growth.
    </p>
  </div>
</section>
<section id="contact">
  <h2>Contact Us</h2>
  <p>Send us a message and it will go directly to our Gmail.</p>
  <form action="https://formspree.io/f/meeowwbq" method="POST">
   <input
      type="text"
      name="name"
      placeholder="Your Name"
      required >
    <input 
      type="email"
      name="email"
      placeholder="Your Email"
      required>
<textarea
name="message"
placeholder="Your Message"
rows="5"
required
  ></textarea>
  <input type="hidden" name="_subject" value="New Contact Message - S & M Data Analysis Services">
   <button type="submit">Send Message</button>
  </form>
  <div class="info">
      <p><strong>Email:</strong> silverism777@gmail.com</p>
      <p><strong>Business Representate:</strong> Mr. Ryu Samryoung</p>
      <p><strong>Location:</strong> Agujo, Daanbantayan, Cebu, Philippines</p>
<div style="margin-bottom:15px;">
  <h3 style="margin:0;">S & M Data Analysis Services</h3>
  <p style="margin:5px 0;">
    Agujo, Daanbantayan, Cebu, Philippines
  </p>
</div>
<iframe src="https://www.google.com/maps/embed?pb=!1m17!1m12!1m3!1d1196.4089309342678!2d124.01143959958202!3d11.267337977505433!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m2!1m1!2zMTHCsDE2JzAyLjMiTiAxMjTCsDAwJzQyLjIiRQ!5e1!3m2!1sen!2sph!4v1767662167201!5m2!1sen!2sph" 
width="600" 
height="450" 
style="border:0;" 
allowfullscreen="" 
loading="lazy" 
referrerpolicy="no-referrer-when-downgrade">
</iframe>
    </div>
  </div>
</section>
<footer>
  © 2025 S & M Data Analysis Services | Cebu, Philippines
</footer>
</body>
</html>
