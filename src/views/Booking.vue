<template>
    <v-container class="container d-flex flex-column justify-space-around align-center" >
        
        <div class="header">
            <h1>Welcome to Booking</h1>
        </div>
        <v-row>
            <v-col>
                <v-card
                    elevation="2"
                >  
                    <v-card-title>
                        New Patient
                    </v-card-title>
                    <v-card-text>
                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quia, cumque.
                    </v-card-text>
                    <v-card-actions>
                        <v-btn
                        outlined
                        rounded
                        text
                        >
                        Start
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
            <v-col>
                <v-card 
                    color="#385F73"
                    dark
                >
                    <v-card-title>
                        Old Patient
                    </v-card-title>
                    <v-card-text>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, illo qui temporibus aliquam quae quod officia quibusdam maiores ipsam odio.
                    </v-card-text>
                    <v-card-actions>
                        <v-btn
                        outlined
                        rounded
                        text
                        >
                        Start
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>    
    </v-container>
</template>

<script>
export default {
    name:'Booking',
}
</script>

<style scoped>
    .container{
        background-color: burlywood;
        height: 100vh;
    }
</style>