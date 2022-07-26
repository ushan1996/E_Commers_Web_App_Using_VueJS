<template>
     <v-container class="my-15">
        <v-row justify="center">
                <v-col lg="12" class="text-center"><v-subheader class="text-h4 justify-center">Hot Sale Products</v-subheader> <p>You can find every toys you want here</p></v-col>
                <v-col lg="4" v-for="project in 1" :key="project">
                    <v-card :loading="loading" class="mx-auto my-12" max-width="374">
                    <v-img height="350" src="https://ae01.alicdn.com/kf/H7f2544d6bb3647d9aa1df19569c00e6dJ.jpg_480x480Q90.webp"></v-img>
                    <v-card-title>Fashion Watches Men Luxury Calendar Quartz Wristwatch for Man Stainless Steel Band Waterproof Luminous Male Clock</v-card-title>
                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-rating :value="5" color="amber" dense half-increments readonly size="25"></v-rating>
                        <div class="grey--text ms-4"> 5 (3213) </div>
                      </v-row>
                      <div class="my-4 text-subtitle-1"><h2>US $9.89</h2></div>
                      <div>Size and weight<br>band lenght: 25cm<br>Dial diameter: 45mm<br>Dial thickness:12mm<br>Band width: 24mm</div>
                    </v-card-text>
                    <v-divider class="mx-4"></v-divider>
                    <v-card-actions>
                      <v-btn color="black" rounded class="white--text">Buy Now</v-btn>
                      <v-btn color="black" rounded class="white--text">Add to Cart</v-btn>
                    </v-card-actions>
                  </v-card>
                </v-col>
                <v-col lg="4" v-for="project in 1" :key="project">
                    <v-card :loading="loading" class="mx-auto my-12" max-width="374">
                    <v-img height="350" src="https://ae01.alicdn.com/kf/Hf2221ed6285d4057ab793a50352955f7e.jpg_480x480Q90.webp"></v-img>
                    <v-card-title>Free Dropping Role Watch Men Quartz Mens Watches Top Luxury Brand Watch Man Gold Stainless Steel Relogio Masculino Waterproof</v-card-title>
                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-rating :value="4.5" color="amber" dense half-increments readonly size="25"></v-rating>
                        <div class="grey--text ms-4"> 4.5 (1413) </div>
                      </v-row>
                      <div class="my-4 text-subtitle-1"><h2>US $16.14</h2></div>
                      <div>Size and weight<br>band lenght: 31cm<br>Dial diameter: 55mm<br>Dial thickness:18mm<br>Band width: 24mm</div>
                    </v-card-text>
                    <v-divider class="mx-4"></v-divider>
                    <v-card-actions>
                      <v-btn color="black" rounded class="white--text">Buy Now</v-btn>
                      <v-btn color="black" rounded class="white--text">Add to Cart</v-btn>
                    </v-card-actions>
                  </v-card>
                </v-col>
                <v-col lg="4" v-for="project in 1" :key="project">
                    <v-card :loading="loading" class="mx-auto my-12" max-width="374">
                    <v-img height="350" src="https://ae01.alicdn.com/kf/S7bdc2ec71798436b830cbae526d1a44c5.jpg_480x480Q90.webp"></v-img>
                    <v-card-title>2022 Gold Top Brands Men Wristwatches Waterproof Luxury Golden Wrist Watch For Male Clock Dropshipping Gifts Relogio Masculino</v-card-title>
                    <v-card-text>
                      <v-row align="center" class="mx-0">
                        <v-rating :value="4" color="amber" dense half-increments readonly size="25"></v-rating>
                        <div class="grey--text ms-4"> 4 (3423) </div>
                      </v-row>
                      <div class="my-4 text-subtitle-1"><h2>US $11.99</h2></div>
                      <div>Size and weight<br>band lenght: 25cm<br>Dial diameter: 35mm<br>Dial thickness:22mm<br>Band width: 29mm</div>
                    </v-card-text>
                    <v-divider class="mx-4"></v-divider>
                    <v-card-actions>
                      <v-btn color="black" rounded class="white--text">Buy Now</v-btn>
                      <v-btn color="black" rounded class="white--text">Add to Cart</v-btn>
                    </v-card-actions>
                  </v-card>
                </v-col>       
        </v-row>
        
    </v-container>
</template>
<script>
    export default{
        name:"ProjectComponent"
    }
</script>
<style>
    h4.justify-center.theme--light {
    color: black;

}
</style>