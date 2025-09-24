<script>
    export default { 
        data() {
            return {
                width: '200',
                height: '200',
                myImg: '/assets/me.png'
            }
        },
    }
</script>

<template>

    <!-- add code here -->
     <!--! is a shorthand notation for v-bind -->
     <img v-bind:src="myImg" v-bind:width="width" v-bind:height="height"></img>
</template>
