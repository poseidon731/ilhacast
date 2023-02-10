<template>
<div class="footer">
  <div class="container-flex">
    <div class="container-item">
      <p>Links úteis</p>
      <br>
      <ul>
        <li>Podcasts</li>
        <li>...</li>
        <li>Link 3</li>
      </ul>
    </div>
    <div class="container-item">
      <p>Quem somos</p>
      <br>
      <ul>
        <li>Link 1</li>
        <li>Link 2</li>
        <li>Link 3</li>
      </ul>
    </div>
    <div class="container-item">
      <p>Code</p>
      <br>
      <ul>
        <li>Link 1</li>
        <li>Link 2</li>
        <li>Link 3</li>
      </ul>
    </div>
  </div>

</div>


</template>

<style scoped>

ul {
  list-style: none;
}

.container-flex {
  
  padding-top: 80px;
  padding-left: 20px;
  padding-bottom: 80px;
  font-family: RobotoThin;
  flex: 1;
}

p {
  font-weight: bold;
}

.footer {
  color:rgba(255, 255, 255, 0.8);;
  background-color: rgba(0, 0, 0, .9);
  position: absolute;
  display: flex;
  align-content: center;
  align-items: center;
  justify-content: center;
  width: 100%;
}

</style>
