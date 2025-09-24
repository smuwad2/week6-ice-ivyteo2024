<script>
    export default { 

       // add code here 
       data(){
        return{
            loginType:"username",

        }
       }

    }
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="loginType"><!--bind it to the logintype so when user select diff one it will update to it-->
        <option value="username" selected>Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div v-if="loginType === 'username'">
        <label>Username</label>
        <input placeholder="Enter your username">
    </div>
    <div v-else>
        <label>email</label>
        <input placeholder="Enter your email">
    </div>
</template>

