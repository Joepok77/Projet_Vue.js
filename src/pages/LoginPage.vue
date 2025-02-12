<template>
    <main class="loginmain">
        <h1>LoginPage</h1>
        <form v-on:submit.prevent="submitHandler">
            <section>
            <article>
                <label for="email"></label>
                <input 
                v-model="data.email"
                id="email"
                type="email"
                placeholder="entrez votre email"
                class="input"
                />
            </article>
            <article>
                <label for="password"></label>
                <input
                v-model="data.password"
                id="password"
                type="password"
                placeholder="entrez votre mot de passe"
                class="input"
                />
            </article>
        </section>
        <section>
            <button
            type="submit"
            class="button is-primary"
            >Valider</button>
            <button
            type="reset"
            class="button is-danger"
            >réinitialiser</button>
        </section>

        </form>
    </main>
</template>
<script lang="ts" setup>
import {watch, reactive } from "vue"

const data = reactive({
    email: "",
    password: ""
})

watch(data, (val) => {
    console.log('Changement dans la variable data')
})


const isUserInputValid = (input:string): boolean => {

    const pattern = new RegExp()

}

const submitHandler = () => {

}

const inputHandler = function (){

}

</script>
<style lang="scss" scoped>
.loginmain {

}
</style>
