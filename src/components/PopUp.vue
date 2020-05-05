<template>
    <div>
        <div class="arrow" @click="showPopUp">
                        <p>info</p>
        </div>
        <div class="popup" v-bind:class="{'hidden':bird.hidden}">
                <p> {{bird.content}}</p>
                
        </div>
    </div>
</template>



<script lang="ts">
import { Component,Prop, Vue } from 'vue-property-decorator';


@Component
export default class PopUp extends Vue {

    

    @Prop() bird: any | undefined


    showPopUp(){
        this.bird.hidden = !this.bird.hidden;
    }


}


</script>


<style scoped>

    .popup {
        position:absolute;
        text-align: center;
        background: orangered;
        width:100%;
        height:100%;
        bottom:0px;
        
    }
    .hidden {
        visibility: hidden;
    }

    .popup p {
        color: antiquewhite;
    }

     .arrow {
        z-index: 10;
        position: absolute;
        bottom: 28px;
        right: 16px;
        height: 30px;
        width: 30px;
        background: orange;
        border: 1px;  
        border-radius: 5px;    
        text-align: center;   
    }

    .arrow p {
        z-index: 11;
        position: absolute;
        left: 50%;
        transform: translate(-50%, -50%);
    }

</style>