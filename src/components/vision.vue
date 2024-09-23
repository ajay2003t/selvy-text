<template>
  <section class="mission-vision">
    <div class="content-wrapper">
      <div class="card-container">
        <article class="mission-card">
          <iframe src="https://lottie.host/embed/73d0b98c-8ae2-4927-9a22-2c620b271aa2/jC8rCcHAgX.json" style="width: 200px;height: 200px;border: none;"></iframe>
          <h2 class="card-title">OUR MISSION</h2>
          <p class="card-description">
            At SelvyTex, we strive to be a global leader in<br> exceptional quality, client trust, and employee<br> well-being,
            driving innovation and<br> sustainability for a brighter, greener future.
          </p>
        </article>
        <article class="vision-card">
          <iframe src="https://lottie.host/embed/0dcdf4d2-fb63-4dc7-807c-ab2d1b330964/BunVuOy7BC.json" style="width: 200px;height: 200px;border: none;"></iframe>
          <h2 class="card-title">OUR VISION</h2>
          <p class="card-description">
            At <span class="highlight">SelvyTex</span>, we strive to be a global leader in<br> exceptional quality, client
            trust, and employee<br> well-being, driving innovation and<br> sustainability for a brighter, greener future.
          </p>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
.mission-vision {
  padding-top: 89px;
  margin-top: 8em;
}

.content-wrapper {
  background-color: rgba(224, 112, 64, 0.47);
  display: flex;
  justify-content: center;
  padding: 0 12em 97px;
}

.card-container {
  z-index: 10;
  margin-top: -89px;
  width: 100%;
  max-width: 1000px;
  display: flex;
  justify-content: space-between;
  gap: 50px;
}

.mission-card,
.vision-card {
  border-radius: 15px;
  background-color: #fff;
  box-shadow: 14px 14px 14px rgba(0, 0, 0, 0.25);
  border-top: 10px solid #e07040;
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  overflow: hidden;
  align-items: center;
  width: 50%;
  margin-right: 30px;
  padding: 45px 40px 85px;
  transition: all 5 ease;
}
.mission-card:hover
{
  transform: translateY(-20px);
}
.vision-card:hover
{
  transform: translateY(-20px);
}

.card-image {
  aspect-ratio: 1;
  object-fit: contain;
  object-position: center;
  width: 150px;
  max-width: 100%;
}

.card-title {
  color: #e07040;
  letter-spacing: 2px;
  margin-top: 25px;
  font: 600 40px/1 'Magra', sans-serif;
}

.card-description {
  color: rgba(0, 0, 0, 0.7);
  text-align: center;
  align-self: stretch;
  margin-top: 25px;
  font: 400 15px/27px 'Outfit', sans-serif;
}

.highlight {
  font-weight: 700;
  font-size: 20px;
  color: #e07040;
}

@media (max-width: 991px) {
  .content-wrapper {
    max-width: 100%;
    padding: 0 20px;
  }

  .card-container {
    max-width: 100%;
    flex-direction: column;
    align-items: stretch;
    gap: 40px;
  }

  .mission-card,
  .vision-card {
    max-width: 100%;
    width: 100%;
    padding: 45px 20px 85px;
  }

  .card-title {
    margin-top: 40px;
  }
}
</style>