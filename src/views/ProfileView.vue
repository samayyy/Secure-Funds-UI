<template>
    <div>
        <v-card-actions class="clr">
            <v-col>
                <router-link style="text-decoration: none; color: inherit" to="/">
                    <v-btn text>Secure Patrons</v-btn></router-link>
            </v-col>
            <v-col class="text-right">
                <router-link style="text-decoration: none; color: inherit" to="/crowdfunding">
                    <v-btn class="mx-1">Crowdfunding</v-btn></router-link>
            </v-col>
        </v-card-actions>

        <v-container class="fill-height" fluid style="height: 1050px">

            <v-row justify="center">
                <v-col cols="12" sm="10">

                    <v-card class="mx-auto" light max-height="1250" max-width="1000">
                        <div id="loginF" style="color:white;font-weight:bold;">
                            Create Account
                        </div>

                        <v-img height="310"
                            src="https://storage.googleapis.com/proudcity/deleontx/uploads/2016/12/preview-wattpad-cover-maker-thumbnail.jpg">
                            <v-col md="20" offset-md="1">
                                <v-avatar class="profile" color="grey" size="200" margin-top="50px">
                                    <v-img src="https://cdn.vuetifyjs.com/images/profiles/marcus.jpg"></v-img>
                                </v-avatar>
                                <v-list-item color="rgba(100, 0, 50, .4)" dark>
                                    <v-list-item-content>
                                        <v-list-item-title class="title">
                                            <h1> Marcus Obrien </h1>
                                        </v-list-item-title>
                                        <v-list-item-subtitle>
                                            <h2> Australia</h2>
                                        </v-list-item-subtitle>
                                    </v-list-item-content>
                                </v-list-item>
                            </v-col>
                        </v-img>
                        <v-divider class="mx-4" vertical></v-divider>

                        <v-form ref="form" v-model="valid" lazy-validation>
                            <v-col md="10" offset-md="1">
                                <v-text-field value="Marcus Obrien" label="Full Name" readonly></v-text-field>
                                <v-text-field value="1998-11-28" label="Date of Birth" readonly></v-text-field>
                                <v-text-field value="Marcus.O@gmail.com" label="email" readonly></v-text-field>
                                <v-text-field value="077420018" label="Telephone No" readonly></v-text-field>
                                <v-text-field value="Australia" label="Country" readonly></v-text-field>
                                <v-text-field value="442011" label="ZIP code" readonly></v-text-field>
                                <v-text-field value="160/2,1st Lane, Australia." label="Address"
                                    readonly></v-text-field>
                            </v-col>
                            <v-divider class="mx-4" vertical></v-divider>

                            <v-col md="8" offset-md="4">
                                <v-btn color="primary" class="mr-4" @click="validate" router-link to="/Editpro">
                                    Edit Profile
                                </v-btn>
                                <v-btn color="warning" class="mr-4" @click="validate" router-link to="/TimeL">
                                    Timeline
                                </v-btn>
                            </v-col>
                        </v-form>
                        <v-progress-linear color="cyan darken-2" rounded value="100"></v-progress-linear>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>


    </div>
</template>

<script></script>