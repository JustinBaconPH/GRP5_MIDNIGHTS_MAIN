<script setup>
import NavBar from '@/components/GuestNavBar.vue';
import Footers from '@/components/Footers.vue';
import { RouterLink } from 'vue-router';
</script>

<template>
  <main>
    <NavBar />
    <div class="background">
      <div class="opacity-black-screen">
        <div class="business-logo-container">
          <img src="/assets/midnights-logo.png" alt="" class="business-logo">
        </div>
      </div>
    </div>



    <div class="review-profile">
      <div class="name-container">
        <div class="contact-us-content">
          <p>Contact Us</p>
        </div>
        <p class="details">Address:</p>
        <br>
        <p class="details">22 Mindanao, Malanday, Marikina, Philippines, 1805</p>
        <br>
        <br>
        <br>
        <p class="details">Email:</p>
        <br>
        <p class="details">midnightsmobilebar@gmail.com</p>
        <br>
        <br>
        <br>
        <p class="details">Contact Number:</p>
        <br>
        <p class="details">0968 861 1813 | 0906 001 4517 </p>
        <br>
        <br>
        <br>
        <div class="inquire-button-content">
          <a href="https://www.facebook.com/messages/t/105219017745645" class="button">Inquire Now</a>
        </div>
      </div>
      <div class="profile-container">
        <img src="/assets/contact us.jpg" alt="" class="user-pic" />
      </div>
    </div>



    <Footers />
  </main>

</template>

<style scoped>
main {
  background-color: #000;
  min-height: 100vh;
  height: auto;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

.background {
  background-image: url('/assets/midnights-bg.jpg');
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: cover;
  min-height: 100vh;
}

.business-logo-container {
  height: 45rem;
  width: 68rem;
}

.business-logo {
  height: 100%;
  width: 100%;
  object-fit: contain;
}



.opacity-black-screen {
  background-color: rgb(0, 0, 0, 0.8);
  /*opacity */
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
}

p {
  color: #fff;
}

.about-us-content,
.about-us-content-2 {
  text-align: center;
  margin: auto;
  min-height: 2rem;
  margin-top: 4rem;
  margin-bottom: rem;
  font-weight: bold;
  font-size: 3rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  color: #fff;
  background-color: transparent;
  height: auto;

}

.about-us-content-2 {
  margin-top: 10rem;
  margin-bottom: 5rem;
}

.about-us-text,
.about-us-text-2 {
  text-align: center;
  margin: auto;
  margin-left: 20rem;
  margin-right: 20rem;
  height: auto;
  font-weight: bold;
  font-size: 1.5rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  margin-bottom: 4rem;
  height: auto;
}

.gallery-container,
.review-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  margin-top: 2rem;
  background-color: transparent;
  width: 90%;
  margin: auto;
  margin-bottom: 1.2rem;
  padding: 2rem
}

.review-container {
  background-color: transparent;
  height: auto;
  justify-content: center;
}

.gallery-item {
  height: 30rem;
  padding: 0;
  position: relative;
  /*overflow: hidden;*/
  justify-content: space-around;
  background-color: transparent;
  flex: 1;
  /* border: 1px solid #000; */
  margin: 0 0.8rem;
}

.gallery-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 30px;

}

.review-box {
  border: 0.1rem solid #FFF;
  display: flex;
  flex: 1;
  justify-content: center;
  border-radius: 2rem;
  margin: 0.8rem;
  flex-direction: column;
  padding: 1.2rem;
}

.review-ratings-container {
  flex: 1;
  background-color: transparent;
  margin-top: 1rem;
}

.review-comment {
  font-weight: bold;
  color: #FFF;
  font-size: 1.2rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  margin-top: 2rem;
  line-height: 1.4;
}

.review-profile {
  flex: 5;
  /* border: 1px solid #fff; */
  display: flex;
  flex-direction: row;
  margin-top: 1.5rem;
  background-size: cover;
  height: 100%;
  width: 100%;
  margin-top: 10rem;
  margin-left: 1.5rem;
  margin-bottom: 1rem;
}

.profile-container {
  flex: 1s;
  background-color: transparent;
  display: flex;
  height: 100%;
  width: 50%;


}

.name-container {
  flex: 0.9;
  /* background-color:pink; */
  padding: 0 0 0 3rem;
  /*top, right, bottom, left*/
  font-family: 'Poppins', 'Montserrat', sans-serif;
  font-weight: bold;
  justify-content: center;
  flex-direction: column;
  display: flex;

}

.name-container>p {
  padding: 0 0;
  margin: 0;
  /* border:1px solid #000; */
  background-color: transparent;
  font-weight: bold;
  font-size: 1.3rem;
  line-height: 1.8rem;
}

.user-pic {
  margin: 0 0 0 10rem;
  height: 43rem;
  width: 43rem;
  border-radius: 2rem;
  background-image: cover;
  justify-content: center;
  align-items: center;
}

.client {
  font-weight: normal;
}

.review-star {
  margin-right: 0.3rem;
}

.button {
  text-decoration: none;
  color: #fff;
  font-size: 1.3rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  border: 1px solid #fff;
  padding: 1rem 2rem 1rem 2rem;
  border-radius: 0.5rem;
  height: 1rem;
  cursor: pointer;
  transition: background-color linear 0.3s, color linear 0.3s;
}

.button:hover {
  background-color: #7f8080;
}

.inquire-content {
  background-image: url('/assets/inquire2.jpg');
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: 100%;
  /* or specify a fixed size, e.g., 50% */
  align-items: center;
  justify-content: center;
}


.inquire-logo-container {
  height: 5rem;
  width: 5rem;
}

.inquire-black-screen {
  background-color: rgb(0, 0, 0, 0.8);
  /*opacity */
  height: 100vh;
  width: 100;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  font-size: 2.5rem;
}

.inquire-text {
  font-family: 'Poppins', 'Montserrat', sans-serif;
  font-size: 3.5rem;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  width: 90%;
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.reviews-button-content {
  text-align: center;
  margin: auto;
  min-height: 8rem;
  margin-top: 2rem;
  margin-bottom: 3rem;
  font-weight: bold;
  font-size: 2.5rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  color: #fff;
  background-color: transparent;
  height: auto;

}

.inquire-button-content {
  align-items: left;

  margin: auto;
  min-height: 8rem;
  margin-top: 2rem;
  margin-bottom: 3rem;
  font-weight: bold;
  font-size: 2.5rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  color: #fff;
  background-color: transparent;
  height: auto;

}

.contact-us-content {



  font-weight: bold;
  font-size: 3rem;
  font-family: 'Poppins', 'Montserrat', sans-serif;
  color: #fff;
  background-color: transparent;

}

@media only screen and (max-width:1000px) {
  nav {
    background-color: red;
  }
}

@media only screen and (max-width:800px) {
  nav {
    background-color: yellow;
  }

}
</style>
