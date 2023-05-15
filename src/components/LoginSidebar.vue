<template>
    <v-row no-gutters class="h-full text-center">
        <v-col align-self="center">
            <img
                src="../assets/images/image-login.png"
                alt="Bg Login"
                width="414" />
        </v-col>
    </v-row>
</template>

<script>
export default {
    name: "LoginSidebar",
};
</script>

<style>
.h-full {
    height: 100vh;
}
.bg-img-primary {
    background-image: url("../assets/images/bg-login.png");
    background-repeat: no-repeat;
    background-size: cover;
}
.container-login-form {
    width: 60%;
    margin: 0 auto;
}
.disgrid {
    display: grid;
    align-items: center;
    grid-template-columns: 1fr 2fr;
}
.disflex {
    display: flex;
    align-items: center;
}
.textleft {
    text-align: left;
}
.disgrid11 {
    display: grid;
    grid-template-columns: 1fr 1fr;
}
.textright {
    text-align: right;
}
</style>
