<template>
    <div>
        <div class="container mt-5">
            <div class="row">
                <div class="col-6">
                    <h1 class="mb-4">Register</h1>
                    <form @submit.prevent="register">
                        <div class="mb-3">
                            <label for="exampleInputName1" class="form-label"
                                >Name</label
                            >
                            <input
                                type="name"
                                class="form-control"
                                aria-describedby="nameHelp"
                                id="exampleInputName1"
                                v-model="name"
                            />
                        </div>
                        <div class="mb-3">
                            <label for="exampleInputPassword1" class="form-label"
                                >Password</label
                            >
                            <input
                                type="password"
                                class="form-control"
                                id="exampleInputPassword1"
                                v-model="password"
                            />
                        </div>
                        <div class="mb-3">
                            <label for="exampleInputGender1" class="form-label"
                                >Gender</label
                            >
                            <b-form-radio-group
                                v-model="selected"
                                :options="options"
                                :aria-describedby="ariaDescribedby"
                                name="radio-inline"
                                inline="true"
                            ></b-form-radio-group>
                        </div>
                        <div class="mb-3">
                            <label for="exampleInputAddress1" class="form-label"
                                >Address</label
                            >
                            <input
                                type="address"
                                class="form-control"
                                aria-describedby="addressHelp"
                                id="exampleInputAddress1"
                                v-model="address"
                            />
                        </div>
                        <button type="submit" class="btn nav-color" value="Login">Submit</button>
                    </form>
                </div>
            </div>
        </div>
        <HFooter />
    </div>
</template>

<script>
import HFooter from "vue-hacktiv8-footer";
export default {
    name: "Register",
    data(){
        return {
            name: "",
            password: "",
            options: [
                { text: 'Male', value: 'male' },
                { text: 'Female', value: 'female' }
            ],
            address: ""
        }
    },
    components: {
        HFooter
    }
}
</script>

<style>


</style>