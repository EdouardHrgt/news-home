<template>
  <ul class="flex">
    <li>
      <div class="card-img">
        <img src="../assets/images/image-retro-pcs.jpg" alt="retro pcs" />
      </div>
      <div class="card-txt">
        <p><span>01</span></p>
        <h4>Reviving Retro PCs</h4>
        <p>What happens when old PCs are given modern upgrades?</p>
      </div>
    </li>
    <li class="card">
      <div class="card-img">
        <img src="../assets/images/image-top-laptops.jpg" alt="top laptops" />
      </div>
      <div class="card-txt">
        <p><span>02</span></p>
        <h4>Top 10 Laptops of 2022</h4>
        <p>Our best picks for various needs and budgets.</p>
      </div>
    </li>
    <li class="card">
      <div class="card-img">
        <img src="../assets/images/image-gaming-growth.jpg" alt="gaming growth" />
      </div>
      <div class="card-txt">
        <p><span>03</span></p>
        <h4>The Growth of Gaming</h4>
        <p>How the pandemic has sparked fresh opportunities.</p>
      </div>
    </li>
  </ul>
</template>

<style scoped>
ul {
  justify-content: space-between;
  gap: 1rem;
  margin-top: 7rem;
  padding-inline: var(--inline-padding);
}

li {
  display: flex;
  gap: 1rem;
  width: 100%;
}

.card-img {
  height: 16rem;
  width: 13rem;
  flex: 1;
}
.card-txt {
  flex: 1;
}

.card-img img {
  object-fit: cover;
  width: inherit;
  height: inherit;
}

p span {
  color: var(--clr-grayish-blue);
  font-size: 3rem;
  letter-spacing: 1px;
}

h4 {
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--clr-very-dark-blue);
  margin-block: 1rem;
}

p {
  font-size: var(--p-size);
  color: var(--clr-dark-grayish-blue);
  font-weight: 500;
}

@media screen and (max-width: 1024px) {
  ul {
    flex-direction: column;
    margin-top: 2.5rem;
    gap: 2rem;
    margin-bottom: 2rem;
  }
  .card-img {
    flex: unset;
    width: 15rem;
  }
  .card-txt p {
    max-width: 17rem;
  }
}

@media screen and (max-width: 768px) {
  ul {
    flex-direction: column;
    margin-top: 2.5rem;
    gap: 2rem;
    margin-bottom: 2rem;
  }
  .card-img {
    height: auto;
    width: 12rem;
    flex: unset;
  }
}
@media screen and (max-width: 500px) {
  .card-img {
    width: 9rem;
  }
  h4 {
    font-size: 1.1rem;
    margin-block: 0.3rem;
  }
}
</style>
