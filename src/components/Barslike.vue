<template>
  <div class="container-fluid barikonica">
   <div class="row">
    <div class="col-sm h5" align="center">
      <a href="/psi" class="ikonica"><font-awesome-icon :icon="['fas', 'dog']" class="ikonica" /></a>
    </div>
    <div class="col-sm h5" align="center">
      <a href="/macke" class="ikonica"><font-awesome-icon :icon="['fas', 'cat']" class="ikonica" /></a>
    </div>
    <div class="col-sm h5" align="center">
      <a href="/malezivotinje" class="ikonica"><font-awesome-icon :icon="['fas', 'paw']" class="ikonica" /></a>
    </div>
    <div class="col-sm h5" align="center">
      <a href="/konji" class="ikonica"><font-awesome-icon :icon="['fas', 'horse']" class="ikonica" /></a>
    </div>
  </div>
  </div>
</template>
<style scoped>
.ikonica {
  color: white;
  height: 40px;
  opacity: 80%;
  transition: transform 1.2s;
  padding-top: 5px;
}
.ikonica:hover{
  transform: scale(120%);
  opacity: 100%;
}
.barikonica {
  background-color: rgb(78, 122, 158);
  width: 90%;
  border-radius: 20px;
}
.barikonica:hover{
  background-color: rgb(45, 118, 186);
}
</style>



