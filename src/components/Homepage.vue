<template>
  <div class="homepage">
    <section
      class="banner-area relative"
      id="section01"
      data-parallax="scroll"
      data-image-src="img/header-bg.jpg"
    >
      <div class="overlay-bg overlay"></div>
      <div class="container">
        <div id="intro">
          <div
            class="row fullscreen  d-flex align-items-center justify-content-left"
            style="height: 900px;"
          >
            <div class="banner-content col-lg-6 col-md-6">
              <img
                src="../assets/newlogo.png"
                height="150"
              />
              <h9>
                A centralised, data driven platform that empowers you with
                visuals to make more informed decisions.
              </h9>
              <br />
              <br />
              <h3>
                Click me to explore different modules and career prospects in
                greater details!
              </h3>
              <a
                class="btn btn-default btn-lg"
                @click="$router.push({ path: '/module' });"
                role="button"
                ><i class="fas fa-book mr-2"></i>Modules</a
              >
              <a
                class="btn btn-default btn-lg"
                @click="$router.push({ path: '/careerview' });"
                role="button"
                ><i class="fas fa-graduation-cap mr-2"></i>Career</a
              >
              <br />
              <br />
              <h1 style="color:white" @click="scroll">Find out more!</h1>
              <a ><span @click="scroll"></span></a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="service-area pt-100 pb-100" id="section02">
      <div class="generalinfo">
        <div class="container">
          <div class="row d-flex justify-content-center">
            <div class="menu-content pb-70 col-lg-8">
              <div class="title text-center">
                <br />
                <br />
                <br />
                <h2 class="mb-10">
                  <b><font size="7">Why VirtualSenpai! ?</font></b>
                </h2>
                <br />
                <br />
              </div>
            </div>
          </div>
        </div>
        <b></b> <b></b>
        <div class="row">
          <div class="sigle-service col-lg-4 col-md-6">
            <i class="fas fa-question mr-2 fa-2x"></i> <br />
            <h4>Huge dilemma</h4>
            <p>
              Find yourself constantly revolving around seniors' advices
              regarding academic matters? Unsure of which senior's advice to
              follow?
            </p>
          </div>
          <div class="sigle-service col-lg-4 col-md-6">
            <i class="fas fa-lightbulb-o mr-2 fa-2x"></i> <br />
            <h4>Unequal access to information</h4>
            <p>
              Based on our survey results, many students rely on seniors for
              advice yet not all students have seniors to turn to! Knowing more
              seniors give students an unfair advantage in terms of unequal
              access to information and we want to eradicate this information
              inequality!
            </p>
          </div>
          <div class="sigle-service col-lg-4 col-md-4">
            <i class="fas fa-thumbs-down mr-2 fa-2x"></i> <br />
            <h4>Unreliable and ineffective source of information</h4>
            <p>
              Enough of searching for information online just to find that they
              are of little help? Worrying that this information might also be
              unreliable?
            </p>
          </div>
        </div>
      </div>
    </section>
    <section>
      <section class="team-area section-gap" id="team">
        <div class="presentedby">
          <div class="container">
            <div class="row d-flex justify-content-center">
              <div class="menu-content pb-70 col-lg-8">
                <div class="title text-center">
                  <br />
                  <br />
                  <br />
                  <h2 class="mb-10">
                    VirtualSenpai! is proudly presented to you by Team Lambda!
                  </h2>
                  <br />
                </div>
              </div>
            </div>
            <div class="row justify-content-center d-flex align-items-center">
              <div class="col-md-4 single-team">
                <div class="team-member">
                  <img
                    class="mx-auto rounded-circle"
                    src="../assets/zh.jpg"
                    alt=""
                  />
                  <div
                    class="align-items-center justify-content-center d-flex"
                  ></div>
                </div>
                <div class="meta-text mt-30 text-center"><h4>Zhe Hao</h4></div>
              </div>
              <div class="col-md-4 single-team">
                <div class="team-member">
                  <img
                    class="mx-auto rounded-circle"
                    src="../assets/tricia.jpeg"
                    alt=""
                  />
                  <div
                    class="align-items-center justify-content-center d-flex"
                  ></div>
                </div>
                <div class="meta-text mt-30 text-center"><h4>Tricia</h4></div>
              </div>
              <div class="col-md-4 single-team">
                <div class="team-member">
                  <img
                    class="mx-auto rounded-circle"
                    src="../assets/wulin.jpg"
                    alt=""
                  />
                  <div
                    class="align-items-center justify-content-center d-flex"
                  ></div>
                </div>
                <div class="meta-text mt-30 text-center"><h4>Wulin</h4></div>
              </div>
              <div class="col-md-4 single-team">
                <div class="team-member">
                  <img
                    class="mx-auto rounded-circle"
                    src="../assets/chiran.jpeg"
                    alt=""
                  />
                  <div
                    class="align-items-center justify-content-center d-flex"
                  ></div>
                </div>
                <div class="meta-text mt-30 text-center"><h4>Chiran</h4></div>
              </div>
              <div class="col-md-4 single-team">
                <div class="team-member">
                  <img
                    class="mx-auto rounded-circle"
                    src="../assets/yy.jpg"
                    alt=""
                  />
                  <div
                    class="align-items-center justify-content-center d-flex"
                  ></div>
                </div>
                <div class="meta-text mt-30 text-center">
                  <h4>Ying Yang</h4>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </section>
  </div>
