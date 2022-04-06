<template>

  <main>
    <div class="container-90w">
    --- CONTENT GOES HERE ---
    </div>
  </main>

</template>

<script>
export default {
    name: 'MainComponent',
}
</script>

<style lang="scss" scoped>

main{
  background-color: black;
  color: white;
  padding: 5rem 0rem;

  .container-90w{
        display: flex;
        justify-content: space-between;
        align-items: center;
      }
}

</style>