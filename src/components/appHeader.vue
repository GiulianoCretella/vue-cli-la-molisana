<template>
    <header>
        <div>
            <img src="../assets/images/la-molisana-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li  v-for="(item,index) in links" :key="index" :class="{'selected' : item.active}" @click="item.active = true">{{item.testo}}</li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
   name:'appHeader',
   data(){
       return {
           links:[
                {
                    testo:'Home',
                    link:'',
                    active:false,
                },
                {
                    testo:'Prodotti',
                    link:'',
                    active:true,
                },
                {
                    testo:'Chi siamo',
                    link:'',
                    active:false,
                },
                {
                    testo:'Contatti',
                    link:'',
                    active:false,
                }
            ]
       }
    }
}
</script>
<style lang="scss">
@import '../style/variables';
header{
    text-align: center;
    nav ul{
        display: flex;
        justify-content: center;
        li{
            list-style-type: none;
            padding: 10px;
        }
    }
}
    nav ul{
        display: flex;
    }
    .selected{
        background-color: $bg-azure;
    }
</style>
