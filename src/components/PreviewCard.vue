<template>
  <div class="background">
    <div class="container">
      <div class="card sedans">
        <img src="../../images/icon-sedans.svg" alt="Sedan icon" />
        <h1>Sedans</h1>
        <p>
          Choose a sedan for its affordability and excellent fuel economy. Ideal
          for cruising in the city or on your next road trip.
        </p>
        <button>Learn More</button>
      </div>
      <div class="card suvs">
        <img src="../../images/icon-suvs.svg" alt="SUV icon" />
        <h1>SUVs</h1>
        <p>
          Take an SUV for its spacious interior, power, and versatility. Perfect
          for your next family vacation and off-road adventures.
        </p>
        <button>Learn More</button>
      </div>
      <div class="card luxury">
        <img src="../../images/icon-luxury.svg" alt="Luxury icon" />
        <h1>Luxury</h1>
        <p>
          Cruise in the best car brands without the bloated prices. Enjoy the
          enhanced comfort of a luxury rental and arrive in style.
        </p>
        <button>Learn More</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PreviewCard",
};
</script>

<style scoped>
.background {
  color: var(--very-light-gray);
  background-color: var(--very-light-gray);
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
}
.container {
  width: 920px;
  height: 500px;
  display: flex;
}
.card {
  width: 33%;
  padding: 48px;
  text-align: start;
}

.sedans {
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
  background-color: var(--clr-bright-orange);
}
.sedans > button {
  color: var(--clr-bright-orange);
}

.suvs {
  background-color: var(--clr-dark-cyan);
}
.luxury {
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
  background-color: var(--clr-very-dark-cyan);
}
h1 {
  font-family: "Big Shoulders Display";
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 48px;
  text-transform: uppercase;
}
p {
  color: var(--transparent-white);
}

button {
  width: 146px;
  height: 48px;
  border: none;
  border-radius: 24px;
  font-family: "Lexend Deca";
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 25px;
  margin-top: 88px;
}

button:hover {
  color: var(--very-light-gray);
  border: 2px solid var(--very-light-gray);
  background-color: transparent;
}

@media screen and (max-width: 1200px) {
  .background {
    height: 1600px;
    align-items: start;
    padding-top: 48px;
  }
  .container {
    width: 327px;
    flex-wrap: wrap;
  }
  .card {
    width: 100%;
  }
  .sedans {
    border-top-left-radius: 8px;
    border-bottom-left-radius: 0px;
    border-top-right-radius: 8px;
    background-color: var(--clr-bright-orange);
  }
  .luxury {
    border-top-right-radius: 0px;
    border-bottom-right-radius: 8px;
    border-bottom-left-radius: 8px;
    background-color: var(--clr-very-dark-cyan);
  }
}
</style>
