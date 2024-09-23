<template>
    <div> <!--service-->
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
        <div class="service-header">
            <div class="service-line"></div>
            <h2 class="service-title">OUR SERVICES</h2>
            <div class="service-line"></div>
        </div>
        <div class="sec1">
            <img
                src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2F7ffb2b5d70dd4f39a27765f401b3446b">
        </div>
        <div class="sec2">
            <img
                src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2F5674fcd44c9d4c8495c2e25dd0ba3a00">
        </div>
        <div class="sec3">
            <img
                src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2Fb83ba3684db04e1f8c980b3445a2d913">
        </div>
        <div class="sec4">
            <img
                src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2F3fb2734da7e94ef09d6e8501094c119e">
        </div>
        <div class="sec5">
            <img src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2Fa0a74457f7ce4e42a3484787a10b81f3"
                class="responsive-image">
        </div>
        <div class="sec6">
            <img
                src="https://cdn.builder.io/api/v1/image/assets%2Faf0c4f4a34884a7c857808257a84dbe0%2F34e2bf7b808948cc9e101807c0d35e9e">
        </div>
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
import { RouterLink } from "vue-router"
export default {

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
/*
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 2em;
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
}

.nav-links li {
    font: 400 20px Monda, sans-serif;
}

.nav-links a {
    text-decoration: none;
    color: #D25D38;
    font-weight: bold;
    font-size: 1.1rem;
    margin-left: 3em;
}
*/
.navbar {
display: flex;
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

.sec1 {
    margin-top: 5em;
}

.sec1 img {
    width: 100%;
}

.sec2 {
    margin-top: 5em;
}

.sec2 img {
    width: 100%;
}

.sec3 {
    margin-top: 5em;
}

.sec3 img {
    width: 100%;
}

.sec4 {
    margin-top: 5em;
}

.sec4 img {
    width: 100%;
}

.sec5 {
    margin-top: 5em;
}

.sec5 img {
    width: 100%;
}

.sec6 {
    margin-top: 5em;
}

.sec6 img {
    width: 100%;
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
    margin-top: 13px;
    font-family: "Outfit-Regular", Helvetica;
    font-size: 17px;
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
.cont {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top: 2em;
}

.flag {
    margin-top: 1em;
    margin-left: 3em;
}

.service-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 40px 44px;
    color: #e07040;
    text-align: center;
    text-transform: uppercase;
    font: 600 40px/1 Magra, sans-serif;
    margin-top: 0.5em;
    margin-bottom: 2em;
}

.service-line {
    background-color: rgba(224, 112, 64, 0.4);
    align-self: stretch;
    width: 161px;
    max-width: 100%;
    height: 12px;
    margin: auto 0;
    flex-basis: 10%;
    transition: all 0.5ms ease-in;
}

.service-title {
    align-self: stretch;
    flex-basis: 60%;
    font: 600 40px / 1 Magra, sans-serif;
}
.service-header:hover .service-line
{
    flex-basis: 40%;
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