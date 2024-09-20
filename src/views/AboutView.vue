<script setup>
import footerComponent from '@/components/footerComponent.vue'
import readyComponent from '@/components/readyComponent.vue'
</script>
<template>
  <section class="about-section">
    <div class="section-intro">
      <div class="container">
        <div class="row">
          <div class="title">
            <h1>About</h1>
          </div>
          <div class="desc">
            <span></span>
            <p>
              We help companies build dynamic teams made up of top global talent. Using our network
              of passionate professionals we drive innovation and deliver incredible outcomes.
              Talented, diverse teams shape the best products and experiences. We’ll bring those
              teams to you.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="directors">
      <div class="container">
        <h1>Meet the directors</h1>
        <div class="row">
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/339265.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Nikita Marks</h3>
              <p class="director-job"><i>Founder & CEO</i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Nikita Marks</h3>
              <q>It always amazes me how much talent there is in every corner of the globe.</q>
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/eb2a3f.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Cristian Duncan</h3>
              <p class="director-job"><i>Co-founder & COO</i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Cristian Duncan</h3>
              <q
                >Distributed teams required unique processes. You need to approach work in a new
                way.</q
              >
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/f608c9.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Cruz Hamer</h3>
              <p class="director-job"><i>Co-founder & CTO </i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Cruz Hamer</h3>
              <q
                >Technology is at the forefront of enabling distributed teams. That's where we come
                in.</q
              >
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/9c6c6b.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Drake Heaton</h3>
              <p class="director-job"><i>Business Development Lead </i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Drake Heaton</h3>
              <q
                >Hiring similar people from similar backgrounds is a surefire way to stunt
                innovation.</q
              >
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/2a1d53.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Griffin Wise</h3>
              <p class="director-job"><i>Lead Marketing</i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Griffin Wise</h3>
              <q
                >Unique perspectives shape unique products, which is what you need to survive these
                days.</q
              >
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
          <div class="director">
            <div class="front-side">
              <img
                src="https://myteam-multi-page-website-teal.vercel.app/_nuxt/image/f0fded.jpg"
                class="director-img"
                alt=""
              />
              <h3 class="director-name">Aden Allan</h3>
              <p class="director-job"><i>Head of Talent</i></p>
              <span class="flip-btn" @click="toggleFlip($event)"
                ><i class="fa-solid fa-plus"></i
              ></span>
            </div>
            <div class="back-side">
              <h3 class="director-name">Aden Allan</h3>
              <q
                >Empowered teams create truly amazing products. Set the north star and let them
                follow it.</q
              >
              <ul class="socials">
                <li>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fa-brands fa-instagram"></i></a>
                </li>
              </ul>
              <span class="flip-btn" @click="toggleFlip($event)">
                <i class="fas fa-times icon close"></i>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="clients-div">
      <div class="container">
        <h1>Some of our clients</h1>
        <ul class="clients">
          <li>
            <img
              src="https://myteam-multi-page-website-teal.vercel.app/images/logo-the-verge.png"
              alt=""
            />
          </li>
          <li>
            <img
              src="https://myteam-multi-page-website-teal.vercel.app/images/logo-jakarta-post.png"
              alt=""
            />
          </li>
          <li>
            <img
              src="https://myteam-multi-page-website-teal.vercel.app/images/logo-the-guardian.png"
              alt=""
            />
          </li>
          <li>
            <img
              src="https://myteam-multi-page-website-teal.vercel.app/images/logo-tech-radar.png"
              alt=""
            />
          </li>
          <li>
            <img
              src="https://myteam-multi-page-website-teal.vercel.app/images/logo-gadgets-now.png"
              alt=""
            />
          </li>
        </ul>
      </div>
    </div>
    <readyComponent></readyComponent>
    <footerComponent></footerComponent>
  </section>
</template>

<script>
export default {
  name: 'aboutView',

  methods: {
    toggleFlip(event) {
      const directorDiv = event.target.closest('.director')
      directorDiv.classList.toggle('flip')
      console.log(directorDiv)
    }
  }
}
</script>

