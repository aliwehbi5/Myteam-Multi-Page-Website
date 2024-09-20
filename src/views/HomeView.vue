<script setup>
import footerComponent from '@/components/footerComponent.vue'
import readyComponent from '@/components/readyComponent.vue'
</script>

<template>
  <main>
    <div class="landing-page">
      <div class="container">
        <div class="row">
          <div class="title">
            <h1>Find the best <b>talent</b></h1>
          </div>
          <div class="detials">
            <span></span>
            <p>
              Finding the right people and building high performing teams can be hard. Most
              companies aren’t tapping into the abundance of global talent. We’re about to change
              that.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="team-div">
      <div class="container">
        <div class="row">
          <div class="title">
            <span></span>
            <h1>Build & manage distributed teams like no one else.</h1>
          </div>
          <div class="team">
            <div class="team-member">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/393512.svg"
                alt=""
              />
              <div class="content">
                <h4>Experienced Individuals</h4>
                <p>
                  Our network is made up of highly experienced professionals who are passionate
                  about what they do.
                </p>
              </div>
            </div>
            <div class="team-member">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/015c88.svg"
                alt=""
              />
              <div class="content">
                <h4>Easy to Implement</h4>
                <p>
                  Our processes have been refined over years of implementation meaning our teams
                  always deliver.
                </p>
              </div>
            </div>
            <div class="team-member">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/3671c4.svg"
                alt=""
              />
              <div class="content">
                <h4>Enhanced Productivity</h4>
                <p>
                  Our customized platform with in-built analytics helps you manage your distributed
                  teams.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="stories-div">
      <div class="container">
        <div class="title">
          <h1>Delivering real results for top companies. Some of our <b>success stories.</b></h1>
        </div>
        <div class="stories">
          <div class="story">
            <q>
              The team perfectly fit the specialized skill set required. They focused on the most
              essential features helping us launch the platform eight months faster than planned.
            </q>
            <div class="detials">
              <h4 class="name">Kady Baker</h4>
              <p><i>Product Manager at Bookmark</i></p>
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/306942.jpg"
                alt=""
                class="person-img"
              />
            </div>
          </div>
          <div class="story">
            <q>
              We needed to automate our entire onboarding process. The team came in and built out
              the whole journey. Since going live, user retention has gone through the roof!
            </q>
            <div class="detials">
              <h4 class="name">Aiysha Reese</h4>
              <p><i>Founder of Manage </i></p>
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/d23913.jpg"
                alt=""
                class="person-img"
              />
            </div>
          </div>
          <div class="story">
            <q>
              Amazing. Our team helped us build an app that delivered a new experience for hiring a
              physio. The launch was an instant success with 100k downloads in the first month.
            </q>
            <div class="detials">
              <h4 class="name">Arthur Clarke</h4>
              <p><i>Co-founder of MyPhysio </i></p>
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/db2316.jpg"
                alt=""
                class="person-img"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <readyComponent></readyComponent>
    <footerComponent></footerComponent>
  </main>
</template>

