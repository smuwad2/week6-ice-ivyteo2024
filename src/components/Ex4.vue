<script>
    export default { 
        data() {
            return {
                // Add code here
                id:"demo1",
                isActive:true,
            }
        },
        methods: { 
   			// Add code here
            changeColor(){
                this.isActive = !this.isActive
                
            }
		}
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" class="m-2" v-bind:class="{'blueBox':isActive,'redBox':!isActive}">
            div ID : {{id}} 
        </div>
        
        <button type="button"  @click="changeColor()" v-bind:class="{'btn btn-primary':isActive,'btn btn-danger':!isActive}" >Change Color</button>

    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
