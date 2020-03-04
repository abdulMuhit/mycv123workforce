<template>
  <v-app id="main">
    <v-card>
      <v-card-title class="header">
        <div class="wrap-image">
          <div class="wrap-inside" :style="{'background-image': 'url(/img/foto_p1.jpeg)'}"></div>
        </div>
        <div class="wrap-text">
          <h1 class="name">Abdul Muhit T.</h1>
          <p class="title">Web developer</p>
        </div>

        <div class="medsos-main">
          <div class="medsos">
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_loc.svg)'}"></div>
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_gplus.svg)'}"></div>
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_linked.svg)'}"></div>
          </div>

          <div class="medsos2">
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_wa.svg)'}"></div>
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_be.svg)'}"></div>
            <div class="meditem" :style="{'background-image': 'url(/img/icons/icon_dribble.svg)'}"></div>
          </div>
        </div>

        <div class="email">
          <div class="medemail" :style="{'background-image': 'url(/img/icons/icon_email.svg)'}"></div>
          <div class="medpdf" :style="{'background-image': 'url(/img/icons/icon_pdf.svg)'}"></div>
        </div>
      </v-card-title>
      <v-tabs v-model="tab" background-color="transparent" grow>
        <v-tab v-for="item in items" :key="item">{{ item }}</v-tab>
      </v-tabs>
      <v-tabs-items v-model="tab">
        <!--    <v-tab-item v-for="item in items" :key="item">
          <v-card flat>
            <v-card-text>{{ text }}</v-card-text>
          </v-card>
        </v-tab-item>-->

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <h2 class="about-t">About</h2>
              <p
                class="about-p"
              >A Fullstack JavaScript developer, using vue, nuxt, express.js (node.js), with more than 2 years experience.</p>
            </v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <h2 class="about-t">Portfolio</h2>

              <div class="images-portfolio">
                <div class="image-p">
                  <img src="/img/porto1.png" alt="porto1" />
                </div>
                <div class="image-p">
                  <img src="/img/porto2.png" alt="porto2" />
                </div>
                <div class="image-p">
                  <img src="/img/porto3.png" alt="porto3" />
                </div>
              </div>
            </v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <div class="resume-section-content">
                <div class="resume-timeline position-relative">
                  <article class="resume-timeline-item position-relative pb-5">
                    <div class="resume-timeline-item-header mb-2">
                      <div class="d-flex flex-column flex-md-row">
                        <h3 class="resume-position-title font-weight-bold mb-1">
                          Freelance Web
                          Developer
                        </h3>
                        <div class="resume-company-name ml-auto">
                          <ul>
                            <li>
                              <a
                                href="https://insta-nuxt-clone.herokuapp.com"
                                target="_blank"
                                rel="noopener noreferrer"
                              >
                                Sample Project
                                Insta Store
                              </a>
                            </li>
                            <li>
                              <a
                                href="http://www.tizenstore.com/main/getDetail.as?Id=hmAptON8fe"
                                target="_blank"
                                rel="noopener noreferrer"
                              >
                                Sample Project
                                Kang Parkir
                              </a>
                            </li>
                          </ul>
                        </div>
                      </div>
                      <!--//row-->
                      <div class="resume-position-time">March 2020 - now</div>
                    </div>

                    <!--//resume-timeline-item-header-->
                    <div class="resume-timeline-item-desc">
                      <p>Build some webapp Project</p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">Achievements:</h4>
                      <p class="h6">
                        <strong>Mockup Insta Store</strong>
                      </p>
                      <ul>
                        <li>Adding responsive web page</li>
                        <li>Adding PWA technology.</li>
                      </ul>
                      <p class="h6">
                        <strong>Tizen Store Kang Parkir</strong>
                      </p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Technologies
                        used:
                      </h4>
                      <ul class="list-inline">
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Vue</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Nuxt</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">
                            Node.js
                            (express.js)
                          </span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">socket.io</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">HTML/SASS</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">mongo db</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">PostgreSql</span>
                        </li>
                      </ul>
                    </div>
                    <!--//resume-timeline-item-desc-->
                  </article>
                  <article class="resume-timeline-item position-relative pb-5">
                    <div class="resume-timeline-item-header mb-2">
                      <div class="d-flex flex-column flex-md-row">
                        <h3 class="resume-position-title font-weight-bold mb-1">
                          Front End Web
                          Developer
                        </h3>
                        <div class="resume-company-name ml-auto">
                          <ul>
                            <li>
                              <a
                                href="https://m.bandros.co.id"
                                target="_blank"
                                rel="noopener noreferrer"
                              >m.bandros.co.id</a>
                            </li>
                          </ul>
                        </div>
                      </div>
                      <!--//row-->
                      <div class="resume-position-time">February 2018 - February 2020</div>
                    </div>

                    <!--//resume-timeline-item-header-->
                    <div class="resume-timeline-item-desc">
                      <p>Built some dropship e-commerce webapp for member of bandros.co.id.</p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">Achievements:</h4>
                      <p>Rebuilt front web page from bandros ver 3 to bandros ver 4.0.0</p>
                      <ul>
                        <li>Adding responsive web page</li>
                        <li>Adding PWA technology.</li>
                        <li>Using socket.IO for realtime discussion feature.</li>
                      </ul>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Technologies
                        used:
                      </h4>
                      <ul class="list-inline">
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Vue</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Nuxt</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Node.js</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">socket.io</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">HTML/SASS</span>
                        </li>
                      </ul>
                    </div>
                    <!--//resume-timeline-item-desc-->
                  </article>
                  <!--//resume-timeline-item-->
                  <article class="resume-timeline-item position-relative pb-5">
                    <div class="resume-timeline-item-header mb-2">
                      <div class="d-flex flex-column flex-md-row">
                        <h3 class="resume-position-title font-weight-bold mb-1">
                          Freelancer
                          Web
                          Developer
                        </h3>
                        <div class="resume-company-name ml-auto">
                          <ul>
                            <li>
                              <a
                                href="https://www.assemblrworld.com"
                                target="_blank"
                                rel="noopener noreferrer"
                              >https://www.assemblrworld.com</a>
                            </li>
                            <li>
                              <a
                                href="https://tender-bhaskara-2bc85d.netlify.com/"
                                target="_blank"
                                rel="noopener noreferrer"
                              >
                                Sample Project
                                webapp assemblr
                              </a>
                            </li>
                          </ul>
                        </div>
                      </div>
                      <!--//row-->
                      <div class="resume-position-time">November 2019 - Desember 2019</div>
                    </div>
                    <!--//resume-timeline-item-header-->
                    <div class="resume-timeline-item-desc">
                      <p>
                        Handle some minor change in the app, with some webview technology that
                        embed to android / ios app.
                      </p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">Achievements</h4>

                      <ul>
                        <li>Adding some books page</li>
                        <li>Adding some view page fix</li>
                        <li>Adding some bugs fix</li>
                      </ul>

                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Technologies
                        used:
                      </h4>
                      <ul class="list-inline">
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Vue</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Firebase</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">HTML/SASS</span>
                        </li>
                      </ul>
                    </div>
                    <!--//resume-timeline-item-desc-->
                  </article>
                  <!--//resume-timeline-item-->

                  <article class="resume-timeline-item position-relative pb-5">
                    <div class="resume-timeline-item-header mb-2">
                      <div class="d-flex flex-column flex-md-row">
                        <h3 class="resume-position-title font-weight-bold mb-1">
                          Android
                          Developer
                        </h3>
                        <div class="resume-company-name ml-auto">
                          <a
                            href="https://play.google.com/store/apps/details?id=com.bandros&hl=en"
                            target="_blank"
                            rel="noopener noreferrer"
                          >
                            bandros Android
                            App
                          </a>
                        </div>
                      </div>
                      <!--//row-->
                      <div class="resume-position-time">February 2018 - Mei 2018</div>
                    </div>
                    <!--//resume-timeline-item-header-->
                    <div class="resume-timeline-item-desc">
                      <p>Responsible to maintenance and fixing some bugs in bandros android app.</p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">Achievements</h4>

                      <ul>
                        <li>Adding some bandros video education page</li>
                        <li>Make some view pages fix</li>
                        <li>Make some bugs fix</li>
                      </ul>

                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Technologies
                        used:
                      </h4>
                      <ul class="list-inline">
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Java</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Sqlite</span>
                        </li>
                      </ul>
                    </div>
                    <!--//resume-timeline-item-desc-->
                  </article>
                  <!--//resume-timeline-item-->

                  <article class="resume-timeline-item position-relative">
                    <div class="resume-timeline-item-header mb-2">
                      <div class="d-flex flex-column flex-md-row">
                        <h3 class="resume-position-title font-weight-bold mb-1">
                          Learning &
                          Challenge Hunter
                        </h3>

                        <div class="resume-company-name ml-auto">
                          <a
                            href="https://www.dicoding.com/users/2128"
                            target="_blank"
                            rel="noopener noreferrer"
                          >dicoding.com</a>
                        </div>
                      </div>
                      <!--//row-->
                      <div class="resume-position-time">Maret 2015 - Now</div>
                    </div>
                    <!--//resume-timeline-item-header-->
                    <div class="resume-timeline-item-desc">
                      <p>
                        Take a part in online programming course at dicoding.com (dicoding
                        academy) and get some IT certificate. I also join their challenge
                        program (dicoding challenge) to test my skill and also win some awards
                        and prizes.
                      </p>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Learning
                        Achievements
                      </h4>

                      <ul>
                        <li>(2016) Learn to build Android App HTML5, dicoding.com</li>
                        <li>(2017) Learn to build LINE ChatBot, dicoding.com</li>
                        <li>
                          (2017) Learn to build android app with IBM Bluemix,
                          dicoding.com
                        </li>
                        <li>(2017) Learn to build android app for beginner, dicoding.com</li>
                        <li>(2017) Learn to build android app for Expert, dicoding.com</li>
                      </ul>

                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Awards
                        Achievements
                      </h4>
                      <ul>
                        <li>
                          <div class="resume-award-name">
                            Tizen Thematic Challenges - Tools
                            <a
                              href="http://www.tizenstore.com/main/getDetail.as?Id=FiPyYQTTJm"
                              target="_blank"
                              rel="noopener noreferrer"
                            >Morse Code</a>
                          </div>
                          <div class="resume-award-desc">by Samsung Indonesia</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            DBS Live More Society: Developer
                            Challenge
                            <a
                              href="http://www.tizenstore.com/main/getDetail.as?Id=FiPyYQTTJm"
                              target="_blank"
                              rel="noopener noreferrer"
                            >Morse Code</a>
                          </div>
                          <div class="resume-award-desc">by DBS Indonesia</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            Indonesia Next Apps 4.0 – Tizen
                            Smartphone
                            Challenge
                            <a
                              href="http://www.tizenstore.com/main/getDetail.as?Id=FiPyYQTTJm"
                              target="_blank"
                              rel="noopener noreferrer"
                            >Morse Code</a>
                          </div>
                          <div class="resume-award-desc">by dicoding</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            Tizen Thematic Challenges - Puzzle
                            Games
                            <a
                              href="http://www.tizenstore.com/main/getDetail.as?Id=BqPsgjNzlZ"
                              target="_blank"
                              rel="noopener noreferrer"
                            >Oei Takuzu</a>
                          </div>
                          <div class="resume-award-desc">by Samsung Indonesia</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            LINE Bot Developer Challenge -
                            Cuacaku
                          </div>
                          <div class="resume-award-desc">by LINE Indonesia</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            Dicoding Web Master - Data
                            Transportasi Laut
                            Perprovinsi di tahun 2009
                          </div>
                          <div class="resume-award-desc">by dicoding</div>
                        </li>

                        <li>
                          <div class="resume-award-name">
                            Mobile Game Developer Challenge
                            Professional -
                            Run Chibis Run!
                          </div>
                          <div class="resume-award-desc">by intel Indonesia</div>
                        </li>
                      </ul>
                      <h4 class="resume-timeline-item-desc-heading font-weight-bold">
                        Technologies
                        used:
                      </h4>
                      <ul class="list-inline">
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">JavaScript</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Apache Cordova</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">HTML/SCSS</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Restfull API</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">IBM bluemix</span>
                        </li>
                        <li class="list-inline-item">
                          <span class="badge badge-primary badge-pill">Tizen Technology</span>
                        </li>
                      </ul>
                    </div>
                    <!--//resume-timeline-item-desc-->
                  </article>
                  <!--//resume-timeline-item-->
                </div>
                <!--//resume-timeline-->
              </div>
            </v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <section class="resume-section education-section mb-5">
                <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Education</h2>
                <div class="resume-section-content">
                  <ul class="list-unstyled">
                    <li>
                      <div class="resume-degree font-weight-bold">Learn to build PWA</div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2018</div>
                    </li>
                    <li>
                      <div class="resume-degree font-weight-bold">
                        Learn to build Android app for
                        Expert
                      </div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2017</div>
                    </li>
                    <li>
                      <div class="resume-degree font-weight-bold">
                        Learn to build Android App for
                        Beginner
                      </div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2017</div>
                    </li>
                    <li>
                      <div class="resume-degree font-weight-bold">
                        Learn to build Android App with IBM
                        bluemix
                      </div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2017</div>
                    </li>
                    <li>
                      <div class="resume-degree font-weight-bold">Learn to build LINE ChatBot</div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2017</div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-degree font-weight-bold">Learn to build Android HTML5 App</div>
                      <div class="resume-degree-org">dicoding.com</div>
                      <div class="resume-degree-time">2016</div>
                    </li>
                  </ul>
                </div>
              </section>
              <!--//education-section-->
            </v-card-text>
          </v-card>
        </v-tab-item>

        <v-tab-item>
          <v-card flat>
            <v-card-text>
              <div class="resume-section-content">
                <div class="resume-skill-item">
                  <h4 class="resume-skills-cat font-weight-bold">Frontend</h4>
                  <ul class="list-unstyled mb-4">
                    <li class="mb-2">
                      <div class="resume-skill-name">Vue</div>
                      <div class="progress resume-progress">
                        <v-progress-linear value="90"></v-progress-linear>
                      </div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">Nuxt</div>
                      <div class="progress resume-progress">
                        <v-progress-linear value="90"></v-progress-linear>
                      </div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">JavaScript</div>
                      <div class="progress resume-progress">
                        <v-progress-linear value="90"></v-progress-linear>
                      </div>
                    </li>

                    <li class="mb-2">
                      <div class="resume-skill-name">HTML/CSS/SASS</div>
                      <div class="progress resume-progress">
                        <v-progress-linear value="80"></v-progress-linear>
                      </div>
                    </li>
                  </ul>
                </div>
                <!--//resume-skill-item-->

                <div class="resume-skill-item">
                  <h4 class="resume-skills-cat font-weight-bold">Backend</h4>
                  <ul class="list-unstyled">
                    <li class="mb-2">
                      <div class="resume-skill-name">Node.js</div>

                      <v-progress-linear value="70"></v-progress-linear>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">Golang</div>
                      <v-progress-linear value="50"></v-progress-linear>
                    </li>
                  </ul>
                </div>
                <!--//resume-skill-item-->
              </div>
            </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs-items>
    </v-card>
  </v-app>
