<template>
    <div id="app">
        <body>
            <section>
                <div class="categories-title">
                    <span >NOSSAS DELÍCIAS</span>
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
    padding: 25px;
    background-color: white;
}

.categories-title{
    text-align: center;
    color: #810947;
    font-size: 30px;
    font-weight: 600;
}

</style>
