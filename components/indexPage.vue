<template>
    <div class="indexPage">
        <div class="shape">
            <div class="shape--aqua">
                <a @click="gotoHome">Home</a>
            </div>
            <div class="shape--yellow">
                <a @click="gotoAbout">About</a>

            </div>
            <div class="circle">
                <a @click="gotoInfor">Infor </a>

            </div>
        </div>
        <div class="form">
            <input type="text" id="userName" name="fname" value="Name"><br>
            <input type="text" id="passWord" name="lname" value="Password"><br>
            <input type="submit" value="Submit">
        </div>
    </div>
</template>
<script>




export default {
    name: "index",
    methods: {
        gotoAbout() {
            console.log("about");
            setTimeout(() => {

                this.$router.push("/about");
                setTimeout(() => {
                    console.log("exitPage")
                }, 2000);
            }, 15000

            );
        },
        gotoInfor() {
            console.log("infor");
            setTimeout(() => {

                this.$router.push("/infor");
                setTimeout(() => {
                    console.log("exitPage")
                }, 2000);
            }, 15000

            );
        },

    },

  
}

</script>
<style scoped>
html {
    font-size: 62.5%;

}
a{
    cursor: pointer;
}
body {
    margin: 0;
    padding: 0;

}

:root {
    --dimension: 15rem
}

.indexPage {
    display: flex;
    flex: 1;
    flex-direction: column;
    align-items: center;

    margin-top: 1%;
}

.shape {
    margin-top: 0;
    position: relative;
    display: flex;
    margin-bottom: 7rem;
    position: relative;
    flex: 1;
}

.shape--aqua {
    width: 10rem;
    height: 10rem;
    background-color: aqua;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
}

.shape--yellow {
    width: 10rem;
    height: 10rem;
    background-color: yellow;
    transform: translate(-30%, 50%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    text-align: center;

}

.circle {
    width: 10rem;
    height: 10rem;
    background-color: red;
    border-radius: 50%;
    transform: translate(-60%);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    text-align: center;
}

.form {
    padding-top: 5rem;
    width: 40rem;
    height: auto;
    background-color: rgb(85, 240, 240);
    border-radius: 2rem;
    display: flex;
    flex-direction: column;
    align-items: center;


}

input {
    width: 80%;
    text-align: center;
    height: 2rem;
    margin-bottom: 1rem;
    border-radius: 2rem;
    font-weight: bold;
    border: 1px solid black;
    padding: 6px 0;

}

input[type="submit"] {
    width: 80%;
    height: 3rem;
    background-color: green;

}

a {
    text-decoration: none;
}
</style>