</template>
<script>
import { Btn, Fa } from "mdbvue";
import image from "../assets/clouds-cold-dark-540518.png";


export default {
  components: {
    Btn,
    Fa,
    image
  },
  methods:{
    scroll(){
      let element = document.getElementById("section02");
      element.scrollIntoView({behavior: "smooth", block: "start", inline: "nearest"});
    }
  }
  ,data() {
    return {
    };
  }
};
</script>

<style scoped>
.row {
  display: flex;
  flex-wrap: wrap;
  margin-right: -15px;
  margin-left: -15px;
  padding: 0;
}
.generalinfo {
  background: rgba(255, 255, 255, 255);
  opacity: 1;
  border-radius: 3px;
  margin-top: 0px;
  position: relative;
  width: 100%;
  height: 450px;
  padding: 0;
}
.info {
  background: rgba(255, 255, 255, 0.18);
  border-radius: 3px;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.25);
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  margin-top: 0px;
  text-align: centre;
  position: relative;
  margin-left: 0px;
  margin-right: 0px;
  right: 0;
  z-index: 2;
  padding: 0 px;
  width: 100%;
}

.content {
  background: rgba(255, 255, 255, 0.35);
  border-radius: 3px;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.25);
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  margin-top: 150px;
  left: 0;
  position: relative;
  margin-left: 20px;
  margin-right: 20px;
  right: 0;
  z-index: 2;
  padding: 0 10px;
  width: 700px;
}

.explore {
  background: rgba(255, 255, 255, 0.35);
  opacity: 1;
  border-radius: 3px;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.25);
  font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
  margin-top: 200px;
  left: 0;
  position: relative;
  margin-left: 0%;
  margin-right: 20px;
  right: 0;
  z-index: 2;
  padding: 0 10px;
  width: 100%;
}

.presentedby {
  background: rgba(255, 255, 255, 255);
  opacity: 0.9;
  border-radius: 3px;
  margin-top: 0px;
  position: relative;
  width: 100%;
  height: 750px;
}
h9 {
  font-weight: bold;
  color: #fff;
  font-size: 24px;
}
h2 {
  font-weight: bold;
  font-size: 30px;
}
h3 {
  font-weight: bold;
  color: #fff;
  font-size: 18px;
}

.img-fluid {
  max-width: 100%;
  height: auto;
}
.team-member img {
  width: 225px;
  height: 225px;
  border: 7px solid #fff;
  opacity: 1;
}
.fa.fa-question {
  font-size: 70px;
}
.banner-content {
  position: relative;
  left: -100px;
  top: -65px;
}
.btn {
  border: 1.5px solid white;
  border-radius: 10px;
  background-color: #fff;
}
#section01 a span {
  position: absolute;
  top: 100%;
  left: 50%;
  width: 24px;
  height: 24px;
  margin-left: -12px;
  border-left: 1px solid #fff;
  border-bottom: 1px solid #fff;
  -webkit-transform: rotate(-45deg);
  transform: rotate(-45deg);
  box-sizing: border-box;
}


</style>
