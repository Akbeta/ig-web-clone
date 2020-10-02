<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size"/>
  </figure>

</template>

<script>
export default {
  name: 'Avatar',
  props: {
    src: {
      type: String,
      default:
          'https://instagram.fsaw1-8.fna.fbcdn.net/v/t51.2885-19/s150x150/42632011_317572295464928_3823266370913566720_n.jpg?_nc_ht=instagram.fsaw1-8.fna.fbcdn.net&_nc_ohc=TYCP6p6_FxIAX83tHV6&oh=f2b21bf674c5c5096fdc21348a94ba3e&oe=5F9FDDCB'
    },
    alt: {
      type: String
    },
    size: {
      type: Number
    }
  }
}
</script>

<style scoped>
.avatar {
  display: inline-flex;
  padding: 2px;
  border-radius: 999px;
  background: linear-gradient(
      219deg,
      rgba(184, 63, 140, 1) 0%,
      rgba(237, 158, 90, 1) 100%
  );

  img {
    border-radius: inherit;
    border: 2px solid white;
  }
}
</style>