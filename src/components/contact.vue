<template>
  <div>
    <header>
      <nav class="navbar">
        <div class="logo">
          <a href="#"><img src="../assets/Group 247.png" alt="SELVY TEX Logo"></a>
        </div>
        <ul class="nav-links">
          <li class="fonts"><router-link to="/">Home</router-link></li>
          <li class="fonts"><router-link to="company">Our Company</router-link></li>
          <li class="fonts"><router-link to="services">Our Services</router-link></li>
          <li class="fonts"><router-link to="product">Our Product</router-link></li>
          <!--<li><a href="#">How To Order</a></li>-->
          <li class="fonts"><router-link to="contact">Contact</router-link></li>
          </ul>
            <!--<div class="flag">
                <img loading="lazy"
                    srcset="https://cdn.builder.io/api/v1/image/assets%2Fb4f70d42747f4784a7941910e7311e3c%2F53e717eb79cc432db4d5dd09319488b6"
                    class="nav-flag" />
            </div>-->
      </nav>
    </header>
    <section class="sec2">
      <div class="sec2-text">
        <h1>SELVYTEX</h1>
        <!--<p>Selvy Tex exceptionally blends premium fabrics like Polyester, Viscose, and Modal <br> to create outstanding
          garments, offering clients more than just a product and <br>providing strong partnerships and guaranteed high
          quality. Our meticulous <br> production process, from cutting to packing, is overseen by a specialized
          Quality<br>Control Team, ensuring each stage meets the highest standards for export.</p>-->
          <pre>"Let's create something extraordinary together! Reach out to <span style="size: 1.6em;">SELVYTEX</span> 
  for partnerships and inquiries, and be a part of our journey towards a 
    stylish, sustainable future."</pre>
      </div>
      <order></order>
    </section>
    <section class="image-section">
      <div class="image-container">
        <img loading="lazy"
          src="https://cdn.builder.io/api/v1/image/assets/TEMP/728827dc69be2012abcfd0b704bb8a1fcc2942be34e669a0e82cb6bd2b5bb7ad?placeholderIfAbsent=true&apiKey=5acb37f697474270ad553272da64e56a"
          alt="Decorative image" class="main-image" />
      </div>
    </section>
    <footer>
      <div class="footer">
          <div class="footer-column">
              <img src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2Fa5682d076d5c4a38903293c828d70d7f"
                  class="footer-logo" />
          </div>
          <div class="footer-column">
              <div class="footer-title">Contact</div>
              <div class="footer-address">
                  8/962, PN Rd, Karupparayan Nagar,
                  <br />
                  Tiruppur, India. 641603
              </div>
              <div class="footer-email">
                  Email:
                  <span style="font-weight: 400">contact@selvytex.com</span>
              </div>
          </div>
          <div class="footer-column">
              <div class="footer-title1">Quick links</div>
              <a class="footer-link">Home</a>
              <a class="footer-link">Our Company</a>
              <a class="footer-link">Our Services</a>
              <a class="footer-link">Our Products</a>
              <a class="footer-link">Contact</a>
          </div>
          <div class="footer-column">
              <div class="footer-title2">Follow</div>
              <section class="image-gallery">
                  <a href="#" class="gallery-link">
                          <iframe src="https://lottie.host/embed/1de96175-78f1-4470-b4bd-1ecee7f015b4/xwRhL2Oyom.json" style="border: none;width: 50px;height: 50px;"></iframe>
                  </a>
                  <a href="#" class="gallery-link">
                      <iframe src="https://lottie.host/embed/411e08a3-9b01-4c6c-81f2-a4f56f380914/yzQ74zRUxY.json" style="border: none;width: 50px;height: 50px;"></iframe>
                  </a>
                  <a href="#" class="gallery-link">
                    <iframe src="https://lottie.host/embed/21aa1fcc-14ac-4496-af7b-461b1dd17b64/L7s9Cabj26.json" style="border: none;width: 40px;height: 40px;"></iframe>      
                  </a>
              </section>
          </div>
      </div>
      <div class="footer-rect">

      </div>
  </footer>
  </div>
</template>

