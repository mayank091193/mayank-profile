<template>
  <q-layout view="lHh lpr lFf">
    <div v-bind:class="{'main': $q.platform.is.desktop, 'mobile_main': $q.platform.is.ipad || $q.platform.is.mobile}"
         class="full-height" style="background-color:rgba(0, 0, 0, 0.7);">

      <q-header class="q-py-sm" style="background-color:rgba(0, 0, 0, 0.7);">
        <q-toolbar class="text-h4">
          <q-space></q-space>
          <q-tabs v-model="selected_tab" shrink>
            <q-tab :style="[selected_tab == 't_0' ? {backgroundColor: 'blue'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_about_me')" style="width:120px;min-height:auto !important;color: white"
                   label="About Me"/>
            <q-tab :style="[selected_tab == 't_1' ? {backgroundColor: 'blue'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_projects')" style="width:120px;min-height:auto !important;color: white"
                   label="Projects"/>
            <q-tab :style="[selected_tab == 't_2' ? {backgroundColor: 'blue'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_sponsors')" style="width:120px;min-height:auto !important;color: white"
                   label="Sponsors"/>
            <q-tab :style="[selected_tab == 't_3' ? {backgroundColor: 'blue'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_sketches')" style="width:120px;min-height:auto !important;color: white"
                   label="Sketches"/>
            <q-tab :style="[selected_tab == 't_4' ? {backgroundColor: 'blue'} : {}]" class="q-mr-sm q-py-xs custom_tab"
                   @click="scrollToElement('id_contact_me')"
                   style="width:120px;min-height:auto !important;color: white" label="Contact Me"/>
          </q-tabs>
        </q-toolbar>
      </q-header>
      <section>
        <div class="full-height full-width flex flex-center text-center"
           style="background-color: rgba(0, 0, 0, 0.68) !important;z-index:0;height: 100vh !important;">
        <div class="">
          <div class="text-h6 text-grey-5">WELCOME TO MY PAGE</div>
          <div class="text-h2 text-white q-py-sm q-my-md"
               style="border-top:3px solid #1595de;border-bottom: 3px solid #2faa64;">I'M FULL-STACK DEVELOPER
          </div>
          <div class="text-h6" style="color: #f4b825;">
            WEB DEVELOPMENT | WEB DESIGN | SERVER MANAGEMENT
          </div>
          <div style="color: #1495de !important;" class="text-h4 q-mt-md text-grey-2 my-font">
            Mayank Patel
          </div>
        </div>
      </div>
        <canvas id="canvas1" style="height: 100%;width:100%;"></canvas>
      </section>
    </div>

    <div style="background-color:#33495e" id="id_about_me">
      <div class="row">
        <div class="col-md-4 col-lg-4 col-xs-12 col-sm-12">
          <div style="background-color:#ea4946" class="q-pa-md text-center text-white text-weight-bolder text-h4">
            ABOUT ME
          </div>
          <div style="background-color: rgba(0, 0, 0, 0.68) !important;">
            <div style="background-color: rgba(0, 0, 0, 0.68) !important;">
              <q-img style="height:300px"
                     class="col-5"
                     src="/statics/images/my_2.png"
              />
            </div>
          </div>
        </div>
        <div class="col-md-8 col-lg-8 col-xs-12 col-sm-12 q-px-md q-pt-sm">
          <div class="text-h4 text-center text-white q-py-xs q-my-xs"
               style="border-top:3px solid #bdbdbd;border-bottom: 3px solid #bdbdbd;">HELLO
          </div>
          <h5 class="q-my-none text-caption" style="color: #20ffff;">
            I am Mayank Patel (Known as mayank091193). I am in the programming field since 2011. I always wanted to
            become a skilled programmer. My passion to become a full-stack developer increased when I started working at
            my first job in Vadodara, Gujarat.
            <br>
            <br>
            I started my career with HTML/CSS as the front-end and ASP.NET C#. In the initial stage, I was working on 3
            tier architecture that our company had built. Later we had implemented ASP.NET MVC Architecture. Later after
            2 years, I have decided to move to another company to get myself challenges and learn more. In my second
            company, I started working on HTML/Bootstrap/AngularJS as the front-end and Python as the back-end language.
            <br>
            <br>
            In this phase, I have learned many technologies. I got many projects to work on. The major project includes
            the Sales reporting system, CRM system, AWS based data warehouse solution and many more. Eventually, I
            introduced myself to Quasar-Framework and Vue.js. After getting hands-on experience on Quasar-Framework for
            2 years, I got involved in creating some plugins for Quasar Framework such as QDraggableHierarchy App
            Extension.
            <br>
            <br>
            Also, I do believe in Free or Open Source Software (FOSS) because I believe "Knowledge management doesn’t
            happen until somebody reuses something". I believe for sustaining in the market, you need to keep yourself
            updated with knowledge. Solution matters technology doesn't.

          </h5>
        </div>
      </div>
    </div>
    <div style="background-color:#2b5873" id="id_projects">
      <div class="row q-px-xl">
        <div class="text-h4 text-center text-white q-py-sm q-my-md full-width"
             style="border-top:3px solid #bdbdbd;border-bottom: 3px solid #bdbdbd;">MY OPEN SOURCE PROJECTS
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <q-ribbon class="github-text" position="top-right" type="corner" color="white" background-color="#eb4f71">
                <a href="https://github.com/mayank091193/quasar-admin-crm" target="_blank">FORK ME ON GITHUB!</a>
              </q-ribbon>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-overline text-pink">Made With Love</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/mayank091193/quasar-admin-crm" target="_blank">Quasar Admin CRM</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      A free and beautiful Quasar template for CRM needs. It is a fully responsive template built using
                      the Quasar framework that makes it available for all screen sizes from big screens to smartphones.
                      <ul>
                        <li>Modern and responsive design</li>
                        <li>Building design based on CRM</li>
                        <li>Simple CRM Dashboard</li>
                        <li>Activity tracking on Calendar</li>
                        <li>Export feature</li>
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
                      src="/statics/images/admin_crm.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            <q-card-actions class="block">
              <a style="font-size: 25px;" class="q-py-sm q-pl-sm" href="https://github.com/sponsors/mayank091193"
                 target="_blank" title="Donate"><i class="fas fa-heart" style="color: #eb5daa"></i></a>
              <div class="float-right q-py-sm">
                <iframe class="float-right"
                        src="https://ghbtns.com/github-btn.html?user=mayank091193&repo=quasar-admin-crm&type=star&count=true&size=large"
                        frameborder="0" scrolling="0" width="136" height="30" title="GitHub"></iframe>
              </div>
            </q-card-actions>
          </q-card>
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <q-ribbon class="github-text" position="top-right" type="corner" color="white" background-color="#eb4f71">
                <a href="https://github.com/mayank091193/quasar-scrum" target="_blank">FORK ME ON GITHUB!</a>
              </q-ribbon>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-overline text-pink">Made With Love</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/mayank091193/quasar-scrum" target="_blank">Quasar
                        Scrum</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      Quasar Scrum - Free Project Management Template - Agile process framework for managing complex
                      tasks.
                      <ul>
                        <li>Dashboard</li>
                        <li>Taskboard Grid View</li>
                        <li>Taskboard List View</li>
                        <li>Drag and drop tasks</li>
                        <li>Homepage with basic details, pricing</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/quasar_scrum.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            <q-card-actions class="block">
              <a style="font-size: 25px;" class="q-py-sm q-pl-sm" href="https://github.com/sponsors/mayank091193"
                 target="_blank" title="Donate"><i class="fas fa-heart" style="color: #eb5daa"></i></a>
              <div class="float-right q-py-sm">
                <iframe class="float-right"
                        src="https://ghbtns.com/github-btn.html?user=mayank091193&repo=quasar-scrum&type=star&count=true&size=large"
                        frameborder="0" scrolling="0" width="136" height="30" title="GitHub"></iframe>
              </div>
            </q-card-actions>
          </q-card>
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <q-ribbon class="github-text" position="top-right" type="corner" color="white" background-color="#eb4f71">
                <a href="https://github.com/mayank091193/vue-quasar-company-profile-website" target="_blank">FORK ME ON
                  GITHUB!</a>
              </q-ribbon>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-overline text-pink">Made With Love</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/mayank091193/vue-quasar-company-profile-website" target="_blank">Company
                        Profile Template</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      Free template for company profile made using Quasar Framework and Vue.js! It is a fully responsive
                      template which you can use for your company or may be for your own portfolio website.
                      <ul>
                        <li>Homepage</li>
                        <li>Portfolio</li>
                        <li>About Us</li>
                        <li>Services</li>
                        <li>Testimonial</li>
                        <li>Pricing</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/company_profile.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            <q-card-actions class="block">
              <a style="font-size: 25px;" class="q-py-sm q-pl-sm" href="https://github.com/sponsors/mayank091193"
                 target="_blank" title="Donate"><i class="fas fa-heart" style="color: #eb5daa"></i></a>
              <div class="float-right q-py-sm">
                <iframe class="float-right"
                        src="https://ghbtns.com/github-btn.html?user=mayank091193&repo=vue-quasar-company-profile-website&type=star&count=true&size=large"
                        frameborder="0" scrolling="0" width="136" height="30" title="GitHub"></iframe>
              </div>
            </q-card-actions>
          </q-card>
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <q-ribbon class="github-text" position="top-right" type="corner" color="white" background-color="#eb4f71">
                <a href="https://github.com/mayank091193/quasar-draggable-tree" target="_blank">FORK ME ON GITHUB!</a>
              </q-ribbon>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-overline text-pink">Made With Love</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/mayank091193/quasar-draggable-tree" target="_blank">Quasar Draggable
                        Tree</a>
                    </div>
                    <div class="text-caption text-grey-9">
                      QDraggableTree is a Quasar App Extension. It is a component that displays hierarchical data with
                      drag and drop ability.
                      <ul>
                        <li>Ability to drag-drop nodes in QTree</li>
                        <li>Slot Support</li>
                        <li>Usage documentation and Demo</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-5 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/quasar_draggable_tree.png"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            <q-card-actions class="block">
              <a style="font-size: 25px;" class="q-py-sm q-pl-sm" href="https://github.com/sponsors/mayank091193"
                 target="_blank" title="Donate"><i class="fas fa-heart" style="color: #eb5daa"></i></a>
              <div class="float-right q-py-sm">
                <iframe class="float-right"
                        src="https://ghbtns.com/github-btn.html?user=mayank091193&repo=quasar-draggable-tree&type=star&count=true&size=large"
                        frameborder="0" scrolling="0" width="136" height="30" title="GitHub"></iframe>
              </div>
            </q-card-actions>
          </q-card>
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-card class="my-card" flat bordered>
            <q-card-section>
              <q-ribbon class="github-text" position="top-right" type="corner" color="white" background-color="#eb4f71">
                <a href="https://github.com/mayank091193/CoolTab" target="_blank">FORK ME ON GITHUB!</a>
              </q-ribbon>
              <div class="row">
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="q-py-xs">
                    <div class="text-overline text-pink">Made With Love</div>
                    <div class="text-h5 q-mt-sm q-mb-xs">
                      <a class="project_link" style="text-decoration: none;color: #eb4f71;"
                         href="https://github.com/mayank091193/CoolTab" target="_blank">CoolTab</a></div>
                    <div class="text-caption text-grey-9">
                      Free chrome extension - CoolTab | Free chrome extension starter. It replaces new tab page with a
                      personal dashboard featuring notes, thoughts, time,etc.
                      <ul>
                        <li>Free Chrome Extension</li>
                        <li>Built using Bootstrap</li>
                        <li>Special New Tab</li>
                      </ul>
                    </div>
                  </q-card-section>
                </div>
                <div class="col-lg-6 col-md-6 col-xs-12 col-sm-12">
                  <q-card-section class="col-md-6 flex flex-center">
                    <q-img
                      class="rounded-borders"
                      style="border:1px solid darkgrey"
                      src="/statics/images/cooltab.jpg"
                    />
                  </q-card-section>
                </div>
              </div>
            </q-card-section>

            <q-separator/>

            <q-card-actions class="block">
              <a style="font-size: 25px;" class="q-py-sm q-pl-sm" href="https://github.com/sponsors/mayank091193"
                 target="_blank" title="Donate"><i class="fas fa-heart" style="color: #eb5daa"></i></a>
              <div class="float-right q-py-sm">
                <iframe class="float-right"
                        src="https://ghbtns.com/github-btn.html?user=mayank091193&repo=CoolTab&type=star&count=true&size=large"
                        frameborder="0" scrolling="0" width="136" height="30" title="GitHub"></iframe>
              </div>
            </q-card-actions>
          </q-card>
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <iframe src="https://github.com/sponsors/mayank091193/card" title="Sponsor Mayank" height="171" width="700"
                  style="border: 0;"></iframe>
        </div>
      </div>
    </div>
    <div style="background-color:#14104e" id="id_sponsors">
      <div class="row row q-px-xl">
        <div class="text-h4 text-center text-white q-py-sm q-my-md full-width"
             style="border-top:3px solid #bdbdbd;border-bottom: 3px solid #bdbdbd;">Bronze Sponsor(S)
        </div>
        <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl flex flex-center">
          <q-btn target="_blank" type="a" href="https://github.com/ex-kimura">
            <q-card class="sponsor-card q-my-sm">
              <q-card-section class="q-pb-none">
                <div class="text-h6 text-center text-grey-9">ex-kimura</div>
              </q-card-section>
              <q-card-section class="flex flex-center">
                <img class="" style="height: 185px;width: 185px;"
                     src="https://avatars.githubusercontent.com/ex-kimura">
              </q-card-section>
            </q-card>
          </q-btn>
        </div>
      </div>
    </div>
    <section>
      <div style="background-color:#206b73;z-index:0;" class="content" id="id_sketches">
        <div class="row row q-px-xl">
          <div class="text-h4 text-center text-white q-py-sm q-my-md full-width"
               style="border-top:3px solid #bdbdbd;border-bottom: 3px solid #bdbdbd;">My Sketches
          </div>
          <div class="col-md-12 col-md-12 col-xs-12 col-sm-12 q-mb-xl">
            <div class="q-pa-md">
              <div class="q-col-gutter-md row">
                <div class="col-md-6 col-md-6 col-xs-12 col-sm-12 text-center flex flex-center">
                  <q-img
                    src="statics/images/sketch_1.jpg"
                    v-bind:class="{'sketch_desktop': $q.platform.is.desktop, 'sketch_mobile': $q.platform.is.ipad || $q.platform.is.mobile}"
                  >
                  </q-img>
                </div>

                <div class="col-md-6 col-md-6 col-xs-12 col-sm-12 text-center flex flex-center">
                  <q-img src="statics/images/sketch_2.jpg"
                         v-bind:class="{'sketch_desktop': $q.platform.is.desktop, 'sketch_mobile': $q.platform.is.ipad || $q.platform.is.mobile}">
                  </q-img>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <canvas id="canvas2" style="height: 100%;width:100%;"></canvas>
    </section>
    <div id="contact_us">
      <div style="background-color: rgba(0, 0, 0, 0.68) !important;">
        <form
          action="https://formspree.io/mpzydoze"
          method="POST"
        >
          <div class="row text-center flex flex-center q-py-lg">
            <div class="col-md-6 col-lg-6 col-sx-12 col-sm-12 q-gutter-lg q-px-xl q-pb-none q-ma-none">
              <q-input required v-model="name" name="name" bg-color="white" outlined label="Your Name *">
                <template v-slot:append>
                  <q-icon name="list" style="color:blue"/>
                </template>
              </q-input>
              <q-input required v-model="email" bg-color="white" outlined label="Your Email *">
                <template v-slot:append>
                  <q-icon name="email" style="color:blue"/>
                </template>
              </q-input>
            </div>
            <div class="col-md-6 col-lg-6 col-sx-12 col-sm-12 q-gutter-lg q-px-xl q-pb-none q-ma-none">
              <q-input required v-model="message" name="message" class="" type="textarea" bg-color="white" outlined
                       label="Your Message *">
                <template v-slot:append>
                  <q-icon name="comment" style="color:blue"/>
                </template>
              </q-input>
            </div>
          </div>
          <div class="row flex flex-center text-center q-pb-xl q-mt-md">
            <div class="col-md-12 col-lg-12 col-sx-12 col-sm-12">
              <q-btn type="submit" size="lg" style="background:blue;color: white" label="Send Message"/>
            </div>
          </div>
        </form>
      </div>
    </div>
    <q-toolbar class="flex flex-center text-white" style="background-color: #1c1b21;border-top: 2px solid blue"
               id="id_contact_me">
      <div class="q-pa-sm q-gutter-sm">
        <q-btn target="_blank" style="border: 2px solid blue" round type="a" href="https://twitter.com/mayank91193"
               glossy
               icon="fab fa-twitter"/>
        <q-btn target="_blank" style="border: 2px solid blue" round type="a"
               href="https://github.com/mayank091193"
               glossy
               icon="fab fa-github"/>
        <q-btn style="border: 2px solid blue" round type="a" href="mailto:mayank091193@gmail.com"
               glossy
               icon="email"/>
        <q-btn target="_blank" style="border: 2px solid blue;" round type="a"
               href="https://github.com/sponsors/mayank091193"
               glossy
               icon="fas fa-heart"/>
        <q-btn target="_blank" style="border: 2px solid blue;" round type="a"
               href="https://stackoverflow.com/users/4763038/mayank-patel"
               glossy
               icon="fab fa-stack-overflow"/>
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
                selected_tab: 't_0',
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
        mounted: function () {
            let canvas1Settings = {
                "target": "canvas1",
                "max": "99",
                "animate": true,
                "props": ["circle", "square", "triangle", "line"],
                "colors": [[165, 104, 246], [230, 61, 135], [0, 199, 228], [253, 214, 126]],
                "clock": "9"
            };
            let canvas1 = new ConfettiGenerator(canvas1Settings);
            canvas1.render();
            let canvas2Settings = {
                "target": "canvas2",
                "max": "120",
                "animate": true,
                "props": ["circle", "square", "triangle", "line"],
                "colors": [[165, 104, 246], [230, 61, 135], [0, 199, 228], [253, 214, 126]],
                "clock": "20"
            };
            let canvas2 = new ConfettiGenerator(canvas2Settings);
            canvas2.render();
        }
    }
</script>

<style>
  .main {

    background: url(/statics/images/my_1.jpg) no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    height: 100vh !important;
  }

  .mobile_main {
    background: url(/statics/images/my_1_2.jpg) no-repeat center center fixed;
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
    width: 450px;
    height: 620px;
    border: 20px solid #30313b;
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
