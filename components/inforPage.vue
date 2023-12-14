<template>

<div class="modal">
        <div class="header">
            <v-icon icon="mdi-home"  style="color: #fff; font-size: 3rem;" @click="gotoHome">
                
                </v-icon>

        </div>
        <div class="modal__body">
            <p>﻿

                Although the pattern and issue of transition from school to work (TSW) is commonly discussed in France,
                Germany, Japan, the Netherlands, Sweden, the UK, and the US, it cannot find a place as a topic of
                discussion in the press and academe in Turkey. In reality, transition from school to work constitutes
                one of the most critical steps in young people's careers. It is therefore necessary to discuss the power
                of public policies to improve policies for young people, such as the regulation of the labor market,
                labor market programs, the effect of education on having a profession, and transition from higher
                education to work, all of which are underlined in the literature. The aim of this chapter is to discuss
                the process of transition from higher education to work within the context of Turkey based on the
                literature.</p>
        </div>
        <footer>
            Infor
        </footer>
    </div>
</template>
<script>

export default{
    methods:{
        gotoHome() {
            console.log("home");
            setTimeout(() => {

                this.$router.push("/");
                setTimeout(() => {
                    console.log("exitPage")
                }, 2000);
            }, 15000

            );
        },
    }
}
</script>
<style scoped>
.modal{
    width: 30rem;
    height: auto;
    background-color: rgb(244, 22, 22);
   
    
    border-radius: 20px;
   margin: 0 auto;

}
.header{
  
  margin-top: 20px;
  margin-right: 20px;
  display: flex;
    justify-content: flex-end;
}
.modal__body{
    color: #fff;
    padding: 3rem;
    text-overflow: ellipsis;
}
footer{
    font-weight: bold;
    font-size: 5rem;
    color: #fff;
    text-align: center;
    padding-top: 4rem;
}
</style>