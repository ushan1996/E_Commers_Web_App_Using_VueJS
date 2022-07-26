<template>
     <v-container class="my-15">
        <v-row justify="center">
                <v-col lg="12" class="text-center">
                     <v-subheader class="text-h4 justify-center">Contact Us </v-subheader> 
                     <p>bnds sni dfiosdjf ndfso ondf osn n ofdmf cnsdnfs fdnf no fns dodso</p>
                </v-col>
                <v-col lg="6">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4770989.212121536!2d-77.90928876464929!3d40.705934010208175!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c24fa5d33f083b%3A0xc80b8f06e177fe62!2sNew%20York%2C%20NY%2C%20USA!5e0!3m2!1sen!2slk!4v1657568026604!5m2!1sen!2slk" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </v-col>
                <v-col lg="6">
                    <v-form ref="form">
    <v-text-field
      v-model="contactInfo.name"
      :counter="10"

      label="Name"
      required
    ></v-text-field>

    <v-text-field
      v-model="contactInfo.email"
      label="E-mail"
      required
    ></v-text-field>
    <v-textarea label="Message" v-model="contactInfo.message">

    </v-textarea>

   

  

    <v-btn

      color="success"
      class="mr-4"

    >
      Send
    </v-btn>

    
  </v-form>
                </v-col>
        </v-row>
    </v-container>
</template>
<script>
    export default{
        name:"ContactComponent",
        data(){
            return{
                contactInfo:{}
            }
        }
    }
</script>
<style>
    
</style>