</template>
<script>
export default {
  name: "App",
  data: () => ({
    tab: null,
    items: ["About", "PortFolio", "Work", "Education", "Skills"],
    text:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
  })
};
</script>

<style lang="scss">
* {
  font-family: "Open Sans", sans-serif;
}

.header {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  background: #1d1d1d;
  box-shadow: 0px 6px 30px rgba(0, 0, 0, 0.12);

  .wrap-image {
    .wrap-inside {
      display: block;
      width: 185px;
      height: 185px;
      background-color: #edeff2;
      border-radius: 50%;
      background-repeat: no-repeat;
      background-position: center center;
      background-size: cover;
    }
  }

  .wrap-text {
    .name {
      font-weight: 600;
      font-size: 22px;
      line-height: 30px;
      color: #ffffff;
    }

    .title {
      font-size: 12px !important;
      line-height: 16px;
      color: #ffffff;
    }
  }

  .medsos-main {
    display: flex;
    justify-content: space-between;
  }

  .medsos {
    display: grid;
    grid-template: 20px 20px / repeat(3, 43%);
    text-align: center;
    margin-top: 37px;
    margin-right: 50px;

    .meditem {
      display: block;
      width: 37px;
      height: 37px;
      background-color: #edeff2;
      border-radius: 50%;
      background-position: center center;
      margin-right: 5px;
    }
  }

  .medsos2 {
    display: grid;
    grid-template: 20px 20px / repeat(3, 43%);
    text-align: center;
    margin-top: 37px;

    .meditem {
      display: block;
      width: 37px;
      height: 37px;
      background-color: #edeff2;
      border-radius: 50%;
      background-position: center center;
      margin-right: 5px;
    }
  }

  .email {
    display: flex;
    flex-basis: 100%;
    margin-top: 37px;
    justify-content: center;

    .medemail {
      display: block;
      width: 52px;
      height: 52px;
      background-color: #edeff2;
      border-radius: 50%;
      background-position: center center;
      margin-right: 10px;
    }

    .medpdf {
      display: block;
      width: 52px;
      height: 52px;
      background-color: #000000;
      border-radius: 50%;
      background-position: center center;
      margin-right: 10px;
    }
  }
}

.header > div {
  margin-right: 10px;
}

.about-t {
  margin-top: 37px;
  font-weight: 600;
  font-size: 18px;
  line-height: 25px;
  color: #1d1d1d;
}

.about-p {
  margin-top: 27px;
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 19px;
  color: #1d1d1d;
}

.images-portfolio {
  margin-top: 27px;
  margin: 0 auto;
  padding: 1px;

  .image-p {
    margin-bottom: 26px;
  }
}

@media (min-width: 320px) {
  .header {
  

    .wrap-image {
      .wrap-inside {
       
        width: 85px;
        height: 85px;
     
      }
    }

    .wrap-text {
      .name {
     
        font-size: 22px;
        line-height: 30px;
     
      }

      .title {
        font-size: 12px !important;
        line-height: 16px;
        color: #ffffff;
      }
    }

  
  }





}
@media (min-width: 360px) {
  .header {
 
    .wrap-image {
      .wrap-inside {
     
      }
    }

    .wrap-text {
      .name {
      
      }

      .title {
      
      }
    }

   
  }
 
}
@media (min-width: 767px) {
}
@media (min-width: 1024px) {
}
</style>
