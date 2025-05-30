<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NoteBazaar - Buy & Sell School Notes</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fdf5e6;
      color: #111;
    }
    header {
      background-color: #000;
      color: #fdf5e6;
      padding: 1em 2em;
      text-align: center;
    }
    nav {
      background-color: #111;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav a {
      color: #fdf5e6;
      padding: 14px 20px;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #fdf5e6;
      color: #111;
    }
    .section {
      padding: 2em;
    }
    .course-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 1em;
      padding: 2em 0;
    }
    .course-box {
      background: #111;
      color: #fdf5e6;
      padding: 1em;
      border-radius: 10px;
      text-align: center;
      cursor: pointer;
      transition: 0.3s;
    }
    .course-box:hover {
      background: #333;
    }
    .notes {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1em;
    }
    .note-card {
      background-color: #fff;
      padding: 1em;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    form {
      background: #fff;
      padding: 2em;
      border-radius: 8px;
      max-width: 600px;
      margin: auto;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    input, textarea, select {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      background-color: #111;
      color: #fdf5e6;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #444;
    }
    .add-notes-btn {
      display: block;
      margin: 3em auto 1em;
      background-color: #fdf5e6;
      color: #111;
      font-weight: bold;
      font-size: 1.2em;
      padding: 15px 30px;
      border-radius: 50px;
      border: 2px solid #111;
      cursor: pointer;
      transition: 0.3s;
    }
    .add-notes-btn:hover {
      background-color: #111;
      color: #fdf5e6;
    }
    footer {
      background: #000;
      color: #fdf5e6;
      text-align: center;
      padding: 1em;
    }
  </style>
</head>
<body>
  <header>
    <h1>NoteBazaar</h1>
    <p>Buy and Sell School Notes and Projects</p>
  </header>  <nav>
    <a href="#home">Home</a>
    <a href="#browse">Browse Notes</a>
    <a href="#sell">Sell/Donate Notes</a>
    <a href="#profile">Profile</a>
    <a href="#contact">Contact</a>
  </nav>  <section id="home" class="section">
    <h2>Choose Your Course</h2>
    <div class="course-grid">
      <div class="course-box" onclick="location.href='#browse'">Class 10</div>
      <div class="course-box" onclick="location.href='#browse'">Class 11</div>
      <div class="course-box" onclick="location.href='#browse'">Class 12</div>
      <div class="course-box" onclick="location.href='#browse'">JEE</div>
      <div class="course-box" onclick="location.href='#browse'">NEET</div>
      <div class="course-box" onclick="location.href='#browse'">Commerce</div>
    </div>
    <button class="add-notes-btn" onclick="location.href='#sell'">+ Add Notes</button>
  </section>  <section id="browse" class="section">
    <h2>Available Notes</h2>
    <div class="notes">
      <div class="note-card">
        <h3>Class 11 Business Studies</h3>
        <p>PDF notes - Chapterwise with examples.</p>
        <strong>₹30</strong>
      </div>
      <div class="note-card">
        <h3>JEE Physics Formulas</h3>
        <p>Full syllabus quick-revision notes.</p>
        <strong>₹40</strong>
      </div>
      <div class="note-card">
        <h3>NEET Biology Diagrams</h3>
        <p>High quality hand-drawn images with labels.</p>
        <strong>₹50</strong>
      </div>
    </div>
  </section>  <section id="sell" class="section">
    <h2>Sell or Donate Notes</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email ID" required />
      <input type="text" placeholder="Phone Number" required />
      <input type="text" placeholder="Course/Class" required />
      <input type="file" accept="application/pdf" required />
      <input type="number" placeholder="Set Price (or 0 to Donate)" required />
      <textarea placeholder="Short Description of Your Notes"></textarea>
      <button type="submit">Upload Notes</button>
    </form>
  </section>  <section id="profile" class="section">
    <h2>Your Profile</h2>
    <form>
      <input type="text" placeholder="Full Name" required />
      <input type="email" placeholder="Email Address" required />
      <input type="text" placeholder="Phone Number" required />
      <input type="text" placeholder="Your Course" required />
      <input type="file" accept="image/*" />
      <button type="submit">Save Profile</button>
    </form>
  </section>  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>Questions? Want to list your notes faster?</p>
    <ul>
      <li>WhatsApp: <a href="https://wa.me/91XXXXXXXXXX">Chat Now</a></li>
      <li>Email: notebazaar@example.com</li>
    </ul>
  </section>  <footer>
    <p>&copy; 2025 NoteBazaar. Built for students, by students.</p>
  </footer>
</body>
</html>
