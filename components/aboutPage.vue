<template>
     <div class="modal">
        <header class="header">
            
            <a @click="gotoHome">Trang chủ</a>

          
           
            <v-icon icon="mdi-home"  style="color: #fff;"/>

        </header>
        <div class="modal__body">
            <span class="icon">
            <i class="mdi mdi-account" style="font-size: 10rem;"></i>
        </span>
        </div>
        <footer>
            <p>
                Although the pattern and issue of transition from school to work
                (TWS) is commonly disscused in France Germany , Japan , the Netherlands , Sweden
                , the UK , and the US , it cannot find a place
                as a topic of discussion in the press and academe in Turkey .In reality , transition from school to work
                constitutes one of the most
                critical steps in young people, such as the regutation of the labor market .
            </p>
        </footer>
    </div>
</template>
<script>




export default{
    
  methods:{
    gotoHome(){
        this.$router.push("/");
    }
  }
}

</script>
<style scoped>
html{
    
    font-family: 'Roboto', sans-serif;
    font-size: 62.5%;
}
.modal{
    width: 25rem;
    height: 30rem;
    background-color: aqua;
    margin: 0 auto;
    border-radius: 8px;
    margin-top: 1rem;
    
   
}
.header{
    font-weight: bold;
    font-size: 2rem;
    display: flex;
    justify-content: space-between;
    
}
.modal__body{
   margin: 2rem auto;
    
    width: 20rem;
    height: 20rem;
    background-color: white;
  
    border-radius: 1rem;
    position: relative;

    
}
.icon{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
   
}
p{
    font-weight: bold;
    font-size: 1rem;
    padding-left: 2rem;
}
</style>