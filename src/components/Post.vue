<template>
  <div class="post">
      <!-- header -->
      <header class="header section">

        <div class="header-author">
          <Avatar :size="40" />
          <div class="header-author-info">
            <div class="">
              <CustomText tag="b">akinankarali</CustomText>
            </div>
            <div class="">
              <CustomText size="xsmall">Montreal, Quebec</CustomText>
            </div>
          </div>
        </div>
        <div class="header-more">
          <button type="button">
            <IconMore />
          </button>
        </div>

      </header>
      <!-- media -->
      <div class="post-media">
        <img src="https://instagram.fbtz1-3.fna.fbcdn.net/v/t51.2885-15/sh0.08/e35/s750x750/120535466_670681246985841_3776624366342773200_n.jpg?_nc_ht=instagram.fbtz1-3.fna.fbcdn.net&_nc_cat=109&_nc_ohc=IS--UnMHsFEAX-roTED&oh=1b00386c5627fdb6a4706192d535c412&oe=5FA1C2BD" alt="">
      </div>
      <!-- actions -->
      <div class="action-buttons section">
        <button type="button">
          <IconLike />
        </button>
        <button type="button">
          <IconComment />
        </button>
        <button type="button">
          <IconDirect />
        </button>
        <button type="button" class="action-save">
          <IconSave />
        </button>
      </div>
      <!-- view count -->
      <div class="view-count section">
        <CustomText tag="b">1.345 beğenme</CustomText>
      </div>
      <!-- comment list -->
    
      <!-- datatime -->
    
      <!-- comment form -->
  </div>
</template>

<script>
import Avatar from "@/components/Avatar";
import CustomText from "@/components/CustomText";
import IconMore from "@/icons/more.svg"
import IconLike from "@/icons/like.svg"
import IconComment from "@/icons/comment.svg"
import IconDirect from "@/icons/direct.svg"
import IconSave from "@/icons/save.svg"

export default {
  name: 'Post',
  components: {
    CustomText,
    Avatar,
    IconMore,
    IconLike,
    IconComment,
    IconDirect,
    IconSave,
  }
}
</script>

<style scoped>
.post{
  border-radius: 3px;
  border: 1px solid rgb(var(--b6a));
}
.section {
  padding-left: 16px;
  padding-right: 16px;
}
.header{
  height: 60px;
  display: flex;
  align-items: center;
  &-author{
    display: flex;
    align-items: center;
    &-info{
      margin-left: 8px;
    }
  }
  &-more{
    margin-left: auto;
  }
}
.action-buttons {
  height: 45px;
  display: flex;
  align-items: center;

  button{
    margin-right: 16px;
  }
  .action-save{
    margin-left: auto;
    margin-right: 0;
  }
}
</style>