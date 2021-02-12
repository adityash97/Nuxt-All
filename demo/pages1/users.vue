<template>
    <div>
        <h1>It is same page output</h1>
         Enter Id : <input type="text" v-model="userId"/>
        <button @click="locadUsers"> Users </button>
        <nuxt-child/> <!-- It will be replaced by the child of users folder
                        i.e : suppose it will be replaced by all ouput of users folder(first index page will be rendered then according to output it will work)-->
    </div>
</template>

<script>
export default {
    data(){
        return{
            userId :  ""
        }
    },
    methods: {
        locadUsers(){
            this.$router.push('/users/'+this.userId)
        }
    },
    layout:"users"
}
</script>