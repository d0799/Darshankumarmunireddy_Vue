<template>
    <div class="laptop-details">
      <h2 class="title">{{ Laptops.Brand }}</h2>
      <div class="details">

        <div class="detail">
          <h3 class="label">Price</h3>
          <p class="value">{{ Laptops.Price }}</p>
        </div>

        <div class="detail">
          <h3 class="label">Storage</h3>
          <p class="value">{{ Laptops.Storage}}</p>
        </div>

        <div class="detail">
          <h3 class="label">Display</h3>
          <p class="value">{{ Laptops.Display }}</p>
        </div>

        <div class="detail">
          <h3 class="label">Processor</h3>
          <p class="value">{{ Laptops.Processor}}</p>
        </div>

        <div class="detail">
          <h3 class="label">Color</h3>
          <p class="value">{{ Laptops.Color }}</p>
        </div>

        <div class="detail">
          <h3 class="label">Battery life</h3>
          <p class="value">{{Laptops.Battery_life }}</p>
        </div>

      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SingleLaptop',
    props: {
      Laptops: Array
    }
  }
  </script>
  
  <style scoped>
  .laptop-details {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;
  padding: 20px;
  background-color: rgb(21, 198, 229);
  border-radius: 5px;
}

.title {
  font-size: 32px;
  margin-bottom: 16px;
}

.details {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  width: 100%;
}

.detail {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 16px;
}

.label {
  font-size: 16px;
  margin-bottom: 8px;
}

.value {
  font-size: 24px;
  font-weight: bold;
}

  </style>
  