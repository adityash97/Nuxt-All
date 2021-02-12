<template>
    <div>
        <baseUrls/>
        <h1>This is a users page</h1>
        Enter user id: <input type="text" v-model="userId"/>
        <button @click="gotoUser">Goto user</button>
    </div>
</template>


<script>
import baseUrls from '~/components/baseUrls.vue'
export default {
    data(){
        return{
            userId : ""
        }
    },
    components:{
        baseUrls
    },
    methods:{
        gotoUser(){
            this.$router.push('/users/'+this.userId)
        }
    }

}
</script>