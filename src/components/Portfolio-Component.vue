<template>
    <v-container class="my-15">
        <v-row justify="center">
                <v-col lg="12" class="text-center">
                     <v-subheader class="text-h4 justify-center">Types of Watches</v-subheader> 
                     <p>Traditional Sourcing Brought Online. Find Quality Products & Contact Verified Suppliers! Reduce Costs With Factory Direct Sourcing. Low MOQ, OEM/ODM Available.</p>
                </v-col>
                <v-col lg="12">
                    <div class="text-center">
                        <v-chip large @click="activePortfolio= 'aaa'" :color="activePortfolio=='aaa'? 'black':''"  class=" mr-40 pa-40 white--text">Watch for Men</v-chip>
                         <v-chip large @click="activePortfolio= 'bbb'" :color="activePortfolio=='bbb'? 'black':''" class="mx-5 white--text x-large">Watch for Ladies</v-chip>
                          <v-chip large @click="activePortfolio= 'ccc'" :color="activePortfolio=='ccc'? 'black':''"  class="mx-5 white--text ">Watch for Kids</v-chip>
                         
                    </div>
                </v-col>
                <slot v-if="activePortfolio == 'aaa'">
                     <v-col lg="3" v-for="(aaa,aaaindex) in aaa " :key="aaaindex">
                     <v-card>
                         <v-img
                             :src="aaa.image" 
                             class="white--text align-end"
                             gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                              height="200px"
                             >
                            <v-card-title>{{aaa.title}}</v-card-title>
                        </v-img>
                     </v-card>
                </v-col>
                </slot>
               <slot v-if="activePortfolio == 'bbb'">
                     <v-col lg="3" v-for="(bbb,bbbindex) in bbb " :key="bbbindex">
                     <v-card>
                         <v-img
                             :src="bbb.image" 
                             class="white--text align-end"
                             gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                              height="200px"
                             >
                            <v-card-title>{{bbb.title}}</v-card-title>
                        </v-img>
                     </v-card>
                </v-col>
                </slot>
                 <slot v-if="activePortfolio == 'ccc'">
                     <v-col lg="3" v-for="(ccc,cccindex) in ccc " :key="cccindex">
                     <v-card>
                         <v-img
                             :src="ccc.image" 
                             class="white--text align-end"
                             gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                              height="200px"
                             >
                            <v-card-title>{{ccc.title}}</v-card-title>
                        </v-img>
                     </v-card>
                </v-col>
                </slot>
        </v-row>
    </v-container>
</template>
<script>
    export default{
        name:"PortfolioComponent",
        data(){
            return{
                activePortfolio: 'aaa',
                aaa:[
                    {title:'Style 1',image:'https://ae01.alicdn.com/kf/Hfb9312aca31d4cf6b0a41d6b31f4e3bb7.jpg'},
                    {title:'Style 2',image:'https://ae01.alicdn.com/kf/S60295ccb19964d8390a4db51376a401fU.jpg'},
                    {title:'Style 3',image:'https://ae01.alicdn.com/kf/H0a4048cc096f4f609d8f37df88faf06ek.jpg'},
                    {title:'Style 4',image:'https://ae01.alicdn.com/kf/H292f171e1b3a46099e4279095a3f1098v.jpg'},
                    {title:'Style 5',image:'https://ae01.alicdn.com/kf/Hb54d3bd53a454e6f9fe4df8beef6eb3fD.jpg'},
                    {title:'Style 6',image:'https://ae01.alicdn.com/kf/H07bc6f76e2704a92bf9ad6da27ecb623K.jpg'},
                    {title:'Style 7',image:'https://ae01.alicdn.com/kf/Sd713966d5ab247c195803103dc694b6b4.jpg'},
                    {title:'Style 8',image:'https://ae01.alicdn.com/kf/H419901c3604d435faa14a278c6b68a97Z.jpg'},
                ],
                 bbb:[
                    {title:'Style 1',image:'https://ae01.alicdn.com/kf/H96e22e297d9142799fe952fa5e0b1abbu.jpg'},
                    {title:'Style 2',image:'https://ae01.alicdn.com/kf/H0447b3d4a4234858bd1b12452cc26430t.jpeg'},
                    {title:'Style 3',image:'https://ae01.alicdn.com/kf/Se882e264206247c1b76de8e0e6601684a.jpg'},
                    {title:'Style 4',image:'https://ae01.alicdn.com/kf/H6c9fdfbf83ab4aa8be2c7c30978e6a3fj.jpg'},
                    {title:'Style 5',image:'https://ae01.alicdn.com/kf/S3a1d117cde894f6cbcedda79366e779eT.jpg'},
                    {title:'Style 6',image:'https://ae01.alicdn.com/kf/Sf9dab1a4b3004d249460b789381d5bafk.jpg'},
                    {title:'Style 7',image:'https://ae01.alicdn.com/kf/H7ab4509b191441aeb4f6a52016f307beG.jpg?width=800&height=800&hash=1600'},
                     {title:'Style 8',image:'https://ae01.alicdn.com/kf/H820e5d6fcb9445a09e6b7d9aa7abafd68.jpg?width=1000&height=1000&hash=2000'},
                ],
                 ccc:[
                    {title:'CCC 1',image:'https://ae01.alicdn.com/kf/S7c4b37e9dfa8429382ed9b88044e20053.jpg'},
                    {title:'web App 2',image:'https://ae01.alicdn.com/kf/H14f82eeb90114cad8a244b0248de5022D.jpg'},
                    {title:'web App 3',image:'https://ae03.alicdn.com/kf/Sec8b0396b8e4424caa167395c4a661cab.jpg'},
                    {title:'web App 4',image:'https://ae01.alicdn.com/kf/Hea8103c299f84a16ad1c3411d48d51b9J.jpg'},
                    {title:'web App 5',image:'https://ae01.alicdn.com/kf/S1b2419199f3c4fad931c7c7bafce2540D.jpg'},
                    {title:'web App 6',image:'https://ae01.alicdn.com/kf/Hb07b49b1e08b494492ea1cb05042c192l.jpg?width=1080&height=1368&hash=2448'},
                    {title:'web App 7',image:'https://ae01.alicdn.com/kf/S606de5a046d34f379ea18db6ea3ce744g.jpg'},
                     {title:'web App 8',image:'https://ae01.alicdn.com/kf/Sb7ef03e9968245c19729e90adf5c971f4.jpg?width=800&height=800&hash=1600'},
                ]
            }
        }
    }
</script>
<style>
    h4.justify-center.theme--light {
    color: black;
    font-size: 50px;
        font-weight: 480;
}
</style>