<template>
    <v-row no-gutters class="h-full">
        <v-col cols="4" class="bg-img-primary">
            <LoginSide />
        </v-col>
        <v-col cols="8">
            <v-row no-gutters class="h-full text-center">
                <v-col align-self="center">
                    <div class="container-login-form">
                        <h1>{{ textData.masuk }}</h1>
                        <span class="body2">{{
                            textData.masukDenganAkun
                        }}</span>
                        <form class="d-grid gap-med mb-2 text-left">
                            <div class="w-full mb-2">
                                <label for="Label">{{ textData.nik }}</label>
                                <input
                                    class="form-control"
                                    type="text"
                                    autocomplete="off" />
                            </div>
                            <div class="w-full input-icon">
                                <label for="Label">{{ textData.sandi }}</label>
                                <input class="form-control" type="password" />
                                <span class="suffix">
                                    <i id="hide1" class="fa-solid fa-eye"></i>
                                    <i
                                        id="hide2"
                                        class="fa-solid fa-eye-slash"></i>
                                </span>
                            </div>
                            <div class="disgrid11">
                                <label class="checkbox"
                                    >{{ textData.ingatSaya }}
                                    <input type="checkbox" checked="checked" />
                                    <span class="checkmark"></span>
                                </label>
                                <span class="a textright">{{
                                    textData.lupaSandi
                                }}</span>
                            </div>
                        </form>

                        <div class="d-grid gap">
                            <button type="button" class="btn btn-primary">
                                {{ textData.masuk }}
                            </button>
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
                masuk: "Masuk",
                masukDenganAkun: "Silahkan masuk dengan akun yang terdaftar",
                nik: "NIK",
                sandi: "Kata Sandi",
                ingatSaya: "Ingat saya",
                lupaSandi: "Lupa Kata Sandi",
                sandiBerhasilDiubah:
                    "Kata sandi berhasil diubah. Silakan login kembali",
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
</style>
