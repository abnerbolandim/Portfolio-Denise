<template>
    <div id="app">
        <body>
            <section>
                <div class="about-title">
                    <span >SOBRE MIM</span>
                </div>


            </section>
        </body>
    </div>
</template>

<script>
export default {
  name: 'App',
  props: {
  }
}
</script>

<style scoped>
#app{
    font-family: Arial, sans-serif;
    justify-content: center;
    /* padding: 25px; */
    background-color: #e8dddd;
}

body{
    font-family: Arial, sans-serif;
    box-sizing: unset;
}

.shape-divider{
    width: 100%;
}

.about-title{
    letter-spacing: 0.5px;
    text-align: center;
    color: #810947;
    font-size: 30px;
    font-weight: 600;
    padding-top: 40px;
    padding-bottom: 15px;
}
</style>
