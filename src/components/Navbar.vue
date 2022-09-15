<script>
export default {
  inject: ['fullname', 'username', 'profile'],
  data(){
    return {
      Foto:this.profile
    }
  }
};
</script>

<template>
 <div class="navbar">
    <h2 class="title">Simple Twitter Clone With Vue</h2>
    <div class="user">
        <div class="text">
            <p>{{ fullname }}</p>
            <p>{{ username }}</p>
        </div>
    </div>
    <div class="profile">
        <img :src="Foto" alt="">
    </div>
 </div>
</template>

<style>
.navbar{
    height: 100%;
    width: 100%;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: aquamarine;
}

.profile{
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
</style>