<script>
export default {
  name: 'ContactForm',
  data() {
    return {
      firstName: '',
      lastName: '',
      email: '',
      phone: '',
      message: ''
    }
  },
  methods: {
    submitForm() {
      console.log('Form submitted', this.$data);
    }
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}

header {
  background-color: white;
}

.navbar {
  display: flex;
  /*
  align-items: center;
  justify-content: space-between;
  padding: 0 2em;
  */
}
.fonts
{
  font-family: 'Outfit', sans-serif;
  text-transform: uppercase;
  position: relative;
}
.logo
{
  flex-basis: 25%;
  margin-top: 20px;
}
.nav-links
{
  flex-basis: 70%;
}

.logo img {
  width: 96%;
}

.nav-links {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

/*.nav-links li {
  font: 400 20px Monda, sans-serif;
}*/

.nav-links a {
  text-decoration: none;
  color: #E07040;
  font-weight: bold;
  font-size: 1.6rem;
  margin-left: 2em;
}

/* Responsive Design for Tablets and Smaller Screens */
@media screen and (max-width: 1024px) {
  .navbar {
    padding: 0 30px;
  }

  .nav-links a {
    font-size: 1rem;
    margin-left: 2em;
  }

  .logo img {
    height: 80px;
    width: 150px;
  }
}

@media screen and (max-width: 768px) {
  .navbar {
    padding: 0 20px;
  }

  .nav-links a {
    font-size: 0.9rem;
    margin-left: 1.5em;
  }

  .logo img {
    height: 70px;
    width: 130px;
  }
}

@media screen and (max-width: 480px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
    padding: 0 10px;
  }

  .logo img {
    height: 60px;
    width: 110px;
  }

  .nav-links {
    flex-direction: column;
    width: 100%;
  }

  .nav-links li {
    margin-left: 0;
    margin-bottom: 10px;
  }

  .nav-links a {
    font-size: 1rem;
    margin-left: 0;
  }
}

.sec2 {
  height: 111vh;
  width: 100%;
  background-image: url(/src/assets/Ellipse.png);
  background-position: center;
  background-size: cover;
  margin-top: 1em;
  opacity: 95%;
}

.sec2-text h1 {
  color: #D25D38;
  font-family: "Magra", sans-serif;
  font-size: 40px;
  font-size: 4rem;
  font-weight: bolder;
  letter-spacing: 1px;
  line-height: 50px;
  text-align: center;
  padding-top: 2em;
  transition: all 0.5ms ease-in-out;
}
.sec2-text h1:hover
{
  letter-spacing: 20px;
  opacity: 70%;
}

.sec2-text pre {
  font-family: "Open Sans-Regular", Helvetica;
  text-align: center;
  /*text-align: center;*/
  font-size: 20px;
  font-weight: 400;
  line-height: 27px;
  margin-top: 1em;
  margin-bottom: 2em;
  padding-bottom: 3.5em;
}

.contact-container {
  display: flex;
  justify-content: space-between;
  padding: 40px;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 20px;
  width: 80%;
  margin: 0 auto;
  margin-top: 4em;
  height: 85%;

}

.contact-info {
  margin-right: 40px;
  padding: 0em 4em;
}

.contact-info h2 {
  color: #e07040;
  font-family: "Magra",sans-serif;
  font-size: 48px;
  font-weight: bold;
  height: 100px;
  left: 0;
  letter-spacing: 0;
  line-height: 100px;
  text-align: center;
  white-space: nowrap;
}

.info {
  margin-top: 2em;
}

.social-media {
  margin-top: 2em;
}

.social-img {
  margin-top: 1em;
}

.social-img img {
  margin-left: 1em;
}

.social-media h3 {
  color: #e07040;
  font-family: "Magra", sans-serif;
  font-size: 24px;
  font-weight: 700;
  letter-spacing: 0;
  white-space: nowrap;
}

.contact-form {
  font-family: Poppins, sans-serif;
  text-align: center;
  max-width: 698px;
  margin: 0 auto;
}

.form-container {
  background-color: rgba(224, 112, 64, 0.9);
  border-radius: 20px;
  padding: 1em 56px;
  height: 97%;

}

.form-title {
  color: #fff;
  font: 600 48px/100px Magra, sans-serif;
  margin-bottom: 0.40em;
}

.name-fields {
  display: flex;
  gap: 40px;
  margin-bottom: 3px;
}

.input-group {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  width: 100%;
  margin-bottom: 18px;
}

.input-group label {
  color: #fff;
  font-size: 15px;
  font-weight: 400;
  margin-bottom: 11px;
}

.input-field {
  width: 100%;
  padding: 15px;
  border: none;
  border-radius: 15px;
  background-color: #fff;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.8);
  font-weight: 275;
}

.phone-input {
  display: flex;
  align-items: center;
  background-color: #fff;
  border-radius: 15px;
  padding: 0 25px;
  width: 96%;
}

.country-code {
  color: #000;
  font-size: 15px;
  font-weight: 300;
  margin-right: 17px;
}

.message-area {
  height: 17vh;
  resize: vertical;
}

.submit-button {
  background-color: #fff;
  border: none;
  border-radius: 15px;
  color: rgba(0, 0, 0, 0.8);
  cursor: pointer;
  font-size: 20px;
  font-weight: 400;
  padding: 13px 70px;
  transition: background-color 0.3s ease;
}

.submit-button:hover {
  background-color: #f0f0f0;
}

@media (max-width: 991px) {
  .form-container {
    padding: 26px 20px;
  }

  .form-title {
    font-size: 40px;
    line-height: 93px;
  }

  .name-fields {
    flex-direction: column;
    gap: 20px;
  }

  .submit-button {
    width: 100%;
    padding: 13px 20px;
  }
}

.image-section {
  display: flex;
  padding-top: 123px;
  flex-direction: column;
  margin-top: 33em;
}

.image-container {
  background-color: rgba(224, 112, 64, 0.55);
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0 70px 146px;
}

.main-image {
  aspect-ratio: 3.5;
  object-fit: contain;
  object-position: center;
  width: 100%;
  z-index: 10;
  max-width: 1240px;
  margin: -123px 0 -29px;
  transition: all 2ms ease-in-out;
}
.main-image:hover
{
  transform: translateY(10px);
}

@media (max-width: 991px) {
  .image-section {
    padding-top: 100px;
  }

  .image-container {
    max-width: 100%;
    padding: 0 20px 100px;
  }

  .main-image {
    max-width: 100%;
    margin-bottom: 10px;
  }
}
.footer {
  align-items: start;
  display: flex;
  gap: 20px;
  font-weight: 400;
  justify-content: space-between;
  margin-top: 3em;
  padding: 2em 8em 0em 7em;
  height: 410px;
}

@media (max-width: 991px) {
  .footer {
      flex-wrap: wrap;
  }
}

.footer-column {
  display: flex;
  flex-direction: column;
  font-size: 12px;
  color: #333;
  padding: 0 20px 12px;
}



.footer-message {
  font-family: Lora, sans-serif;
  margin-top: 36px;
}

.footer-title {
  color: #e07040;
  margin-top: 55px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-family:'Magra', sans-serif;
  font-weight: 900;
  font-size: 20px;
  position: relative;
}

.footer-title1 {
  color: #e07040;
  position: relative;
  margin-top: 55px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font: 20px/150% Magra, sans-serif;
  font-weight: 900;
  margin-bottom: 1em;
}

.footer-title2 {
  color: #E07040;
  position: relative;
  margin-top: 55px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font: 20px/150% Magra, sans-serif;
  font-weight: 900;
  margin-bottom: 1em;
}

.footer-address {
  font-family: "Outfit", sans-serif;
  font-size: 15px;
  font-weight: 400;
  line-height: 32px;
  align-self: stretch;
  margin-top: 30px;
}

.footer-email {
  font-family: "Outfit", sans-serif;
  font-size: 15px;
  font-weight: 400;
  font-weight: 700;
  line-height: 32px;
}

.footer-language {
  color: #333;
  margin-top: 13px;
  font: 18px/156% Open Sans, sans-serif;
}

.footer-language-option {
  margin-top: 33px;
  gap: 6px;
  white-space: nowrap;
  line-height: 173%;
}

@media (max-width: 991px) {
  .footer-language-option {
      white-space: initial;
  }
}

.footer-language-flag {
  aspect-ratio: 1.45;
  object-fit: auto;
  object-position: center;
  width: 16px;
  align-self: start;
}

.footer-language-name {
  font-family: Open Sans, sans-serif;
}

.footer-link {
  margin-top: 10px;
  font-family: "Outfit", sans-serif;
  font-size: 15px;
  font-weight: 400;
}

.footer-social {
  color: #959595;
  margin-top: 32px;
  font: 15px/213% Open Sans, sans-serif;
}

.footer-rect {
  width: 100%;
  height: 5vh;
  background-color: #e07040;
}
.image-gallery {
  display: flex;
  gap: 19px;
}

.gallery-link {
  display: inline-block;
  text-decoration: none;
}
.gallery-link:hover
{
  size: 1.2em;
  cursor: pointer;
}

.gallery-image {
  object-fit: contain;
  object-position: center;
}

.small-image {
  width: 20px;
  aspect-ratio: 1;
}
.medium-image {
  width: 28px;
  aspect-ratio: 1.4;
}

.large-image {
  width: 22px;
  aspect-ratio: 1.16;
  align-self: start;
}
.cont{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: 3em;
}
.flag{
  margin-top: 1em;
  margin-left: 3em;
}
.fonts::after
{
    position: absolute;
    background:#D25D38;
    content: "";
    width: 0%;
    height: 4px;
    right: 0;
    bottom: -3px;
    transition: width 1s;
}
.fonts:hover::after
{
    width: 90%;
    cursor: pointer;
}
.footer-title1::after
{
    position: absolute;
    background:#D25D38;
    content: "";
    width: 0%;
    height: 4px;
    left: 0;
    right: 1;
    bottom: -3px;
    transition: width 1s;
}
.footer-title1:hover::after
{
    width: 90%;
    cursor: pointer;
}
.footer-title::after
{
    position: absolute;
    background:#D25D38;
    content: "";
    width: 0%;
    height: 4px;
    left: 0;
    right: 1;
    bottom: -3px;
    transition: width 1s;
}
.footer-title:hover::after
{
    width: 40%;
    cursor: pointer;
}
.footer-title2::after
{
    position: absolute;
    background:#D25D38;
    content: "";
    width: 0%;
    height: 4px;
    left: 0;
    right: 1;
    bottom: -3px;
    transition: width 1s;
}
.footer-title2:hover::after
{
    width: 50%;
    cursor: pointer;
}
.footer-link
{
  transition: transform 0.3s ease;
}
.footer-link:hover
{
  transform: translateX(5px);
}

</style>
