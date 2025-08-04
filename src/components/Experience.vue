<script setup>
// const items = ref([{ message: 'Foo' }, { message: 'Bar' }])
</script>
<template>
  <div class="page-wrapper">
    <h1>Experience</h1>
    <p>Here is a quick summary of my most recent experiences:</p>
    <li v-for="item in items">
      {{ item.message }}
    </li>
    <div class="experience-cards">
      <ul>
        <li v-for="experience in experiences">
          {{ experience.message }}
          <div class="card">
            <div class="content">
              <div class="logo">Placeholder logo</div>
              <contet> {{ experience.message }}</contet>
              <dates>Dates for the placholder etc</dates>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.page-wrapper{
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  place-items: center;
}

.card{
  width: 60%;
  min-width: 424px;
  min-height: 224px;
  box-shadow: inset 2px 2px 5px #555;
  border-radius: 28px;
  display: flex;
  place-items: center;
  justify-content: center;
}
.content{
  height: 200px;
  width: 400px;
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  border: 1px solid #000;
  box-shadow: -1px -1px 5px #555;
  padding: 6px;
  border-radius: 16px;
}
</style>