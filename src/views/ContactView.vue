<script setup>
import footerComponent from '@/components/footerComponent.vue'
</script>

<template>
  <div class="contact-section">
    <section class="content">
      <div class="container">
        <div class="row">
          <div class="info">
            <h1>Contact</h1>
            <h3>Ask us about</h3>
            <ul class="detials">
              <li>
                <img
                  src="https://myteam-multi-page-website-teal.vercel.app/images/icon-person.svg"
                  alt=""
                />The quality of our talent network
              </li>
              <li>
                <img
                  src="https://myteam-multi-page-website-teal.vercel.app/images/icon-cog.svg"
                  alt=""
                />Usage & implementation of our software
              </li>
              <li>
                <img
                  src="https://myteam-multi-page-website-teal.vercel.app/images/icon-chart.svg"
                  alt=""
                />How we help drive innovation
              </li>
            </ul>
          </div>
          <form method="post">
            <input type="text" placeholder="Name" />
            <input type="email" placeholder="Email Address" />
            <input type="text" placeholder="Company Name" />
            <input type="text" placeholder="Title" />
            <textarea placeholder="Message"></textarea>
            <button class="submit-btn" @click="handleClick">submit</button>
          </form>
        </div>
      </div>
    </section>
    <footerComponent></footerComponent>
  </div>
</template>

<script>
export default {
  name: 'contactView',
  methods: {
    handleClick(event) {
      const inputs = document.querySelectorAll('form input, form textarea')
      inputs.forEach((input) => {
        if (input.value == '') {
          input.classList.add('empty')
        } else {
          input.classList.remove('empty')
        }
      })
      event.preventDefault()
    }
  }
}
</script>

<style scoped>
section.content {
  background-color: var(--dark-cyan);
  padding: 80px 0;
  position: relative;
  z-index: 10;
  overflow: hidden;
}
section.content::after {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-contact-2.svg);
  position: absolute;
  bottom: 0;
  right: 0;
  transform: translateX(50%);
  z-index: -1;
}
@media (min-width: 769px) {
  section.content::before {
    content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-about-2-contact-1.svg);
    position: absolute;
    top: 0;
    left: 0;
    transform: translateX(-50%);
    z-index: -1;
  }
}
.row {
  display: flex;
  gap: 40px;
}
.info,
form {
  width: 100%;
}
.info h1 {
  color: white;
  font-size: 3rem;
  line-height: 3rem;
}
.info h3 {
  color: var(--salmon);
  margin: 30px 0;
  font-size: 1.5rem;
}
ul.detials li {
  display: flex;
  align-items: center;
  color: white;
  gap: 20px;
  font-weight: bold;
  font-size: 20px;
}
ul.detials li:not(:last-of-type) {
  margin-bottom: 15px;
}
form {
  width: 100%;
  display: grid;
  gap: 20px;
}
input,
textarea {
  font-family: 'Livvic', sans-serif;
  background-color: transparent;
  border: none;
  border-bottom: 2px solid white;
  outline: none;
  color: white;
  padding: 12px;
}
textarea {
  resize: none;
  height: 100px;
}
input::placeholder,
textarea::placeholder {
  color: #99b8bb;
  font-size: 14px;
  font-weight: 600;
}
input.empty,
textarea.empty {
  border-color: #f67e7e;
}
input.empty::placeholder,
textarea.empty::placeholder {
  color: #946b6e;
}
button.submit-btn {
  padding: 15px 12px;
  border: none;
  border-radius: 25px;
  max-width: 160px;
  font-size: 18px;
  font-weight: bold;
  color: var(--dark-cyan);
  display: block;
  transition: 0.3s;
  cursor: pointer;
}
button.submit-btn:hover {
  color: white;
  background-color: var(--salmon);
  transform: scale(1.1);
}
@media (max-width: 768px) {
  .row {
    flex-direction: column;
  }
  ul.detials li {
    font-size: 18px;
  }
}
</style>
