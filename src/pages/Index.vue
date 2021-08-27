<template>
  <q-layout view="lHh lpr lFf">
    <div v-bind:class="{'main': $q.platform.is.desktop}"
         class="full-height" style="background-color:rgba(0, 0, 0, 0.3);">

      <q-header class="q-py-sm" style="background-color:rgba(0, 0, 0, 0.3);">
        <q-toolbar class="text-h4">
          <q-space></q-space>
          <q-tabs v-model="selected_tab" shrink>
            <q-tab name="about_me" :style="[selected_tab == 'about_me' ? {backgroundColor: '#bebebe	'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_about_me')" style="width:120px;min-height:auto !important;color: #CD0000"
                   label="About Me"/>
            <q-tab name="project" :style="[selected_tab == 'project' ? {backgroundColor: '#bebebe	'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_projects')" style="width:120px;min-height:auto !important;color: #CD0000"
                   label="project"/>
            <q-tab name="contact" :style="[selected_tab == 'contact' ? {backgroundColor: '#bebebe	'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_contact_me')"
                   style="width:120px;min-height:auto !important;color: #CD0000" label="Contact Me"/>
          </q-tabs>
        </q-toolbar>
      </q-header>
      <section>
        <div class="full-height full-width flex flex-center text-center"
           style="background-color: rgba(0, 0, 0, 0.3) !important;z-index:0;height: 100vh !important;">
        <div class="">
                  <div class="text-h2 text-white q-py-sm q-my-md"
               >JUNIOR DEVELOPER
          </div>
          <div class="text-h6" style="color: #f4b825;">
            Security (Identity & Access Management)
          </div>
          <br>
          <div style="color: #1495de !important;" class="text-h4">
            Hong Dong-Ki
          </div>
        </div>
      </div>
      </section>
    </div>

    <div style="background-color:#787878" id="id_about_me">
      <div class="row">
        <div class="col-md-4 col-lg-4 col-xs-12 col-sm-12">
          <div style="background-color: rgba(0, 0, 0, 0.68) !important;">
            <div style="background-color: rgba(0, 0, 0, 0.68) !important;">
              <q-img style="height:400px"
                     class="col-5"
                     src="/statics/images/my2.jpg"
              />
            </div>
          </div>
        </div>
        <div class="col-md-8 col-lg-8 col-xs-12 col-sm-12 q-px-md q-pt-sm">
          <div class="text-h4 text-center text-red q-py-xs q-my-xs">ABOUT ME
          </div>
          <h5 class="q-my-none text-caption" style="color: white; font-size:25px;">
            <br>
            <br>
            I worked as a stenographer and I am studying to become a developer by entering 
            <br>
            <br>
            the dept. of Smart Finance at Gangseo Polytechnic University in 2021.
            <br>
            <br>
            <br>
            <br>
            AccessDelegation, OIDC, SAML, and Identity Federation with Social Login 
            <br>
            <br>
            using WSO2 is studying
            <br>
            <br>
            <br>
            <br>            
            I will do my best to be a developer facing upwards, even if it is slow.
          </h5>
        </div>
      </div>
    </div>
    <div style="background-color:	#464646" id="id_projects">
      <div class="row q-px-xl">
        <div class="text-h4 text-center text-red q-py-sm q-my-md full-width">Project
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/HongDonkey/KopoBlockchain" target="_blank">BlockChain</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      Python Blockchain Implementation for educational purposes  
                      (Dept. of Smart Finance of Korea Polytechnics)
                      <ul>
                        <li>REST Interface impl. with Python Socket</li>
                        <li>Transaction validation</li>
                        <li>Hashing data and Mining Block</li>
                        <li>Broadcating Block to certain Nodes</li>
                        <li>Compare and Merge Blocks</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      href="google.com"
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/blockchain.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>


          </q-card>
        </div>


        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/HongDonkey/BoardProject" target="_blank">Board with social login</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      <ul>
                        <li>Basic board with CRUD</li>
                        <li>Kakao, Naver, Facebook social login function establishment</li>
                        <li>Apply MyBatis method</li>
                        <li>Windows10, CentOS8, eGovFramework 3.9.0</li>
                        <li>jdk 1.8, MariaDB 10.1.37, Tomcat 9</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/board.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>


          </q-card>

        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/HongDonkey/stockModel" target="_blank">Stock Model</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      Forecasting stock price based on various finance statistics.
                      Lots of code is produced by students while using some external python libraries like FinanceReader, Selenium.
                      <ul>
                        <li>matplotlib, pandas, numpy, scipy</li>
                        <li>finance-datareader</li>
                        <li>beautifulsoup4</li>
                        <li>mplfinance</li>
                        <li>chart-studio</li>
                        <li>plotly</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/stock.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            
          </q-card>
        </div>
      </div>
    </div>



    <div id="contact_us">
      <div style="background-color: rgba(0, 0, 0, 0.68) !important;">

      </div>
    </div>
    <q-toolbar class="flex flex-center text-white" style="background-color: #1c1b21;border-top: 2px solid red"
               id="id_contact_me">
      <div class="q-pa-sm q-gutter-sm">
        <q-btn target="_blank" style="border: 2px solid red" round type="a" href="https://www.instagram.com/donkey_92/"
               glossy
               icon="fab fa-instagram"/>
        <q-btn target="_blank" style="border: 2px solid red" round type="a"
               href="https://github.com/HongDonkey"
               glossy
               icon="fab fa-github"/>
        <q-btn style="border: 2px solid red" round type="a" href="mailto:dkhong@pharosinfo.com"
               glossy
               icon="email"/>
        <q-btn target="_blank" style="border: 2px solid red;" round type="a"
               href="https://www.facebook.com/profile.php?id=100002104861584"
               glossy
               icon="fab fa-facebook"/>
      </div>
    </q-toolbar>
  </q-layout>
</template>

<script>

    import {scroll} from 'quasar'

    const {getScrollTarget, setScrollPosition} = scroll
    export default {
        name: 'PageIndex',
        data() {
            return {
                name: "",
                email: "",
                message: "",
                selected_tab: 'about_me',
            }
        },
        methods: {
            scrollToElement(id) {
                let el = document.getElementById(id)
                const target = getScrollTarget(el)
                const offset = el.offsetTop - 65
                const duration = 800
                setScrollPosition(target, offset, duration)
            }
        },
    }
</script>

<style>
  .main {

    background: url(/statics/images/my1.jpg) no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    height: 100vh !important;
  }

  .my-card {
    width: 100%;
    max-width: 800px;
    border: none;
    border-radius: 0px;
  }

  .sponsor-card {
    width: 100%;
    max-width: 240px;
    border: none;
    border-radius: 6px;
  }

  .project_link:hover {
    text-decoration: underline !important;
  }

  .sketch_desktop {
    width: 100%;
    height: 100%;
    display:block; 
    margin:auto;
    border: 5px solid #30313b;
  }

  .sketch_mobile {
    width: 100%;
    height: 100% !important;
    border: 20px solid #30313b;
  }

  #contact_us {
    background: url(/statics/images/contact_us.jpg);
    background-size: cover;
    background-position: 50%;
    background-attachment: fixed;
    background-repeat: no-repeat;
  }

  .custom_tab {
    width: 130px;
  }

  body {
    overflow-x: hidden;
  }

  section {
    position: relative;
  }

  section > * {
    z-index: 9;
    position: relative;
    top: 0;
  }

  section > canvas {
    z-index: 1;
    position: absolute;
    left: 0;
  }
</style>
