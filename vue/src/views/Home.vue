<template>

  <div id="parent">

    <div id="cloud-banner-div">
      <img
        class="cloud-banner"
        src="@/assets/cloudbannerfooter/cloudbanner.svg"
        alt="CloudBanner"
      />
    </div>

    <div id="animatedlogo">

    </div>

    <!-- <div id="logo-div">
      <img
        class="logo"
        src="@/assets/logo/cloudcode.svg"
        alt="CodeCatalog Logo"
        v-on:click.prevent="goHome"
      />
    </div> -->

    <div id="title">
      <h1>
      Code Out of Thin Air
    </h1>
    </div>

    <div id="site-catchphrase">
      <h4>Welcome to Code Cloud - your one-stop-shop for all things code!</h4>
    </div>

    <div id="site-desc">
      <p>The team created CodeCloud in order to help spread coding knowledge. We allow anyone and everyone to create their
          own account and upload coding examples for the entire world to see and learn from. On the other end of things we allow 
          anyone and everyone to download code examples from the CodeCloud so that they can use this new found knowledge for their
          own personal projects. We believe that we live in a time where coding is still a very underused and misunderstood skill.
          The more transparent coders are, the faster we will advance our knowledge and technology as a human race.
        </p>
    </div>

    <div id="site-functions">
      <h3>Site Functions</h3>
      <ul>
        <i class="fa-solid fa-droplet"></i>  Create an Account<br>
        <i class="fa-solid fa-droplet"></i>  Publish Code<br>
        <i class="fa-solid fa-droplet"></i>  Explore Code<br>
        <i class="fa-solid fa-droplet"></i>  Download Code<br>
      </ul>
    </div>

    <div id="MeetTeam">
      <h3>The Team</h3>
    </div> 

    <div id="team-row1">
      <div id="Misha">
        <h5>Misha Shatokhin</h5>
        <img
        class="misha-pic"
        src="@/assets/team/MS.jpg"
        alt="misha"
      />
      </div>
      <div id="aboutMisha">
        <ul>
          <i class="fa-solid fa-droplet"></i>  After graduating, from THE Ohio State University with a BS in Finance, I began developing my Analytical and Leadership skills 
          in a corporate financial analyst role where I worked with the finances of 13 individual holding companies. This later turned 
          into a controllership role where I oversaw all financial decisions for 1 of the 13 holding companies all while continuing my 
          responsibilities as the sole corporate financial analyst. I gained a plethora of knowledge in the finance, accounting and data 
          departments and have decided to pivot into a coding career.<br>
          <br>
          <i class="fa-solid fa-droplet"></i>  I began my new career path by learning about coding from various online sources prior to enrolling as a student in the .NET/C# 
          coding bootcamp at Tech Elevator. After graduation I plan on looking for a junior developer role where I will build upon my current 
          knowledge in the coding industry. I will be searching for innovative organizations that have a strong desire to grow both 
          technically and culturally.
        </ul>
      </div>
      <div id="Aidan">
        <h5>Aidan Wallace</h5>
        <img
        class="aidan-pic"
        src="@/assets/team/AW.jpg"
        alt="aidan"
      />
      </div>
      <div id="aboutAidan">
        <ul>
          <i class="fa-solid fa-droplet"></i>  Starting as a self-taught programmer, I've learned many modern tools in JavaScript, Python, and C#. Before attending a coding 
          boot camp with Tech Elevator, I took Python classes offered by Columbus State.<br><br>
          <i class="fa-solid fa-droplet"></i>  I started using my skills to learn tools around network security with Kali Linux, which gave me an idea of my own tools to make. 
          With my experience programming Raspberry Pi's, I applied my tools to a portable penetration testing tool.
        </ul>
        </div>
    </div>

    <div id="team-row2">
      <div id="Jack">
        <h5>Jack Updyke</h5>
        <img
        class="jack-pic"
        src="@/assets/team/JA.jpg"
        alt="jack"
      />
      </div>
      <div id="aboutJack">
        <ul>
          <i class="fa-solid fa-droplet"></i>  Hi, I’m Jack. I graduated from THE Ohio State University in 2018 with a bachelors in both Finance and Economics. During my time 
          at OSU, I always had a curiosity around software so I took a 1 year Data Analytics course where I had the opportunity to work on 
          2 semester long projects in a team setting and this experience pushed me into a career in software. Without the technical skills 
          to become a developer, my passion for software brought me to a career in Software Sales. After a few years spent in a Sales role 
          at various software companies, I decided it was time to shift my focus from selling software to building software applications. I 
          am currently a .NET bootcamp student at Tech Elevator with a desire to use my analytical skills as a foundation for a junior 
          developer role that allows me to collaborate with a team and continue to grow my coding skills.
        </ul>
      </div>
      <div id="Patrick">
        <h5>Patrick Arace</h5>
        <img
        class="patrick-pic"
        src="@/assets/team/PA.jpg"
        alt="patrick"
      />
      </div>
      <div id="aboutPatrick">
        <ul>
          <i class="fa-solid fa-droplet"></i>  My lifeblood: learning. Some favorite topics: music, math, languages, history.
          In the spirit of this project: the best mode in which to learn is to be willing to teach, and the best mode in which to teach is to always be open to learning.<br><br>
          <i class="fa-solid fa-droplet"></i>  A fascination: the symbiotic relationship emerging between humans and computers. Neither can be
          properly understood without the other now. Nature still bears many navigational clues around this field.<br><br>
          <i class="fa-solid fa-droplet"></i>  Things I'm working on: IPFS API in Elixir | p2p coffee review app in Clojure | machine learning program to analyze syntactic use of emoji in Mathematica.<br><br>
          <i class="fa-solid fa-droplet"></i> Motto: 坠落成星星 | Zhuìluò chéng xīngxīng | falling into stars
        </ul>
      </div>
    </div>
    <div id="cloud-footer-div">
      <img
        class="cloud-footer"
        src="@/assets/cloudbannerfooter/cloudbannerfooter.svg"
        alt="Cloudfooter"
      />
    </div>
  </div>

