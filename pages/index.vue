<template>
  <div>
    <section class="intro">
      <h1>Get the lates tech news</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTb4Q83x0SiyQm_kFSNABpN-wqzGF-JHpQE8Q&usqp=CAU"
        title="Heloo"
        previewText="best blog"
      />
      <PostPreview
        id="2"
        thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSjHsEsxJynd7SZgg8I-ezYXzv2pVuT0KULKJvfEjvjYosX8TNr8ZQJlin8c9SXUjTbr9Y&usqp=CAU"
        title="Heloo there"
        previewText="best blog ever"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "../components/Posts/PostPreview.vue";
export default { components: { PostPreview } };
</script>

<style scoped>
.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;

  align-items: center;
  justify-content: center;
  text-align: center;
}
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
  background-image: url("~assets/images/images.png");
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}
</style>
