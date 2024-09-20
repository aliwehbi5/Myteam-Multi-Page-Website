<template>
  <div class="ready">
    <div class="container content">
      <h1>Ready to get started?</h1>
      <RouterLink to="/contact" class="contact-btn">contact us </RouterLink>
    </div>
  </div>
</template>

<style scoped>
.ready {
  padding: 50px 0;
  background-color: var(--salmon);
  position: relative;
}
.ready::before {
  content: url(https://myteam-multi-page-website-teal.vercel.app/images/bg-pattern-home-6-about-5.svg);
  position: absolute;
  bottom: -7px;
  left: 0;
  z-index: 0;
}
.ready .content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  position: relative;
}
.ready h1 {
  font-size: 2.5rem;
  line-height: 2.5rem;
  text-align: center;
  font-weight: bold;
  color: var(--midnight-blue);
}
.ready .contact-btn {
  color: var(--midnight-blue);
  font-size: 18px;
  font-weight: 600;
  padding: 12px 30px;
  border-radius: 30px;
  border: 2px solid var(--midnight-blue);
  transition: 0.3s;
  display: block;
}
.ready .contact-btn:hover {
  color: white;
  background-color: var(--midnight-blue);
  transform: scale(1.1);
}
@media (max-width: 767px) {
  .ready .content {
    flex-direction: column;
    justify-content: center;
  }
}
</style>
