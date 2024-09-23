<template>
  <div>
      <div class="contact-container">
        <!-- Left Side: Contact Information -->
        <div class="contact-info">
          <h2 class="title">Contact US</h2>
          <div class="info">
            <img src="../assets/address.jpg" class="info">
          </div>
          <div class="social-media">
            <h3>Follow us</h3>
            <div class="social-img">
              <img src="../assets/insta.png" alt="Instagram">
              <img src="../assets/you.png" alt="YouTube">
              <img src="../assets/twitter.png" alt="Twitter">
              <img src="../assets/face.png" alt="Facebook">
            </div>
          </div>
        </div>
    
        <!-- Right Side: Contact Form -->
        <section class="contact-form">
          <div class="form-container">
            <h2 class="form-title">Send a Message</h2>
            <form @submit.prevent="submitForm">
              <div class="name-fields">
                <div class="input-group name-field">
                  <label for="firstName">First Name</label>
                  <input type="text" id="firstName" v-model="firstName" class="input-field" placeholder="First Name" required>
                </div>
                <div class="input-group name-field">
                  <label for="lastName">Last Name</label>
                  <input type="text" id="lastName" v-model="lastName" class="input-field" placeholder="Last Name" required>
                </div>
              </div>
              <div class="input-group">
                <label for="email">Email</label>
                <input type="email" id="email" v-model="email" class="input-field" placeholder="Enter Your Email" required>
              </div>
              <div class="input-group">
                <label for="phone">Phone</label>
                <div class="phone-input">
                  <span class="country-code">+91</span>
                  <input type="tel" id="phone" v-model="phone" class="input-field" placeholder="Enter Phone Number" required>
                </div>
              </div>
              <div class="input-group">
                <label for="message">Message</label>
                <textarea id="message" v-model="message" class="input-field message-area" placeholder="Type Message..." required></textarea>
              </div>
              <button type="submit" class="submit-button">Submit <span class="arrow">➔</span></button>
            </form>
          </div>
        </section>
      </div>
    
    
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

.contact-container {
  display: flex;
  padding-top: 50px;
  padding-bottom: 60px;
  /*justify-content: space-between;
  align-items: flex-start;
  padding: 40px;
  */
  flex-direction:row ;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 20px;
  width: 90%;
  /*max-width: 1200px;*/
  margin: 0 auto;
  margin-top: 4em;
  box-sizing: border-box;
  /*flex-wrap: wrap;*/
}

.contact-info {
  margin-left: 10%;
  margin-right: 40px;
  flex-basis: 35%;
  padding: 0em 4em;
  /*min-width: 250px;*/
  box-sizing: border-box;
}

.contact-info h2 {
  color: #e07040;
  font-family: "Magra", sans-serif;
  font-size: 48px;
  font-weight: 700;
  text-align: center;
  margin-bottom: 20px;
}

.info {
  margin-top: 20px;
  font-size: 16px;
  line-height: 1.5;
}

.social-media {
  margin-top: 30px;
}

.social-img {
  display: flex;
  gap: 10px;
  margin-top: 10px;
}

.social-media h3 {
  color: #e07040;
  font-family: "Magra-Bold", Helvetica;
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 10px;
}

.contact-form {
  width: 100%;
  flex-basis: 60%;
  /*max-width: 698px;*/
  margin: 0 auto;
  /*display: flex;
  justify-content: center;
  box-sizing: border-box;*/
  padding: 20px;
}

.form-container {
  background-color: #E07040;
  border-radius: 20px;
  padding-right: 30px;
  width: 90%;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-title {
  color: #fff;
  font-family:'Magra', sans-serif;
  font-weight: bold;
  font-size: 48px;
  margin-bottom: 40px;
  padding-top: none;
  margin-top: none;
}

.name-fields {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  width: 100%;
}

.name-field {
  flex: 1;
}

.input-group {
  display: flex;
  flex-direction: column;
  width: 90%;
  margin-bottom: 20px;
  margin-left: 2em;
  margin-right: 30px;
  padding-top: 10px;
}

.input-group label {
  color: #fff;
  font-size: 15px;
  margin-bottom: 5px;
  padding-bottom: 5px;
  font-family: "Poppins-Regular", Helvetica;
}

.input-field {
  width: 90%;
  padding: 12px;
  border: none;
  border-radius: 10px;
  background-color: #fff;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.8);
}

.phone-input {
  display: flex;
  align-items: center;
  background-color: #fff;
  border-radius: 10px;
  padding: 0 10px;
  width: 90%;
  box-sizing: border-box;
}

.country-code {
  color: #000;
  font-size: 14px;
  margin-right: 5px;
}

.message-area {
  width: 80%;
  height: 107px;
  resize: vertical;
}

.submit-button {
  background-color: #fff;
  border: none;
  border-radius: 10px;
  color: rgba(0, 0, 0, 0.8);
  cursor: pointer;
  font-family: 'poppins',sans-serif;
  font-size: 16px;
  font-weight: 520;
  padding: 7px 30px;
  transition: background-color 0.3s ease;
  width: 36%;
  align-self: center;
  margin-top: 10px;
  margin-left: 11em;
  margin-bottom: 30px;
}

.submit-button:hover {
  background-color: #f0f0f0;
}

@media (max-width: 991px) {
  .contact-container {
    flex-direction: column;
    padding: 20px;
  }

  .contact-info, .contact-form {
    width: 100%;
    margin-bottom: 20px;
  }

  .form-container {
    padding: 20px;
  }

  .name-fields {
    flex-direction: column;
  }
}
input:focus {
    outline: none; /* Removes the default focus outline */
    box-shadow: none; /* Removes any custom focus shadow */
}
textarea:focus {
    outline: none; /* Removes the default focus outline */
    box-shadow: none; /* Removes any custom focus shadow */
}
.title
{
  position: relative;
}
.title::after
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
.title:hover::after
{
    width: 90%;
    cursor: pointer;
}
.submit-button
{
  transition: transform 0.3s ease;
}
.submit-button:hover
{
  transform: translateX(5px);
}


</style>