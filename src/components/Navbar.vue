<script>
// export default {
//     data() {
//         return {
//             name: "tweet",
//             maxLimit: 10
//         },
//         methods : {
//             cekInp(){
//                 this.name = this.name.substr(0, this.maxLimit);
//             }
//         }
//         computed : {
//             minLimit(){
//                 return this.maxLimit - this.name.length;
//             }
//         }
//     }
// }
</script>

<template>
 <div class="navbar">
    <h2 class="title">Simple Twitter Clone With Vue</h2>
    <div class="user">
        <div class="text">
            <p class="fullname">Elda Qotul Maulya</p>
            <p class="username">@eldamaulya</p>
        </div>
    </div>
 </div>
 <section class="section">
 <form class="form">
    <textarea class="tweet" name="tweet" id="tweet" placeholder="Write Something" rows="4"
    v-model="tweet" @input="cekInp" :class="{borderWar : !minLimit}">{{ minLimit }}/{{ maxLimit }}</textarea>
    <div class="footer">
        <p class="panjang">1/10</p>
        <div class="button">
            <button type="submit" class="button button-primary">Tweet</button>
        </div>
    </div>
</form>
</section>
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

.form {
    width: 100%;
    height: 100%;
    width: 100%;
    align-items: center;
    margin: auto;
    padding: 1rem;
}

.textarea {
    width: 100%;
    background-color: #ffffff0d;
}
</style>
