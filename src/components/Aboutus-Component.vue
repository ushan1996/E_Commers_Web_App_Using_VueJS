<template>
    <v-container class="pt-15">
        <v-row>
            <v-col lg="6">
                <img width="100%" src="./../assets/9.jpg" alt="">
            </v-col>
            <v-col lg="6">
               <v-subheader class="about-us-header">About Us</v-subheader>
               <h2 class="text-center">People who love luxury watches inspire us as much as precious timepieces. Thats why sellers and buyers of luxury watches have our undivided attention.</h2>
               <p class="text-center">We know that our company wouldn’t exist without valuable watches and enthusiastic watch lovers. But we are not only fond of high-quality timepieces and their admirers. The complexities of information technology and the challenges of global markets also motivate us to push ourselves further every day. Because web and mobile technologies are our core competencies. </p>
            </v-col>
        </v-row>
    </v-container>
</template>
<script>
    export default{
        name: "AboutComponent"
    }
</script>
<style>
    .about-us-header{
        font-size: 50px;
        font-weight: 480;
        padding-left: 200px;
        padding-top: 150px;
    padding-bottom: 56px;
    }
    us-header.theme--light {
    color: black;
}
</style>