</template>

<script>
export default {
  name: "home",
  components: {
  },
  created() {},
};
</script>

<style scoped>

#parent  {
  display: grid;
  grid-template-columns: auto;
  grid-template-areas:
  "banner"
  "logo"
  "title"
  "site-catchphrase"
  "site-desc"
  "site-func"
  "team1"
  "team2"
  "footer";
}
/* -------------------------------------------------------------------- */
#cloud-banner-div{
  grid-area:"banner";
  display:flex;

  align-items: center;
  justify-content: center;
}
#cloud-banner-div img{
  max-height: 100vw;
}
/* -------------------------------------------------------------------- */
#animatedlogo{
  /* grid-area: "logo";
  display:fixed;
  justify-content: center;
  align-items: center; */

  width:50vw;
  height:40vh;

  background-image:url(../assets/animatedlogo/cloudcodeanimated1.svg);
  background-position: center;
  background-repeat:no-repeat;
  
  margin: 0 auto;
  animation: alternate 4s infinite ;
}
@keyframes alternate{
  3.2%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated2.svg);
  }
  6.4%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated3.svg);
  }
  9.6%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated4.svg);
  }
  12.8%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated5.svg);
  }
  16.1%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated6.svg);
  }
  19.3%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated7.svg);
  }
  22.5%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated8.svg);
  }
  25.7%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated9.svg);
  }
  28.9%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated10.svg);
  }
  32.2%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated11.svg);
  }
  35.4%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated12.svg);
  }
  38.6%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated12-5.svg);
  }
  41.8%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated13.svg);
  }
  45%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated14.svg);
  }
  48.3%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated15.svg);
  }
  51.5%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated16.svg);
  }
  54.7%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated17.svg);
  }
  57.9%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated18.svg);
  }
  61.1%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated19.svg);
  }
  64.4%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated20.svg);
  }
  67.6%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated21.svg);
  }
  70.8%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated22.svg);
  }
  74.%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated23.svg);
  }
  77.2%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated24.svg);
  }
  80.5%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated24-5.svg);
  }
  83.7%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated25.svg);
  }
  86.9%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated26.svg);
  }
  90.1%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated27.svg);
  }
  93.3%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated28.svg);
  }
  96.6%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated29.svg);
  }
  100%{
    background-image:url(../assets/animatedlogo/cloudcodeanimated30.svg);
  }
}
/* #logo-div{
  grid-area: "logo";
  display: flex;

  align-items: center;
  justify-content: center;

  padding-top: 0pt;
  padding-bottom: 10pt;
}
#logo-div img{
  border-radius: 5px;
  border-color: rgb(0, 150, 255);
  width: 55vh;
  box-shadow: 0 0 20px 3px rgb(0, 84, 147); 
}*/
/* -------------------------------------------------------------------- */
#title{
  grid-area: "title";
  display: flex;

  align-items: center;
  justify-content: center;
}
#title h1{
font-weight: bold;
}
/* -------------------------------------------------------------------- */
#site-catchphrase{
  grid-area: "site-catchphrase";
  display: flex;

  align-items: center;
  justify-content: center;
}
/* -------------------------------------------------------------------- */
#site-desc p{
  grid-area: "site-desc";
  display: flex;
                                /*COME BACK TO THIS*/
  align-items: center;
  justify-content: center;

  padding-left:150pt;
  padding-right:150pt;
}
/* -------------------------------------------------------------------- */
#site-functions{
  grid-area: "site-func";
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#site-functions h3{
  font-weight: bold;
  padding-top: 30pt;
  text-decoration: underline;
}
#site-functions ul{
  font-style: italic;
  justify-content: center;
}
/* -------------------------------------------------------------------- */
#MeetTeam{
  display: flex;
  align-items: center;
  justify-content: center;
}
#MeetTeam h3{
  font-weight: bold;
  text-decoration: underline;
  padding-top: 30pt;
}
/* -------------------------------------------------------------------- */
#team-row1{
  grid-area: "team1";
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row1 #Misha{
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row1 #Misha h5{
  font-weight: bold;
  font-style: italic;
}
#team-row1 #Misha img{
  width:25vh;
  padding-right: 20pt;
  padding-bottom: 25pt;
  margin-bottom: 15pt;

  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
