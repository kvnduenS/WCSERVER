<template>
  <div class="Info">
    <div class="left">
      <div class="left-info">
        <div class="picture">
          <img src="./assets/ME.jpg" width="100%" height="100%">
        </div>
          <h3>Duenas Kevin </h3>
      </div>

      <div class="contactInfo"></div>
        <h4 class="information"> Personal information</h4>
        <ul class="contact">
          <li>Name : Duenas, Kevin Brian A.</li>
          <li>Age : 20</li>
          <li>Birthday : September 25, 2001</li>
          <li>Address : Sta Ines betis Guauga Pampanga</li>
        </ul>

        <div class="contactInfo"></div>
          <h4 class="information"> Contact information</h4>
          <ul class="contact">
            <li>Email : duenaskevss@gmail.com</li>
            <li>School Email : kaduenas@student.hau.edu.ph</li>
            <li>Contact No. : 09451844716</li>
          </ul>

        </div>

        <div class="right">
          <div class="Skills">
              <h2 class="title">Skills</h2>
                <skills></skills>
          </div>
          <br>
          <div class="Language">
            <h2 class="title">Language </h2>
            <language></language>
          </div>
          <br>
          <div class="Hobbies">
            <h2 class="title">hobbies </h2>
            <hobbies></hobbies>
        </div>

        </div>
        </div>

</template>

<script>
//------------Imports--------------//
import Skills from './skills.vue'
import Language from './Language.vue'
import Hobbies from './hobbies.vue'
//---------------------------------//
export default {
  //--------Components---------//
  components: { 
    Skills,
    Language,
    Hobbies
    
},
  name: 'app',
  data () {
    return {
      msg: ''
    }
  }
}
      
</script>

<style>
*
{
    margin: 0;
    padding: 0;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
body {
    background-color: black;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
}
.Info {
    position: relative;
    width: 100%;
    max-width: 1000px;
    min-height: 1000px;
    margin: 50px;
    background-color: skyblue;
    display: grid;
    grid-template-columns: 1fr 2fr;
    box-shadow: 0 35px 55px rgb(90, 213, 250);
}
/***************************************************/
.Info .left {
    position: relative;
    background: black;
    padding: 40px;
}
.left-info{
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 20px;
    border-bottom: 2px solid black;
}
.picture {
    position: relative;
    width: 200px;
    height: 200px;
    border-radius: 45%;
    overflow: hidden;
}
.left-info h3 {
    color: white;
    font-size: 1.5em;
    margin-top: 20px;
    text-transform: uppercase;
    text-align: center;
    font-weight: 600;
    line-height: 1.4em;
}
.contactInfo {
    padding-top: 40px;
}
.contact {
    color: white;
    font-weight: 300;
    font-size: 18px;
    display: inline-block;
    
}
.information {
    color: white;
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 1px;
    margin-bottom: 20px;
}
/***************************************************/
.Info .right {
    position: relative;
    background: grey;
    padding: 40px;
}
.about {
    margin-bottom: 50px;
}
.title {
    color: whitesmoke;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 10px;
}
p {
    color: rgb(255, 253, 248);
}
ul {
    font-size: 20px;
    color: rgb(255, 255, 255);
    font-weight: 200;
    letter-spacing: 1px;
    margin-bottom: 20px;
}
</style>