<style scoped>
.section-intro {
  background-color: var(--dark-cyan);
  padding: 50px 0;
  color: white;
  position: relative;
  z-index: 10;
  overflow: hidden;
}
.section-intro::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-about-1-mobile-nav-1.svg);
  position: absolute;
  bottom: 0;
  right: 0;
  transform: translateX(50%);
  z-index: -1;
}
.section-intro .row {
  display: flex;
  gap: 100px;
}
.section-intro h1 {
  font-size: 4rem;
}
.section-intro p {
  font-weight: 500;
  font-size: 1rem;
}
@media (min-width: 769px) {
  .section-intro span {
    width: 50px;
    height: 4px;
    background-color: var(--salmon);
    display: block;
    margin-bottom: 40px;
  }
}
.directors {
  padding: 100px 0;
  background-color: #004047;
  position: relative;
  z-index: 10;
  overflow: hidden;
}
.directors::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-about-2-contact-1.svg);
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transform: translateX(-50%);
}
.directors::after {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-4-about-3.svg);
  position: absolute;
  bottom: -6px;
  right: 0;
  z-index: -1;
}
.directors .row {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  column-gap: 40px;
  row-gap: 60px;
  padding-top: 30px;
}
.directors h1 {
  color: white;
  font-size: 3rem;
  text-align: center;
}
.directors .director {
  background-color: var(--midnight-blue);
  position: relative;
  transform-style: preserve-3d;
  transition: 1s;
}
.directors .director .front-side {
  position: relative;
  z-index: 1;
  text-align: center;
  padding: 30px;
  backface-visibility: hidden;
}
.directors .director .back-side {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #002529;
  color: #fff;
  padding: 30px;
  transform: rotateY(180deg);
  backface-visibility: hidden;
  text-align: center;
}
.directors .director.flip {
  transform: rotateY(180deg);
}
.directors img.director-img {
  width: 96px;
  border-radius: 50%;
  border: 2px solid white;
  margin-bottom: 10px;
}
.directors h3.director-name {
  color: var(--aquamarine);
}
.directors p.director-job {
  color: white;
  margin: 5px 0 10px;
}
.director span.flip-btn {
  position: absolute;
  width: 60px;
  height: 60px;
  background-color: var(--salmon);
  border-radius: 50%;
  left: 50%;
  transform: translateX(-50%);
  cursor: pointer;
  text-align: center;
  line-height: 60px;
  font-size: 23px;
  color: var(--midnight-blue);
  transition: 0.3s;
}
.director .back-side span.flip-btn {
  bottom: -30px;
  background-color: var(--aquamarine);
}
.director .back-side span.flip-btn:hover {
  background-color: var(--salmon);
}
.director .front-side span.flip-btn:hover {
  background-color: var(--aquamarine);
}
.director .back-side q {
  margin: 15px 0;
  font-size: 16px;
  font-weight: 500;
  display: block;
}
.director .back-side .socials {
  display: flex;
  gap: 15px;
  align-items: center;
  justify-content: center;
}
.director .back-side .socials a {
  color: white;
  font-size: 20px;
  transition: 0.3s;
}
.director .back-side .socials a:hover {
  color: var(--salmon);
}
.clients-div {
  background-color: var(--midnight-blue);
  padding: 100px 0;
  position: relative;
  z-index: 10;
}
.clients-div:before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-about-4.svg);
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}
.clients-div h1 {
  color: white;
  font-size: 3rem;
  text-align: center;
}
.clients-div .clients {
  margin-top: 40px;
  display: flex;
  gap: 50px;
  align-items: center;
}
.clients-div .clients img {
  width: 100%;
}
@media (max-width: 768px) {
  .section-intro::before {
    transform: translate(50%, 50%);
  }
  .section-intro {
    text-align: center;
  }
  .section-intro .row {
    flex-direction: column;
    gap: 20px;
  }
  .section-intro .title h1 {
    font-size: 3rem;
  }
  .directors::before {
    transform: translate(-50%, -50%);
  }
  .directors h1,
  .clients-div h1 {
    font-size: 2rem;
    line-height: 2rem;
  }
  .clients-div .clients {
    flex-direction: column;
  }
  .clients-div .clients img {
    max-width: 150px;
  }
}
</style>
