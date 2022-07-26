
<template>  
    <v-carousel cycle height="500" hide-delimiter-background show-arrows-on-hover>
         <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src" reverse-transition="fade-transition"  ></v-carousel-item>
    </v-carousel>
</template>
<script>
    export default{
        name:"SliderComponent",
        data () {
        return {
            items: [
            {
                src: 'https://ae01.alicdn.com/kf/H5311f487c2414c67abc66e702ea82aa0g.jpg',
            },
            {
                src: 'https://ae01.alicdn.com/kf/H2cee95d1a186450eae488afa6c25728fD.jpg',
            },
            
            {
                src: 'https://ae01.alicdn.com/kf/H3dce6a7966cc49d999caf00fb536a5a12.jpg',
             },
            {
                src: 'https://ae01.alicdn.com/kf/S5f7ed3003a4a4ce6929311384ecd4ba9J.jpg',
            },
            ],
        }
        },
    }
</script>
<style>
    
</style>