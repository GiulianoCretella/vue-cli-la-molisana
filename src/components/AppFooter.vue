<template>
    <div class="footer">
        <div class="container">
            <img src="../assets/images/la-molisana-logo.png" alt="">
            <ul>
                <span>IL PASTIFICIO</span>
            <li class="listaFooter" v-for="(item,index) in pasta" :key="index">{{item.text}}</li>
            </ul>
        </div>
        <div class="img-footer">
            <img src="../assets/images/footer-montagne-bottom.jpg" alt="">
        </div>
    </div>
   
</template>
<script>
export default {
   nome:'AppFooter',
   data(){
       return{
            
        }
    },
    props:['pasta']
}
</script>
<style lang="scss" scoped>
@import '../style/variables';
.footer{
    width: 100%;
    .container{
         display: flex;
         align-content: center;
         align-items: center;
         justify-content: space-around;
         width: 100%;
         span{
             font-size: 1em;
             color:$primaryText;
             font-weight: bold;
         }
         li{
             list-style-type: none;
             color: gray;
             font-size: 0.8em;
         }
    }
    .img-footer{
        width: 100%;
        img{
            width: 100%;
        }
    }
}
    
</style>