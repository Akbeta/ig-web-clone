<template>
  <div class="home">


    <div class="timeline">
      <h1>Home</h1>
      <CustomText class="a1" tag="p">Merhaba dünya</CustomText>
      <CustomText class="a2" tag="p" size="small">Merhaba dünya</CustomText>
      <CustomText class="a3" tag="p" size="xsmall">Merhaba dünya</CustomText>
      <CustomText tag="p" size="xxsmall">Merhaba dünya</CustomText>
      <IconHome width="60" height="60" />
      <IconComment width="60" heigth="60" />
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
    </div>


    <div class="sidebar">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias blanditiis doloremque enim et eveniet expedita ipsa maxime nemo porro voluptas. Corporis cum eligendi minima officia quae quam repellendus unde veritatis.
      </p>
    </div>

  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import IconHome from '../../icons/home.svg'
import IconComment from '../../icons/comment.svg'

export default {
  name: 'Home',
  components: {
    CustomText,
    IconHome,
    IconComment
  }
}
</script>

<style scoped>
.home{
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
.sidebar{
  display: none;

  @media (--t) {
    display: block;
  }
}
</style>
