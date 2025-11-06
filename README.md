<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Skills Arena</title>
  <style>
    body {

      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fdfdfd;
      color: #333;
    }
    header {
      background: linear-gradient(135deg, #ff6a00, #ee0979);
      color: white;
      padding: 40px;
      text-align: center;
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }
    header p {
      font-size: 1.2rem;
    }
    .categories {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin: 30px 0;
      flex-wrap: wrap;
    }
    .category {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 200px;
      text-align: center;
      transition: 0.3s;
    }
    .category:hover {
      transform: scale(1.05);
    }
    .category img {
      width: 60px;
      margin-bottom: 10px;
    }
    .prizes {
      background: #fff8e1;
      text-align: center;
      padding: 40px 20px;
    }
    .prizes h2 {
      margin-bottom: 20px;
    }
    .prize-list {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
    }
    .prize {
      background: white;
      padding: 20px;
      border-radius: 10px;
      width: 180px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .prize img {
      width: 50px;
      margin-bottom: 10px;
    }
    .benefits {
      text-align: center;
      padding: 40px 20px;
    }
    .benefits h2 {
      margin-bottom: 20px;
    }
    .benefits ul {
      list-style: none;
      padding: 0;
    }
    .benefits ul li {
      margin: 10px 0;
      font-size: 1.1rem;
    }
    .register {
      text-align: center;
      padding: 40px 20px;
      background: #e3f2fd;
    }
    .register img {
      width: 200px;
      margin: 20px 0;
      border: 3px solid #2196f3;
      border-radius: 10px;
    }
    .footer {
      text-align: center;
      background: #333;
      color: white;
      padding: 20px;
      margin-top: 20px;
    }
    .motivation {
  text-align: center;
  padding: 40px 20px;
  background: linear-gradient(135deg, #ffecd2, #fcb69f);
  border-radius: 15px;
  margin: 40px auto;
  max-width: 900px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.motivation h2 {
  font-size: 28px;
  color: #d35400;
  margin-bottom: 15px;
}

.motivation p {
  font-size: 18px;
  margin-bottom: 25px;
  color: #333;
}

.motivation-gallery {
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-bottom: 25px;
  flex-wrap: wrap;
}

.motivation-gallery img {
  width: 200px;
  height: auto;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.highlight {
  font-size: 22px;
  font-weight: bold;
  color: #c0392b;
  margin: 15px 0;
}

.register-btn {
  display: inline-block;
  padding: 12px 30px;
  background: #e74c3c;
  color: white;
  font-size: 18px;
  font-weight: bold;
  border-radius: 30px;
  text-decoration: none;
  transition: 0.3s;
}

.register-btn:hover {
  background: #c0392b;
  transform: scale(1.05);
}

  </style>
</head>
<body>

  <header>
    <h1>
  <img src="C:\Users\hp\Desktop\index.html\skills arena.jpg" alt="Skill Arena Logo" style="height:60px; vertical-align:middle; margin-right:10px;">
  Skills Arena
</h1>
    <p>Show your talent in Singing, Dancing, Painting, and Writing & Win Exciting Prizes!</p>
  </header>

  <!-- Categories -->
  <div class="categories">
  <div class="category" onclick="showForm('Singing')">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTNc54G4O-Qy7wXwIoUdWrelrT8vCROyFCBFw&s" alt="Singing">
    <h3>Singing</h3>
  </div>

  <div class="category" onclick="showForm('Painting')">
    <img src="https://clipart-library.com/2023/360_F_108418331_8bOR9TsEkyL8wj8sT75AGxeZmqs73eb1.jpg" alt="Painting">
    <h3>Painting</h3>
  </div>

  <div class="category" onclick="showForm('Writing')">
    <img src="https://thumbs.dreamstime.com/b/old-writing-script-ink-feather-tool-12163152.jpg" alt="Writing">
    <h3>Writing</h3>
  </div>

  <div class="category" onclick="showForm('Dancing')">
    <img src="https://dbdzm869oupei.cloudfront.net/img/sticker/preview/6111.png" alt="Dancing">
    <h3>Dancing</h3>
  </div>
</div>
<section id="registerForm" style="display:none;">
  <h2 id="formTitle">📌 Register Now</h2>
  <form>
    <label>Full Name:</label><br>
    <input type="text" name="name" required><br><br>
    
    <label>Age:</label><br>
    <input type="number" name="age" required><br><br>
    
    <label>Location:</label><br>
    <input type="text" name="location" required><br><br>
    
    <label>Category:</label><br>
    <input type="text" id="categoryField" name="category" readonly><br><br>
    
    <p><b>💰 Entry Fee:</b> ₹99 for 1 entry | ₹149 for 3 entries</p>
    <p style="color:red; font-weight:bold;">
    ⚠️ Without paying the registration fee, your work will not be validated and you will be disqualified.
    </p>

    <p>Step 1: Scan & Pay using QR below</p>
    <img src="C:\Users\hp\Desktop\index.html\qr.png.jpg" alt="Payment QR Code" style="width:150px;"><br><br>
    
    <p>Step 2: Upload Screenshot of Payment</p>
    <input type="file" accept="image/*" required><br><br>
    
    <p>Step 3: Upload Your Work</p>
    <input type="file" accept="image/*,video/*,application/pdf" required><br><br>
    
    <button type="submit">Submit Entry</button>
  </form>
</section>


  <!-- Prizes -->
  <section class="prizes">
    <h2>🏆 Prizes Worth ₹4500</h2>
    <div class="prize-list">
      <div class="prize">
        <img src="https://cdn-icons-png.freepik.com/128/11173/11173709.png" alt="First Prize">
        <h3>🥇 1st Prize</h3>
        <p>₹2000 + Certificate</p>
      </div>
      <div class="prize">
        <img src="https://cdn-icons-png.freepik.com/128/11173/11173876.png" alt="Second Prize">
        <h3>🥈 2nd Prize</h3>
        <p>₹1500 + Certificate</p>
      </div>
      <div class="prize">
        <img src="https://cdn-icons-png.freepik.com/128/11173/11173877.png" alt="Third Prize">
        <h3>🥉 3rd Prize</h3>
        <p>₹1000 + Certificate</p>
      </div>
    </div>
  </section>

  <!-- Benefits -->
  <section class="benefits">
    <h2>✨ What You Get</h2>
    <ul>
      <li>🏆 Exciting Cash Prizes</li>
      <li>📜 Participation Certificates</li>
      <li>🌟 Recognition for Your Talent</li>
      <li>🎯 Chance to Get Featured</li>
    </ul>
  </section>

  <!-- Registration -->
 <section class="motivation">
  <h2>🌟 Show Your Talent, Shine Like a Star! 🌟</h2>
  <p>Join <strong>Skill Arena</strong> and take part in our National Level Online Competition.  
     Whether you sing, paint, dance, or write — this is your stage to shine.  
     Winners get <b>Cash Prizes</b>, <b>Certificates</b>, and a chance to showcase their art across India! 🏆</p>

  <div class="motivation-gallery">
    <img src="c:\Users\hp\Desktop\index.html\Screenshot 2025-11-06 163131.png" alt="Winner with certificate">
    <img src="c:\Users\hp\Desktop\index.html\Screenshot 2025-11-06 164600.png" alt="Celebrating">
    <img src="c:\Users\hp\Desktop\index.html\Screenshot 2025-11-06 164322.png" alt="Competition moment">
  </div>

  <h3 class="highlight">🔥 Don’t Just Participate, Be a Champion! 🔥</h3>

  <a href="#registration" class="register-btn">🚀 Register Now</a>
  <a href="https://www.instagram.com/skills_arena_?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==">Instagram</a>
</section>



  <div class="footer">
    <p>© 2025 Skill Arena | Follow us on Instagram & Telegram</p>
  </div>
  <script>
  function showForm(category) {
    document.getElementById('registerForm').style.display = 'block';
    document.getElementById('formTitle').innerText = "📌 Register for " + category;
    document.getElementById('categoryField').value = category;
    window.scrollTo(0, document.getElementById('registerForm').offsetTop);
  }
</script>

</body>
</html>
