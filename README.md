<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mediaqueries.css" />
  </head>
  <style>
    /* GENERAL */
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap");
* {
  margin: 0;
  padding: 0;
}
body {
  font-family: "Poppins", sans-serif;
  background-color: floralwhite;
}
html {
  scroll-behavior: smooth;
}
p {
  color: rgb(85, 85, 85);
}
/* TRANSITION */
a,
.btn {
  transition: all 300ms ease;
}
/* DESKTOP NAV */
nav,
.nav-links {
  display: flex;
}
nav {
  justify-content: space-around;
  align-items: center;
  height: 17vh;
}
.nav-links {
  gap: 2rem;
  list-style: none;
  font-size: 1.5rem;
}
a {
  color: black;
  text-decoration: none;
  text-decoration-color: white;
}
a:hover {
  color: grey;
  text-decoration: underline;
  text-underline-offset: 1rem;
  text-decoration-color: rgb(181, 181, 181);
}
.logo {
  font-size: 2rem;
}
.logo:hover {
  cursor: default;
}
/* HAMBURGER MENU */
#hamburger-nav {
  display: none;
}
.hamburger-menu {
  position: relative;
  display: inline-block;
}
.hamburger-icon {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 24px;
  width: 30px;
  cursor: pointer;
}
.hamburger-icon span {
  width: 100%;
  height: 2px;
  background-color: black;
  transition: all 0.3 ease-in-out;
}
.menu-links {
  position: absolute;
  top: 100%;
  right: 0;
  background-color: white;
  width: fit-content;
  max-height: 0;
  overflow: hidden;
  transition: all 0.3 ease-in-out;
}
.menu-links a {
  display: block;
  padding: 10px;
  text-align: center;
  font-size: 1.5rem;
  color: black;
  text-decoration: none;
  transition: all 0.3 ease-in-out;
}
.menu-links li {
  list-style: none;
}
.menu-links.open {
  max-height: 300px;
}
.hamburger-icon.open span:first-child {
  transform: rotate(45deg) translate(10px, 5px);
}
.hamburger-icon.open span:nth-child(2) {
  opacity: 0;
}
.hamburger-icon.open span:last-child {
  transform: rotate(-45deg) translate(10px, -5px);
}
.hamburger-icon span:first-child {
  transform: none;
}
.hamburger-icon span:first-child {
  opacity: 1;
}
.hamburger-icon span:first-child {
  transform: none;
}
/* SECTIONS */
section {
  padding-top: 4vh;
  height: 96vh;
  margin: 0 10rem;
  box-sizing: border-box;
  min-height: fit-content;
}
.section-container {
  display: flex;
}
/* PROFILE SECTION */
#profile {
  display: flex;
  justify-content: flex-start ;
  /* gap: 5rem; */
  height: 80vh;
}
.section__pic-container {
  display: flex;
  height: 400px;
  width: 400px;
  margin: auto 0;
}
.section__text {
  align-self: center;
  text-align: center;
}
.section__text p {
  font-weight: 600;
}
.section__text__p1 {
  text-align: center;
}
.section__text__p2 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
}
.title {
  font-size: 3rem;
  text-align: center;
}
#socials-container {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 1rem;
}
/* ICONS */
.icon {
  cursor: pointer;
  height: 2rem;
}
/* BUTTONS */
.btn-container {
  display: flex;
  justify-content: center;
  gap: 1rem;
}
.btn {
  font-weight: 600;
  transition: all 300ms ease;
  padding: 1rem;
  width: 8rem;
  border-radius: 2rem;
}
.btn-color-1,
.btn-color-2 {
  border: rgb(53, 53, 53) 0.1rem solid;
}
.btn-color-1:hover,
.btn-color-2:hover {
  cursor: pointer;
}
.btn-color-1,
.btn-color-2:hover {
  background: rgb(53, 53, 53);
  color: white;
}
.btn-color-1:hover {
  background: rgb(0, 0, 0);
}
.btn-color-2 {
  background: none;
}
.btn-color-2:hover {
  border: rgb(255, 255, 255) 0.1rem solid;
}
.btn-container {
  gap: 1rem;
}
/* ABOUT SECTION */
#about {
  position: relative;
}
.about-containers {
  gap: 2rem;
  margin-bottom: 2rem;
  margin-top: 0rem;
}
.about-details-container {
  justify-content: center;
  flex-direction: column;
}
.about-containers,
.about-details-container {
  display: flex;
}
.about-pic {
  border-radius: 2rem;
}
.arrow {
  position: absolute;
  right: -5rem;
  bottom: 2.5rem;
}
.details-container {
  padding: 1.5rem;
  flex: 1;
  background: white;
  border-radius: 2rem;
  border: rgb(53, 53, 53) 0.1rem solid;
  border-color: rgb(163, 163, 163);
  text-align: center;
}
.section-container {
  gap: 4rem;
  height: 80%;
}
.section__pic-container {
  height: 400px;
  width: 400px;
  margin: auto 0;
}
/* EXPERIENCE SECTION */
#experience {
  position: relative;
}
.experience-sub-title {
  color: rgb(85, 85, 85);
  font-weight: 600;
  font-size: 1.75rem;
  margin-bottom: 2rem;
}
.experience-details-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.article-container {
  display: flex;
  text-align: initial;
  flex-wrap: wrap;
  flex-direction: row;
  gap: 2.5rem;
  justify-content: space-around;
}
article {
  display: flex;
  width: 10rem;
  justify-content: space-around;
  gap: 0.5rem;
}
article .icon {
  cursor: default;
}
/* PROJECTS SECTION */
#projects {
  position: relative;
}
.color-container {
  border-color: rgb(163, 163, 163);
  background: rgb(250, 250, 250);
}
.project-img {
  border-radius: 2rem;
  width: 90%;
  height: 90%;
}
.project-title {
  margin: 1rem;
  color: black;
}
.project-btn {
  color: black;
  border-color: rgb(163, 163, 163);
}
/* CONTACT */
#contact {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 70vh;
}
.contact-info-upper-container {
  display: flex;
  justify-content: center;
  border-radius: 2rem;
  border: rgb(53, 53, 53) 0.1rem solid;
  border-color: rgb(163, 163, 163);
  background: (250, 250, 250);
  margin: 2rem auto;
  padding: 0.5rem;
}
.contact-info-container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  margin: 1rem;
}
.contact-info-container p {
  font-size: larger;
}
.contact-icon {
  cursor: default;
}
.email-icon {
  height: 2.5rem;
}
/* FOOTER SECTION */
footer {
  height: 26vh;
  margin: 0 1rem;
}
footer p {
  text-align: center;
}
@media screen and (max-width: 1400px) {
  #profile {
    height: 83vh;
    margin-bottom: 6rem;
  }
  .about-containers {
    flex-wrap: wrap;
  }
  #contact,
  #projects {
    height: fit-content;
    margin-top: 100px;
  }
}
@media screen and (max-width: 1200px) {
  #desktop-nav {
    display: none;
  }
  #hamburger-nav {
    display: flex;
  }
  #experience,
  .experience-details-container {
    margin-top: 2rem;
  }
  #profile,
  .section-container {
    display: block;
  }
  .arrow {
    display: none;
  }
  section,
  .section-container {
    height: fit-content;
  }
  section {
    margin: 0 5%;
    margin-top:-150px;
  }
  .section__pic-container {
    width: 275px;
    height: 275px;
    margin: 0 auto 2rem;
  }
  .about-containers {
    margin-top: 0;
  }
}
@media screen and (max-width: 600px) {
  #contact,
  footer {
    height: 28vh;
  }
  #profile {
    height: 83vh;
    margin-bottom: 0;
  }
  article {
    font-size: 1rem;
  }
  footer nav {
    height: fit-content;
    margin-bottom: 2rem;
  }
  .about-containers,
  .contact-info-upper-container,
  .btn-container {
    flex-wrap: wrap;
  }
  .contact-info-container {
    margin: 0;
  }
  .contact-info-container p,
  .nav-links li a {
    font-size: 1rem;
  }
  .experience-sub-title {
    font-size: 1.25rem;
  }
  .logo {
    font-size: 1.5rem;
  }
  .nav-links {
    flex-direction: column;
    gap: 0.5rem;
    text-align: center;
  }
  .section__pic-container {
    width: auto;
    height: 62vw;
    justify-content: center;
  }
  .section__text__p2 {
    font-size: 1.25rem;
  }
  .title {
    font-size: 2rem;
  }
  .text-container {
    text-align: justify;
  }
}
  </style>
  <body>
    <nav id="desktop-nav">
      <div class="logo">Dhuwarakesh</div>
      <div>
        <ul class="nav-links">
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>
    <nav id="hamburger-nav">
      <div class="logo">Dhuwarakesh</div>
      <div class="hamburger-menu">
        <div class="hamburger-icon" onclick="toggleMenu()">
          <span></span>
          <span></span>
          <span></span>
        </div>
        <div class="menu-links">
          <li><a href="#about" onclick="toggleMenu()">About</a></li>
          <li><a href="#experience" onclick="toggleMenu()">Experience</a></li>
          <li><a href="#projects" onclick="toggleMenu()">Projects</a></li>
          <li><a href="#contact" onclick="toggleMenu()">Contact</a></li>
        </div>
      </div>
    </nav>
    <section id="profile">
      <div class="section__pic-container">
        <!-- <img src="./assets/dhuwark.jpeg" alt="John Doe profile picture" /> -->
      </div>
      <div class="section__text">
        <p class="section__text__p1">Hello, I'm</p>
        <h1 class="title">Dhuwarakesh R</h1>
        <p class="section__text__p2">Frontend Developer and <br>UI/UX Designer<br></p>
        <div class="btn-container">
          <button
            class="btn btn-color-2"
            onclick="window.open('./assets/Dhuwarakesh_R_Resume.pdf')"
          >
            Download CV
          </button>
          <button class="btn btn-color-1" onclick="location.href='./#contact'">
            Contact Info
          </button>
        </div>
        <!-- <div id="socials-container">
          <img
            src="./assets/linkedin.png"
            alt="My LinkedIn profile"
            class="icon"
            onclick="location.href='https://linkedin.com/'"
          />
          <img
            src="./assets/github.png"
            alt="My Github profile"
            class="icon"
            onclick="location.href='https://github.com/'"
          />
        </div> -->
      </div>
    </section>
    <section id="about">
      <p class="section__text__p1">Get To Know More</p>
      <h1 class="title">About Me</h1>
      <div class="section-container">
        <div class="section__pic-container">
          <img
            src="./assets/dhuwark.jpeg"
            alt="Profile picture"
            class="about-pic"
          />
        </div>
        <div class="about-details-container">
          <div class="about-containers">
            <div class="details-container">
              <img
                src="./assets/experience.png"
                alt="Experience icon"
                class="icon"
              />
              <h3>Experience</h3>
              <p>2+ years <br />Frontend Development <br> Ui/Ux Designer</p>
            </div>
            <div class="details-container">
              <img
                src="./assets/education.png"
                alt="Education icon"
                class="icon"
              />
              <h3>Education</h3>
              <p>B.E Computer Science And Engineer</p>
            </div>
          </div>
          <div class="text-container">
            <p>
              Welcome to my web developer portfolio! I'm Dhuwarakesh, a skilled and
            creative web developer with a passion for  creating beautiful,
            responsive, and user-friendly websites., I've worked on a variety of
            web projects, ranging from personal blogs to e-commerce platforms.
            </p>
          </div>
        </div>
      </div>
      <img
        src="./assets/arrow.png"
        alt="Arrow icon"
        class="icon arrow"
        onclick="location.href='./#experience'"
      />
    </section>
    <section id="experience">
      <p class="section__text__p1">Explore My</p>
      <h1 class="title">Experience</h1>
      <div class="experience-details-container">
        <div class="about-containers">
          <div class="details-container">
            <h2 class="experience-sub-title">Frontend Development</h2>
            <div class="article-container">
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>HTML</h3>
                  <p>Experienced</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>CSS</h3>
                  <p>Experienced</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>React Js </h3>
                  <p>Intermediate</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>JavaScript</h3>
                  <p>Intermediate</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>TypeScript</h3>
                  <p>Basic</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>Laravel</h3>
                  <p>Intermediate</p>
                </div>
              </article>
            </div>
          </div>
          <div class="details-container">
            <h2 class="experience-sub-title">Ui/Ux Designer</h2>
            <div class="article-container">
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>Figma</h3>
                  <p>Intermediate</p>
                </div>
              </article>
              <article>
                <img
                  src="./assets/checkmark.png"
                  alt="Experience icon"
                  class="icon"
                />
                <div>
                  <h3>photoshop</h3>
                  <p>Basic</p>
                </div>
              </article>              
            </div>
          </div>
        </div>
      </div>
      <img
        src="./assets/arrow.png"
        alt="Arrow icon"
        class="icon arrow"
        onclick="location.href='./#projects'"
      />
    </section>
    <section id="projects">
      <p class="section__text__p1">Browse My Recent</p>
      <h1 class="title">Projects</h1>
      <div class="experience-details-container">
        <div class="about-containers">
          <div class="details-container color-container">
            <div class="article-container">
              <img
                src="./assets/123.png"
                alt="Project 1"
                class="project-img"
              />
            </div>
            <h2 class="experience-sub-title project-title">123ezalerts</h2>
            <div class="btn-container">
              <button
                class="btn btn-color-2 project-btn"
                onclick="location.href='https://www.123ezalerts.com/'"
              >
                Live Demo
              </button>
            </div>
          </div>
          <div class="details-container color-container">
            <div class="article-container">
              <img
                src="./assets/web1.jpg"
                alt="Project 2"
                class="project-img"
              />
            </div>
            <h2 class="experience-sub-title project-title">Website Development</h2>
            <div class="btn-container">
              <button
                class="btn btn-color-2 project-btn"
                onclick="location.href='https://github.com/'"
              >
                Live Demo
              </button>
            </div>
          </div>
          <div class="details-container color-container">
            <div class="article-container">
              <img
                src="./assets/foood.png"
                alt="Project 3"
                class="project-img"
              />
            </div>
            <h2 class="experience-sub-title project-title">Food Ordering App<br>Ui/Ux design</h2>
            <div class="btn-container">
              <button
                class="btn btn-color-2 project-btn"
                onclick="location.href='https://www.figma.com/design/CyxF27UAQWjehMAa5z6f6w/Food-app-design?m=dev&node-id=1-132&t=0o5NZLk3UC5GO6sb-1'"
              >
                Live Demo
              </button>
            </div>
          </div>
        </div>
      </div>
      <img
        src="./assets/arrow.png"
        alt="Arrow icon"
        class="icon arrow"
        onclick="location.href='./#contact'"
      />
    </section>
    <section id="contact">
      <p class="section__text__p1">Get in Touch</p>
      <h1 class="title">Contact Me</h1>
      <div class="contact-info-upper-container">
        <div class="contact-info-container">
          <img
            src="./assets/email.png"
            alt="Email icon"
            class="icon contact-icon email-icon"
          />
          <p><a href="mailto:dhuwarakesh2602@gmail.com">dhuwarakesh2602@gmail.com</a></p>
        </div>
      </div>
    </section>
    <script src="script.js"></script>
  </body>
</html>

<script>
  function toggleMenu() {
  const menu = document.querySelector(".menu-links");
  const icon = document.querySelector(".hamburger-icon");
  menu.classList.toggle("open");
  icon.classList.toggle("open");
}

</script>#   d h u w a r u  
 