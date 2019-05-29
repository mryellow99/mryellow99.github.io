<template>
  <section class="container">
      <article class="top_images">
        <img src="~/assets/top1.jpg">
        <img src="~/assets/top2.jpg">
        <div class="double_pieces">
          <img src="~/assets/top3.jpg">
          <img src="~/assets/top3.jpg">
        </div>
      </article>
  </section>
</template>

<style lang="scss">
.container {
  margin: 4% auto 64px;
  padding: 0 8px;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.top_images {
  max-width: 800px;
  > img {
    width: 100%;
    margin-bottom: 4%;
  }
  .double_pieces {
    display: flex;
    width: 100%;
    img {
      height: 100%;
      width: 48%;
      object-fit: contain;
      &:first-child {
        margin-right: auto;
      }
      &:last-child {
        margin-left: auto;
      }
    }
  }
}
</style>