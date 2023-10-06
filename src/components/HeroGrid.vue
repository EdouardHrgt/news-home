<script setup></script>

<template>
  <main class="grid">
    <div class="col-1">
      <div class="col-1-img">
        <img src="../assets/images/image-web-3-desktop.jpg" alt="web 3 image" class="web-3-pc" />
        <img src="../assets/images/image-web-3-mobile.jpg" alt="web 3 image" class="web-3-mobile" />
      </div>
      <div class="col-1-txt flex">
        <h1>The Bright Future of Web 3.0?</h1>
        <div class="col-1-p-btn">
          <p class="col-1-p">
            We dive into the next evolution of the web that claims to put the power of the platforms back into the hands of the
            people. But is it really fulfilling its promise?
          </p>
          <button>read more</button>
        </div>
      </div>
    </div>

    <!-- Right column -->
    <div class="col-2">
      <h2>New</h2>
      <ul>
        <li>
          <h3>Hydrogen VS Electric Cars</h3>
          <p class="col-2-p">Will hydrogen-fueled cars ever catch up to EVs?</p>
        </li>
        <li class="li-2">
          <h3>The Downsides of AI Artistry</h3>
          <p class="col-2-p">What are the possible adverse effects of on-demand AI image generation?</p>
        </li>
        <li>
          <h3>Is VC Funding Drying Up?</h3>
          <p class="col-2-p">Private funding by VC firms is down 50% YOY. We take a look at what that means.</p>
        </li>
      </ul>
    </div>
  </main>
</template>

<style scoped>
.grid {
  margin-top: var(--size-2);
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: var(--size-2);
  grid-row-gap: 0px;
  padding-inline: var(--inline-padding);
}
.web-3-mobile {
  display: none;
}
.col-1 {
  grid-area: 1 / 1 / 2 / 3;
}
.col-2 {
  grid-area: 1 / 3 / 2 / 4;
  background-color: var(--clr-very-dark-blue);
  padding: 1.5rem;
}
.col-1-p-btn {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.col-1-txt {
  margin-top: var(--size-2);
  justify-content: space-between;
}

h1 {
  font-size: 3rem;
  font-weight: 800;
  color: var(--clr-very-dark-blue);
  max-width: 20rem;
  line-height: 3rem;
}
h2 {
  font-size: 2.5rem;
  font-weight: 800;
  color: var(--clr-orange);
}
h3 {
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--clr-white);
  margin-block: 0.8rem;
  cursor: pointer;
  transition: color 0.4s ease-in-out;
}
h3:hover {
  color: var(--clr-orange);
}

p {
  font-size: var(--p-size);
  color: var(--clr-dark-grayish-blue);
  font-weight: 500;
}

.col-1-p {
  max-width: 24rem;
  margin-bottom: 1rem;
  line-height: 1.3rem;
}

button {
  background-color: var(--clr-red);
  color: var(--clr-white);
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: 500;
  padding: 0.8rem 2.2rem;
  transition: 0.4s ease-in-out;
}
button:hover {
  background-color: var(--clr-very-dark-blue);
}

li {
  padding-block: 1rem var(--size-2);
}
.li-2 {
  border-block: 1px solid var(--clr-dark-grayish-blue);
}
.col-2-p {
  max-width: 19rem;
}

@media screen and (max-width: 1250px) {
  .grid {
    grid-column-gap: var(--size-3);
  }
}

@media screen and (max-width: 1024px) {
  .grid {
    margin-top: var(--size-2);
    grid-template-columns: 1fr;
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 1rem;
  }
  .col-1 {
    grid-area: 1 / 1 / 2 / 2;
  }
  .col-2 {
    grid-area: 2 / 1 / 3 / 2;
  }
  .col-1-txt {
    margin-top: var(--size-2);
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
  }
  .col-1-p {
    margin-bottom: 0;
    margin-block: 1.5rem;
  }
  .col-2 {
    margin-block: 1rem;
    text-align: center;
  }
  .col-2-p {
    max-width: 19rem;
    margin-inline: auto;
  }
}

@media screen and (max-width: 768px) {
  .web-3-mobile {
    display: block;
    margin-inline: auto;
  }
  .web-3-pc {
    display: none;
  }
}
</style>
