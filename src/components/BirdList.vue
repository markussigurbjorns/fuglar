<template>
    <div>
        <Bird v-bind:birds="birds" />
    </div>
</template>

<script lang="ts">
import Bird from "@/components/Bird.vue"
import { Component, Vue } from 'vue-property-decorator';

@Component({
    components: {
        Bird
    }
})
export default class BirdList extends Vue {

    birds = [{
        id: 1,
        bird: "Heiðlóa",
        content: "Lasdasdf",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.ovAc-TzkdyzDO4eDK3IySAHaFC%26pid%3DApi&f=1"
    },
    {
        id: 2,
        bird: "Stari",
        content: "Lasdfjaæhfghdf",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.SOb0tyP4lyu81y4KdgiIrQHaE8%26pid%3DApi&f=1"
    },
    {
        id: 3,
        bird: "Álft",
        content: "Lasdfjaæsasdfasdf",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.YVKl7d2ObkPhBQYjsW73GAHaEx%26pid%3DApi&f=1"
    },
    {
        id: 4,
        bird: "Grágæs",
        content: "Grágæs",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.Auud4DIR0Hq8sWUariJ4PgHaE8%26pid%3DApi&f=1"

    },
    {
        id: 5,
        bird: "Haförn",
        content: "asdifjaksdkfjhlaksjdhf",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.4lccZd8d_GKDJYvdG2_JmAHaFk%26pid%3DApi&f=1"


    },
    {
        id: 6,
        bird: "Ugla",
        content: "asdfhpasdfh83h4foe47fhe4f",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Ffarm5.staticflickr.com%2F4052%2F4494218601_9342b11de9_z.jpg&f=1&nofb=1"


    },
    {
        id: 7,
        bird: "Stokkönd",
        content: "asdflkjaælsdkjfælasdlfjkaælsdkf",
        hidden: true,
        src: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flive.staticflickr.com%2F7203%2F6788694936_9fca7070bf.jpg&f=1&nofb=1"


    }]
  
}

</script>


<style scoped>

   


</style>