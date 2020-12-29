<template>
  <main>
    <h1>About</h1>
    <section class="content">
      <div>
        <img alt="Photo of Evan Roane" class="photo" src="~/assets/img/evan-roane.jpg" />
      </div>
      <div class="bio">
        <p>Hi, I'm Evan. I love experiencing things that blow my hair back.</p>
        <p>I work as a software engineer specializing in creating delightful user experiences. I enjoy working in an industry where I get to create beauty and improve everyday tasks for people.</p>
        <p>I'm inspired by big ideas and high ideals. I get most excited when I have opportunities to have a positive impact on others through creating physical artifacts, software, or spaces for people to flourish.</p>
      </div>
    </section>
  </main>
</template>

<style scoped>
p {
  margin-bottom: 1rem;
}

.content {
  display: flex;
}

.bio {
  width: 800px;
  font-size: 1.2rem;
}

.photo {
  height: 50vh;
  object-fit: scale-down;
  margin-right: 2rem;
}
</style>
