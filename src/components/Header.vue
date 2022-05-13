<template>
    <nav class="nav">
        <img class="logo" src=".././assets/img/logo-tkambio.svg"/>
    </nav>
</template>


<script>

    export default{
         props:[]
        
    }

</script>


<style lang="scss" scoped>
    .nav{
        display:flex;
        height: 74px;
        background: linear-gradient(180deg, #02ADF1 -2.37%, #4562E6 124.84%, #4563E6 124.84%);
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        justify-content: center;
        
    
        .logo{
         width: 150px;
         height: auto;
    }
    
    };

    
</style>