<template>
    <div>
        <button type="button" class="btn btn-primary">Primary</button>
        <div>
            <v-row no-gutters>
                <v-col cols="9">
                    <v-card class="pa-2" outlined tile> .col-9 </v-card>
                </v-col>
                <v-col cols="3">
                    <v-card class="pa-2" outlined tile> .col-9 </v-card>
                </v-col>
            </v-row>
        </div>
    </div>
</template>

<script>
export default {
    name: "HomeVue",

    components: {},
};
</script>
