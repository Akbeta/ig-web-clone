<template>
  <div class="home">


    <div class="timeline">
      <h1>Home</h1>

      <Avatar :size="40"/>
    </div>


    <div class="sidebar">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita
        ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
    </div>

  </div>
</template>

<script>

import Avatar from "@/components/avatar";

export default {
  name: 'Home',
  components: {
    Avatar
  }
}
</script>

<style scoped>
.home {
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;

  @media (--t) {
    max-width: none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;
  }
}

.sidebar {
  display: none;

  @media (--t) {
    display: block;
  }
}
</style>
