<script setup></script>

<template>
  <section class="articles">
    <article>
      <div class="card-container">
        <div class="card">
          <div class="front-content">
            <p>Proyecto 1</p>
          </div>
          <div class="content">
            <p class="heading">Proyecto 1</p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipii voluptas ten
              mollitia pariatur odit, ab minus ratione adipisci accusamus vel
              est excepturi laboriosam magnam necessitatibus dignissimos
              molestias.
            </p>
          </div>
        </div>
      </div>
    </article>
    <article>
      <div class="card-container">
        <div class="card">
          <div class="front-content">
            <p>Proyecto 2</p>
          </div>
          <div class="content">
            <p class="heading">Proyecto 2</p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipii voluptas ten
              mollitia pariatur odit, ab minus ratione adipisci accusamus vel
              est excepturi laboriosam magnam necessitatibus dignissimos
              molestias.
            </p>
          </div>
        </div>
      </div>
    </article>
    <article>
      <div class="card-container">
        <div class="card">
          <div class="front-content">
            <p>Proyecto 3</p>
          </div>
          <div class="content">
            <p class="heading">Proyecto 3</p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipii voluptas ten
              mollitia pariatur odit, ab minus ratione adipisci accusamus vel
              est excepturi laboriosam magnam necessitatibus dignissimos
              molestias.
            </p>
          </div>
        </div>
      </div>
    </article>
  </section>
</template>

<style scoped>
.articles {
  display: flex;
  flex-direction: row;
  gap: 40px; /* Espacio entre las cartas */
}

.card-container {
  width: 300px;
  height: 300px;
  position: relative;
  border-radius: 10px;
  box-shadow: 0 10px 20px rgba(255, 255, 255, 0.2);
  overflow: hidden;
}

.card {
  width: 100%;
  height: 100%;
  border-radius: inherit;
}

.card .front-content {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.32, 1);
}

.card .front-content p {
  font-size: 32px;
  font-weight: 700;
  opacity: 1;
  background: linear-gradient(-45deg, #36a8fa 0%, #ff0f7b 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.32, 1);
}

.card .content {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  gap: 10px;
  background: linear-gradient(-45deg, #36a8fa 0%, #ff0f7b 100%);
  color: #e8e8e8;
  padding: 20px;
  line-height: 1.5;
  border-radius: 5px;
  pointer-events: none;
  transform: translateX(-96%);
  transition: all 0.6s cubic-bezier(0.23, 1, 0.32, 1);
}

.card .content .heading {
  font-size: 32px;
  font-weight: 700;
}

.card:hover .content {
  transform: translateY(0);
}

.card:hover .front-content {
  transform: translateX(-30%);
}

.card:hover .front-content p {
  opacity: 0;
}

@media (max-width: 768px) {
  .articles {
    flex-direction: column;
  }
}
</style>