#team-row1 #aboutMisha{
  font-style:italic;
  max-width: 100%;
  padding-right: 50pt;
  padding-left: 50pt;
  padding-top:10pt;

  border-radius: 5px;
  width: 95vh;
  box-shadow: 0 0 10px 3px rgb(0, 84, 147);
}
/* -------------------------- */
#team-row1 #Aidan{
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row1 #Aidan h5{
  padding-top: 20pt;
  font-weight: bold;
  font-style: italic;
}
#team-row1 #Aidan img{
  width:25vh;
  padding-right: 20pt;
  padding-bottom: 15pt;
  margin-bottom: 15pt;

  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
#team-row1 #aboutAidan{
  font-style:italic;
  max-width: 100%;
  padding-right: 50pt;
  padding-left: 50pt;
  padding-top:10pt;

  border-radius: 5px;
  width: 95vh;
  box-shadow: 0 0 10px 3px rgb(0, 84, 147);
}
/* -------------------------- */
#team-row2{
  grid-area: "team2";
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row2 #Jack{
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row2 #Jack h5{
  padding-top: 20pt;
  font-weight: bold;
  font-style: italic;
}
#team-row2 #Jack img{
  width:25vh;
  padding-right: 20pt;
  padding-bottom: 15pt;
  margin-bottom: 15pt;

  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
#team-row2 #aboutJack{
  font-style:italic;
  max-width: 100%;
  padding-right: 50pt;
  padding-left: 50pt;
  padding-top:10pt;

  border-radius: 5px;
  width: 95vh;
  box-shadow: 0 0 10px 3px rgb(0, 84, 147);
}
/* -------------------------- */
#team-row2 #Patrick{
  display: flex;
  flex-direction: column;

  align-items: center;
  justify-content: center;
}
#team-row2 #Patrick h5{
  padding-top: 20pt;
  font-weight: bold;
  font-style: italic;
}
#team-row2 #Patrick img{
  width:25vh;
  padding-right: 20pt;
  padding-bottom: 15pt;
  margin-bottom: 15pt;

  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
}
#team-row2 #aboutPatrick{
  font-style:italic;
  max-width: 100%;
  padding-right: 50pt;
  padding-left: 50pt;
  padding-top:10pt;

  border-radius: 5px;
  width: 95vh;
  box-shadow: 0 0 10px 3px rgb(0, 84, 147);
}
/* -------------------------- */
#cloud-footer-div{
  grid-area:"footer";
  display:flex;

  align-items: center;
  justify-content: center;
}
#cloud-footer-div img{
  max-height: 100vw;
  background-repeat:repeat;
}
</style>