<style scoped>
.landing-page {
  height: calc(100vh - 205px);
  background-color: var(--dark-cyan);
  position: relative;
}
.landing-page .row {
  display: flex;
  position: relative;
  color: white;
  gap: 40px;
  align-items: stretch;
}
.landing-page .container {
  position: relative;
  height: 100%;
}
.landing-page .container::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-2.svg);
  position: absolute;
  bottom: -6px;
  right: 0;
  z-index: 0;
}
.landing-page .title {
  width: 100%;
}
.landing-page .title h1 {
  font-size: 6.5rem;
  line-height: 6.5rem;
  font-weight: bold;
}
.landing-page .title b {
  font-weight: bold;
  color: var(--salmon);
}
.landing-page .detials {
  position: relative;
  display: flex;
  align-items: flex-end;
}
.landing-page .detials p {
  font-size: 18px;
  font-weight: 500;
}
@media (min-width: 769px) {
  .landing-page::before {
    content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-1.svg);
    position: absolute;
    top: 0;
    transform: translateX(-50%);
    z-index: 0;
  }
  .landing-page .detials {
    width: 75%;
  }
  .landing-page .detials span {
    width: 50px;
    height: 4px;
    background-color: #79c8c7;
    position: absolute;
    top: 0;
    left: 0;
  }
}
@media (max-width: 991px) {
  .landing-page .title h1 {
    font-size: 5rem;
    line-height: 5rem;
  }
  .landing-page .detials p {
    font-size: 16px;
  }
}
@media (max-width: 768px) {
  .landing-page {
    height: calc(100vh - 126px);
  }
  .landing-page .row {
    max-width: 450px;
    margin: auto;
    flex-direction: column;
    text-align: center;
  }
  .landing-page .title h1 {
    font-size: 3.5rem;
    line-height: 3.5rem;
  }
  .landing-page .container::before {
    right: auto;
    left: 50%;
    transform: translateX(-50%);
  }
}
.team-div {
  background-color: var(--midnight-blue);
  padding: 100px 0;
  position: relative;
  overflow: hidden;
}
.team-div::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-3.svg);
  position: absolute;
  bottom: 0;
  left: 100%;
  transform: translateX(-50%);
  z-index: 0;
}
.team-div .row {
  display: flex;
  gap: 40px;
  color: white;
  position: relative;
}
.team-div .title span {
  width: 50px;
  height: 4px;
  background-color: var(--salmon);
  display: block;
}
.team-div .title h1 {
  font-size: 3.5rem;
  line-height: 3.5rem;
  font-weight: bold;
  margin-top: 50px;
}
.team-div .row > div {
  width: 100%;
}
.team-div .team-member {
  display: flex;
  gap: 20px;
  margin-bottom: 40px;
  align-items: center;
}
.team-div .content h4 {
  color: var(--salmon);
  font-weight: bold;
  font-size: 18px;
}
.team-div .content p {
  margin-top: 15px;
  font-weight: 600;
  color: #ccd5d6;
}
.stories-div {
  background-color: #004047;
  padding: 100px 0;
  color: white;
  position: relative;
}
.stories-div::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-4-about-3.svg);
  position: absolute;
  top: 0;
  left: 0;
}
.stories-div::after {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-5.svg);
  position: absolute;
  bottom: -6px;
  right: 0;
}
.stories-div .title {
  margin-bottom: 50px;
}
.stories-div .title h1 {
  font-size: 3.5rem;
  line-height: 3.5rem;
  text-align: center;
  font-weight: bold;
}
.stories-div .title h1 b {
  font-weight: bold;
  color: var(--aquamarine);
}
.stories {
  display: flex;
  gap: 30px;
}
.story {
  width: 100%;
  text-align: center;
  padding-top: 30px;
  position: relative;
  z-index: 10;
}
.story::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/icon-quotes.svg);
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  z-index: -1;
}
.stories-div .story q {
  font-weight: 500;
}
.stories .detials {
  margin-top: 30px;
}
.stories h4.name {
  color: var(--aquamarine);
  font-weight: bold;
}
.stories img.person-img {
  margin-top: 15px;
  border: 2px solid white;
  border-radius: 50%;
}
@media (max-width: 991px) {
  .team-div::before {
    bottom: auto;
    top: 0;
  }
  .team-div .row {
    flex-direction: column;
  }
  .team-div .title h1 {
    font-size: 2.5rem;
    line-height: 2.5rem;
    max-width: 80%;
  }
  .stories-div .title h1 {
    font-size: 2.5rem;
    line-height: 2.5rem;
  }
  .stories {
    flex-direction: column;
  }
}
@media (max-width: 767px) {
  .team-div .team-member {
    text-align: center;
    flex-direction: column;
  }
  .stories-div .title h1 {
    font-size: 2rem;
    line-height: 2rem;
  }
}
</style>
