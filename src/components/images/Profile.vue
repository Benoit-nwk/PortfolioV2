<script setup>

</script>

<template>
      <div class="profile-picture">
            <img src="../images/profile_picture.webp" alt="profile_picture">
      </div>
</template>

<style scoped>

.profile-picture{
      width: 100%;
      display: flex;
      justify-content: center;
      margin: 2rem 0;
      > img{
            width: 60%;
      }
}

@media screen and (min-width: 1080px){
      .profile-picture{
            > img{
                  width: 20%;
            }
      }
      
}

</style>
