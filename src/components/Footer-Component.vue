
<template>
    <v-footer padless>
        <v-col lg="12">
            <v-row justify="center">
                <v-col lg="4" class="text-center"> <v-toolbar-title>Smart Smapping</v-toolbar-title>
                    <v-card-text>
                        <v-btn v-for="icon in icons" :key="icon" class="mx-4 black--text" icon>
                        <v-icon size="24px"> {{ icon }} </v-icon>
                    </v-btn>
                    </v-card-text>
                    <v-subheader>Traditional Sourcing Brought Online. Find Quality Products & Contact Verified Suppliers! Reduce Costs With Factory Direct Sourcing. Low MOQ, OEM/ODM Available.</v-subheader>
                    <v-form class="mt-4">
                        <v-text-field label='Email' outlined dense/>
                        <v-btn rounded color="black" class="mx-5 white--text">Subscribe Us</v-btn>
                    </v-form>
                </v-col>
               
            </v-row>
             <div class="mt-10">
                    <v-divider></v-divider>
                    <v-subheader>@copyright smartshopping All Rights Reserved {{ new Date().getFullYear() }} — <strong>Ushan Jayamanne</strong>
                        <v-spacer />
                        <strong>Designed By Ushan Jayamanne</strong>
                    </v-subheader>
                </div>
        </v-col>
        
  </v-footer>
</template>
<script>
    export default{
        name:"FooterComponent",
        data(){
            return{
                icons: [
                    'mdi-facebook',
                    'mdi-twitter',
                    'mdi-linkedin',
                    'mdi-instagram',
                ],
            }
        }
    }
</script>
<style>
    
</style>