<template>
    <div class="wrapper">
        <div v-for="bird in birds" :key="bird.id">
            <div class="container">
                <img :src="bird.src">   
                <h2>{{bird.bird}}</h2>
                 <PopUp v-bind:bird="bird" />  
             </div> 
                
        </div>
        
    </div>
</template>



<script lang="ts">
import PopUp from "@/components/PopUp.vue"
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component({
    components: {
        PopUp
    }
})
export default class Bird extends Vue {

    @Prop() birds: number | string | string | boolean | string | undefined


}

</script>





<style scoped>

    .wrapper{
        display: grid;
        grid-template-columns:repeat(3,1fr);
       
    }

    .wrapper img{
        width:100%;
        height:100%;
    }

    .container {
        position: relative;
        text-align: center;
        color: white;
        width:100%;
        height:100%;
      
    }

    h2 {
        position: absolute;
        bottom: 8px;
        left: 16px;
    }



</style>