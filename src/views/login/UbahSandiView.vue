<template>
    <v-row no-gutters class="h-full">
        <v-col cols="4" class="bg-img-primary">
            <LoginSide />
        </v-col>
        <v-col cols="8">
            <v-row no-gutters class="h-full text-center">
                <v-col align-self="center">
                    <div class="container-login-form">
                        <h1>{{ textData.ubahSandi }}</h1>
                        <span class="body2">{{
                            textData.silahkanUbahKataSandi
                        }}</span>
                        <form class="d-grid gap-med mb-2 textleft">
                            <div class="w-full input-icon">
                                <label for="Label">{{
                                    textData.sandiSementara
                                }}</label>
                                <input class="form-control" type="password" />
                                <span class="suffix">
                                    <i id="hide1" class="fa-solid fa-eye"></i>
                                    <i
                                        id="hide2"
                                        class="fa-solid fa-eye-slash"></i>
                                </span>
                            </div>
                            <div class="w-full input-icon">
                                <label for="Label">{{
                                    textData.sandiBaru
                                }}</label>
                                <input class="form-control" type="password" />
                                <span class="suffix">
                                    <i id="hide1" class="fa-solid fa-eye"></i>
                                    <i
                                        id="hide2"
                                        class="fa-solid fa-eye-slash"></i>
                                </span>
                            </div>
                            <div class="w-full input-icon">
                                <label for="Label">{{
                                    textData.ulangiSandi
                                }}</label>
                                <input class="form-control" type="password" />
                                <span class="suffix">
                                    <i id="hide1" class="fa-solid fa-eye"></i>
                                    <i
                                        id="hide2"
                                        class="fa-solid fa-eye-slash"></i>
                                </span>
                            </div>
                        </form>

                        <div class="d-grid gap">
                            <button type="button" class="btn btn-primary">
                                {{ textData.simpan }}
                            </button>
                            <span class="a">{{
                                textData.kembaliKehalamanLogin
                            }}</span>
                        </div>
                    </div>
                </v-col>
            </v-row>
        </v-col>
    </v-row>
</template>

<script>
import LoginSide from "@/components/LoginSidebar.vue";
export default {
    name: "LoginView",
    components: { LoginSide },
    data() {
        return {
            textData: {
                ubahSandi: "Ubah kata sandi",
                silahkanUbahKataSandi:
                    "Silakan ubah kata sandi Anda demi keamanan data",
                sandiSementara: "Kata sandi Sementara",
                sandiBaru: "Kata sandi Baru",
                ulangiSandi: "Ulangi Kata sandi",
                simpan: "Simpan",
                kembaliKehalamanLogin: "Kembali ke halaman login",
            },
        };
    },
};
</script>

<style scoped>
.h-full {
    height: 100vh;
}
.bg-img-primary {
    background-image: url("../../assets/images/bg-login.png");
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
