![IMG_7369](https://github.com/user-attachments/assets/eb538c47-c9b4-415e-87f3-f3ea7a154f28)
# Derricks-FIRST-HTML-STYLED
This is my first HTML document with added CSS. I am currently learning JavaScript and once I finish my course. I will make projects with more real life meaning and purpose. This was simply a project to show what I currently know and to show how serious I am about my Software Developers Journey. Thank You To All Who Are Watching My Growth!

<!Doctype html>
<html>	
<head>
    <meta charset="utf-8">
    <meta name="description" content="Hello My Name Is Derrick Coburn and this is my first HTML code">
    <title>My First HTML Code 
    </title>
<style>

/* ===== 2030 HOLO INTERFACE THEME ===== */
body {
  margin: 0;
  font-family: "Segoe UI", Tahoma, sans-serif;
  color: #eaf6ff;
  background:
    radial-gradient(circle at 30% 20%, #0c1f3d, #02040a 60%),
    repeating-linear-gradient(
      to bottom,
      rgba(0,180,255,.06) 0px,
      rgba(0,180,255,.06) 1px,
      transparent 2px,
      transparent 6px
    );
  background-attachment: fixed;
}

/* ===== FLOATING HOLO HEADERS ===== */
h1, h2, h3 {
  text-transform: uppercase;
  letter-spacing: 2px;
  color: #9fe8ff;
  text-shadow:
    0 0 8px rgba(0,200,255,.8),
    0 0 24px rgba(0,120,255,.5);
}

/* ===== GLASS PANELS ===== */
section, main, nav, form, details {
  backdrop-filter: blur(10px);
  background: linear-gradient(
    180deg,
    rgba(15,35,65,.65),
    rgba(5,12,22,.75)
  );
  border: 1px solid rgba(0,200,255,.35);
  border-radius: 20px;
  padding: 24px;
  margin: 30px 0;
  box-shadow:
    0 30px 70px rgba(0,0,0,.85),
    inset 0 0 40px rgba(0,200,255,.12);
  transform-style: preserve-3d;
  transition: .25s;
}

section:hover, nav:hover, form:hover, details:hover {
  transform: translateY(-8px) scale(1.01);
  box-shadow:
    0 40px 90px rgba(0,0,0,.95),
    inset 0 0 60px rgba(0,255,255,.2);
}

/* ===== NAV = HUD BAR ===== */
nav ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
  padding: 0;
  margin: 0;
}

nav a {
  text-decoration: none;
  color: #b7f3ff;
  font-weight: 600;
  padding: 10px 16px;
  border-radius: 12px;
  background: linear-gradient(
    135deg,
    rgba(0,200,255,.25),
    rgba(0,120,255,.15)
  );
  border: 1px solid rgba(0,200,255,.45);
  box-shadow:
    0 10px 25px rgba(0,0,0,.6),
    inset 0 0 18px rgba(0,200,255,.25);
  transition: .18s;
}

nav a:hover {
  transform: translateY(-4px) scale(1.06);
  box-shadow:
    0 16px 40px rgba(0,200,255,.45),
    inset 0 0 30px rgba(0,255,255,.35);
}

/* ===== HOLO BUTTONS ===== */
input[type="submit"], button {
  background: linear-gradient(135deg, #00f0ff, #00ffa6);
  color: #00222a;
  border: none;
  border-radius: 999px;
  padding: 14px 22px;
  font-weight: bold;
  cursor: pointer;
  box-shadow:
    0 14px 34px rgba(0,255,200,.45);
  transition: .18s;
}

input[type="submit"]:hover, button:hover {
  transform: translateY(-3px) scale(1.07);
  box-shadow:
    0 20px 46px rgba(0,255,220,.75);
}

/* ===== FUTURE INPUT FIELDS ===== */
input, select {
  background: rgba(5,18,30,.9);
  color: #eaf6ff;
  border: 1px solid rgba(0,200,255,.5);
  border-radius: 12px;
  padding: 12px;
}

input:focus, select:focus {
  outline: none;
  border-color: #00f0ff;
  box-shadow:
    0 0 0 4px rgba(0,240,255,.25),
    inset 0 0 18px rgba(0,240,255,.2);
}

/* ===== DATA GRID TABLE ===== */
table {
  width: 100%;
  border-collapse: collapse;
  border-radius: 18px;
  overflow: hidden;
  box-shadow: 0 30px 70px rgba(0,0,0,.9);
}

th {
  background: linear-gradient(135deg, #00e1ff, #0077ff);
  color: #001018;
  padding: 20px;
  font-size: 22px;
  letter-spacing: 1px;
}

td {
  background: rgba(6,22,40,.95);
  padding: 20px;
  font-size: 20px;
  border-bottom: 1px solid rgba(0,200,255,.25);
}

tr:hover td {
  background: rgba(10,40,70,.95);
  box-shadow: inset 0 0 20px rgba(0,200,255,.15);
}

/* ===== MEDIA = HOLO SCREENS ===== */
img, iframe, video {
  width: 1200px;
  height: 686px;
  max-width: 100%;
  object-fit: cover;
  border-radius: 22px;
  border: 2px solid rgba(0,200,255,.5);
  box-shadow:
    0 35px 80px rgba(0,0,0,.95),
    0 0 35px rgba(0,200,255,.35);
  transform: translateZ(0);
  transition: .25s;
}

img:hover, iframe:hover, video:hover {
  transform: scale(1.02);
  box-shadow:
    0 45px 100px rgba(0,0,0,1),
    0 0 60px rgba(0,255,255,.45);
}

/* ===== ENERGY DIVIDER ===== */
hr {
  border: none;
  height: 2px;
  background: linear-gradient(
    to right,
    transparent,
    #00f0ff,
    #0077ff,
    transparent
  );
  margin: 36px 0;
}
/* ===== 2030 ANIMATION LAYER ===== */

/* slow floating panels */
section, nav, form, details {
  animation: panelFloat 8s ease-in-out infinite;
}

@keyframes panelFloat {
  0%   { transform: translateY(0px); }
  50%  { transform: translateY(-6px); }
  100% { transform: translateY(0px); }
}

/* pulsing neon headers */
h1, h2, h3 {
  animation: neonPulse 3s ease-in-out infinite;
}

@keyframes neonPulse {
  0% {
    text-shadow:
      0 0 6px rgba(0,200,255,.6),
      0 0 18px rgba(0,120,255,.4);
  }
  50% {
    text-shadow:
      0 0 16px rgba(0,255,255,1),
      0 0 40px rgba(0,120,255,.8);
  }
  100% {
    text-shadow:
      0 0 6px rgba(0,200,255,.6),
      0 0 18px rgba(0,120,255,.4);
  }
}

/* scanning light sweep across panels */
section::after,
nav::after,
form::after {
  content: "";
  position: absolute;
  inset: 0;
  border-radius: 20px;
  background: linear-gradient(
    120deg,
    transparent 0%,
    rgba(0,255,255,.18) 45%,
    transparent 60%
  );
  opacity: .25;
  animation: scanSweep 6s linear infinite;
  pointer-events: none;
}

section, nav, form {
  position: relative;
  overflow: hidden;
}

@keyframes scanSweep {
  0%   { transform: translateX(-120%); }
  100% { transform: translateX(120%); }
}

/* button energy charge */
input[type="submit"], button {
  animation: buttonCharge 2.5s ease-in-out infinite;
}

@keyframes buttonCharge {
  0%   { box-shadow: 0 10px 30px rgba(0,255,200,.35); }
  50%  { box-shadow: 0 18px 55px rgba(0,255,220,.9); }
  100% { box-shadow: 0 10px 30px rgba(0,255,200,.35); }
}

/* image holo shimmer */
img:hover, iframe:hover {
  animation: holoShimmer .9s linear;
}

@keyframes holoShimmer {
  0% { filter: brightness(1); }
  50% { filter: brightness(1.25); }
  100% { filter: brightness(1); }
}

/* table row hover ripple */
tr {
  transition: transform .15s, box-shadow .15s;
}

tr:hover {
  transform: scale(1.01);
  box-shadow: 0 0 18px rgba(0,200,255,.25);
}
/* ===== 2030 PARTICLE FIELD ===== */

body::before {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  background-image:
    radial-gradient(circle at 10% 20%, rgba(0,255,255,.25) 1px, transparent 2px),
    radial-gradient(circle at 80% 40%, rgba(0,200,255,.2) 1px, transparent 2px),
    radial-gradient(circle at 30% 70%, rgba(0,255,200,.18) 1px, transparent 2px),
    radial-gradient(circle at 60% 90%, rgba(0,180,255,.22) 1px, transparent 2px);
  background-size: 220px 220px;
  animation: particleDrift 40s linear infinite;
  opacity: .35;
}

@keyframes particleDrift {
  from { transform: translateY(0); }
  to   { transform: translateY(-600px); }
}


/* ===== SCROLLING HOLO GRID ===== */

body::after {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  background:
    linear-gradient(rgba(0,200,255,.12) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0,200,255,.12) 1px, transparent 1px);
  background-size: 60px 60px;
  mask-image: radial-gradient(circle at center, black, transparent 75%);
  animation: gridMove 18s linear infinite;
  opacity: .25;
}

@keyframes gridMove {
  from { background-position: 0 0, 0 0; }
  to   { background-position: 0 600px, 600px 0; }
}


/* ===== HOLO LINK GLOW TRAIL ===== */

a {
  position: relative;
}

a:hover {
  text-shadow:
    0 0 8px rgba(0,255,255,.9),
    0 0 22px rgba(0,180,255,.7);
}


/* ===== CYBER LIST ITEMS ===== */

li {
  transition: transform .15s, text-shadow .15s;
}

li:hover {
  transform: translateX(6px);
  text-shadow: 0 0 10px rgba(0,255,255,.6);
}


/* ===== SUMMARY DROPDOWN FX ===== */

summary {
  cursor: pointer;
  font-weight: bold;
  letter-spacing: 1px;
}

details[open] summary {
  color: #00f0ff;
  text-shadow: 0 0 12px rgba(0,255,255,.8);
}

</style>
</head>
<body>
    <h1>Welcome! This is my first HTML Project!
    </h1>
    <hr>
      <nav>
        <ul>
            <li><a href="#experiences">My Experiences</a></li>
            <li><a href="#code">Why I Want To Code?</a></li>
            <li><a href="#plans">Where Do I See Myself In 5 Years?</a></li>
            <li> <a href="#weakness">Where Do I Need To Strengthen My Code?</a></li>
        </ul>
     </nav>
    <hr>
    <h2>I plan on creating <mark>multiple</mark> projects every week to show my knowledge and understanding of the languages. This is not a specific build or
project but it is just a display of my understanding of HTML elements and semantics as I
continue on my journey of learning more everyday.
    </h2>        
    <details>
          <summary> Listen To This Cool Audio While Reading My HTML Document!</summary>
    <hr>
   <audio controls autoplay>
  <source src="Audio.files/binary-code-interface.mp3" type="audio/mpeg">
</audio>
      </p>
      </details>
     <ul>
       <li>HTML</li>
       <li>CSS</li>
       <li>JAVASCRIPT</li>
    </ul>
    <hr>
    <main>
  <section id="experiences">
    <h2>1. My Experiences So Far?
    </h2>
    <p>It's been pretty challenging learning all of these languages, but overall I enjoy learning the skill as a whole. I usually start coding first thing in the morning at 8am to about 12pm.I will start off with HTML lessons; then I will work my way all the way through CSS down to JAVASCRIPT. I find it beneficial to allow my brain to dive into each language everyday to keep my coder mind flowing & to not stay stagnent. 
    </p>
    <figcaption>Life Of A Developer<figcaption>
    <img src= "https://github.com/user-attachments/assets/70943c8a-d136-45e3-a090-398b2e5ed92e" alt= "Stressed Out Developer" height="686" width="1200" loading="eager">
    </section>
  <section id="code">
    <h2>2. Why I Want To Code?
    </h2>
    <p>When I was a child, I was always drawn to computers. I loved tech, games and social applications from the dawn of the age. I remember building my own myspace page and I will never forget the day Facebook launched and blew myspace out of business. I really want to be apart of the future development of society and apart of the future digital infrastructure.
    </p>
    </section>
    <details>
          <summary>What's my favorite language?          </summary>
    <p>I don't have a favorite, I <em>"LOVE"<em>CODING in general!
    </p>
    </details>
    <p>I am already a spiritual person and I see life in a different way than others. The way I see coding is in the same manner. I see coding to be the invisible realm in the phyisical world of computers. Most of the time it is over-looked, but little do we know its the key factor to all physical life/computing life.
    </p>
    <figcaption>I Love Coding<figcaption>
    <img src="https://github.com/user-attachments/assets/443cdf4a-51fd-4e88-8467-542256250f33" alt="Image Of A Developer" width="1200" height="686">
    <section id="plans" loading="eager">
    <h2> 3. Where Do I See Myself In 5 Years?
    </h2>
    <p>In 5 years, I see myself going very far and creating a great name for myself in the software development space.I know things will not be easy or get easier, as it wasn't even easy for me to make it this far. Being a coder is about loving problems and being solution based. I have a great understadning of that, so I know I will be in the space for the long haul. Making a long story short, I see myslef being a "Senior Developer In 5 Years & maybe even better". After I knock out and have a clear understanding of HTML, CSS & JAVASCRIPT; I will move on the more challenging languages like:
    </p>
    <ul>
       <li>PYTHON</li>
       <li>REACT</li>
       <li>SQL</li>
    </ul>
    <figcaption>More Challenging Programming Languages
    </figcaption>
    <img src="https://github.com/user-attachments/assets/b6c1d10b-1c63-473f-8966-8ac2a75baeeb" alt="Group Of Progamming Languages" height="500" width="1200" loading="lazy">
    </section>
    <section id="weakness">
    <h2>4. Where Do I Think I Should Strengthen My HTML Coding Currently?
    </h2>
    <ol>
       <li>ADDING LINKS ✅</li>
       <li>ADDING TABLES</li>
       <li>ADDING AUDIO</li> ✅
       <li>ADDING VIDEOS ✅</li>
       <li>BETTER SEMANTICS ✅</li>
       <li>ADDING BUTTONS ✅ </li>
    <hr>
    </ol>
    <p>This is my first coding project, so my intentions isn't to make this one super fancy. You will see my growth as I continue to implement what I learn in future projects. See you on the next update! 
    </p>
    <figcaption>Thanks For Reading My First HTML CODE!<figcaption>
    <img src="https://github.com/user-attachments/assets/78e6b4fc-d9d9-4364-bee4-26f68588855b" alt="Software Team Celebrating" width="1200" height="680" loading="lazy">
      </section>
      </main>
     <br>
     <br>
     <section>
     <h2>1.MY FIRST HTML PROJECT (PART2/UPDATES)
     <hr>
     </h2>
     <p>During "Part 1" of my first HTML code; I laid a solid foundation without adding any complex elements.During this session I will be adding LINKS & 1 VIDEO. I hope you all enjoy the process and I would absolutley love to hear feedback from Senior & experienced developers! I know how far you can get just by having a student mentality & I will always be a student of the craft.
     </p>
     <h2>Here is a short video about the importance of adding links to your HTML document:
     </h2>
     <h3>Adding links to your page can not only help you, but it can absolutley help the user gather informatiom from other webs quickly & it can help the user navigate to other parts of the document quicker.
     </h3>
   <figcaption>LINKS 101<figcaption>
    <iframe src="https://www.youtube.com/embed/tsEQgGjSmkM?rel=0" width="1200" height="680"" allowfullscreen scrolling="no" allow="accelerometer *; clipboard-write *; encrypted-media *; gyroscope *; picture-in-picture *; web-share *;" referrerpolicy="strict-origin">
    </iframe>
    </section>
    <section>
    <h2>2. Now That We Have "Links & Videos" On Our Page! Let's Add Some Semantics To Our HTML Document!
    <hr>
    </h2>
    <p>Semantics is the invisible structure of your document that gives the browser and seo a better understanding of what's going on in your HTML document. It gives clearer meanings and organization in your document. Semantics also helps you keep your code clean for future employers and collaboraters.The last thing you want to do is have sloppy code in a group project, it will slow down progress and cause avoidable confusion. I like to see Semantics as the <strong>organizer</strong> of your code</p>
    <figcaption>Semantics 101</figcaption>
 <iframe src="https://www.youtube.com/embed/kX3TfdUqpuU?rel=0" width="1200"  
height="680" allowfullscreen scrolling="no" allow="accelerometer *; clipboard-write *; encrypted-media *; gyroscope *; picture-in-picture *; web-share *;" referrerpolicy="strict-origin">
    </iframe>
    </section>
    <h2>3. We've added LINKS,VIDEOS & SEMANTICS to our HTML document!
    </h2>
    <hr>
    <p>Our HTML document is now starting to come together. We have a nice structure before we even added CSS. We have 3 more elements to add:
        <ol>
            <li>AUDIO</li>
            <li>TABLES</li>
            <li>BUTTONS</li>
        </ol>
        <ul>
        <li>I will add a form and input at the end of our HTML document as well to make our web page look a little more well put together & to get interaction from the user.</li>
        </ul>
          <h2>4. Adding A Form With Input
    <hr>
    </h2>
    <p>Today we will be adding a "Form" with "Input" into our HTML Document.These two elements play a major role in gathering information from the user. "Forms" & "Inputs" are the gateways to commuicating,recieving and giving value from the developer and user. You can allow
a user to suscribe, sign-up, give surveys the list goes on.
When your putting in information for an interview that would
be a "Form" & "Input".
    </p>
    <details>
       <summary>Where do we see "Forms" & "Inputs" in our everyday life?
       </summary>
    <p>
      <ul>
         <li>Interview Applications</li>
         <li>Sign-Up Forms</li>
         <li>Surveys</li>
         <li>Log In</li>
      </ul>
    </details>
    </p>
    <form>
        <h2>5. Login/Sign Up Form With Input</h2>
        <hr>
        <label for="birthday">Birthday</label>
        <input type="date" name="birthday" id="birthday">
        <p>
        <label for="email">Email</label>
        <input type="email" name="email" id="email"/>
        </p>
        <p>
        <label for="password">Password</label>
        <input type="password" name="password" id="password">
        </p>
        <input type="submit">
    </form>
    <hr>
    <p>Do You Want To Recieve Updates By Email?
    <label for="updates-yes">Yes</label>
    <input type="radio" id="updates-yes" name="updates" value ="yes"checked>
    <label for="updates-no">No
    </label>
    <input type="radio" id="updates-no" name="updates" value="no">
    </p>
    <p>
    <label for="accept-terms">I Accept Our Terms & Conditions
    </label>
    <input type="checkbox" id="accept-terms" name="accept-terms" value="accept">
     </p>
     <h2>OUTR0</h2>
     <p>This will be last section of my first HTML. I will be implementing a table into the chart. I will be adding the store hours of one of my favorite fast food restaraunts. Tables have plenty of usages;being a key way of storing data in many different ways. Here's a table of one of my favorite fast food restaraunts called "Freddy's":
       
      <h2>Freddy's Store Hours
      </h2>
      
      <table style="font-size: 30px;">
    <tr>
        <th>Sunday</th>
        <th>Monday</th>
        <th>Tuesday</th>
        <th>Wednesday</th>
        <th>Thursday</th>
        <th>Friday</th>
        <th>Saturday</th>
    </tr>
    <tr>
        <td>10:30am-10:00pm</td>
        <td>10:30am-10:00pm</td>
        <td>10:30am-10:00pm</td>
        <td>10:30am-10:00pm</td>
        <td>10:30am-10:00pm</td>
        <td>10:30am-11:00pm</td>
        <td>10:30am-11:00pm</td>
    </tr>
</table>
      <img src="img/DD068BBD-6FA6-4883-8FD2-155087AB0C75.jpeg" 
     width="1200" 
     height="686" 
     alt="Freddy's Restaurant"
     title="Freddy's"
     style="border: 5px solid black;">
        </p>
        <p><a href="#">Back To Top
    </p></a>
     
       &lt;&lt;&lt; &copy Derrick Coburn &gt;&gt;&gt;    </body>
