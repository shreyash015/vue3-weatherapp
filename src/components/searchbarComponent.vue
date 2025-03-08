<script setup></script>

<template>
  <div>
    <div class="search">
      <input
        style="font-size: 16px"
        type="text"
        class="searchTerm"
        placeholder="Enter the name of a city"
      />
      <button style="position: relative" type="submit" class="searchButton">
        <img
          style="
            height: auto;
            width: 20px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
          "
          src="../assets/magnifying-glass-solid.svg"
          alt=""
        />
      </button>
    </div>
  </div>
</template>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Open+Sans);

input {
  background-color: #263138;
}
.search {
  width: 100%;
  position: relative;
  display: flex;
}

.searchTerm {
  width: 100%;
  border: 3px solid #ced3dc;
  border-right: none;
  padding: 5px;
  height: 20px;
  border-radius: 5px 0 0 5px;
  outline: none;
  color: #9dbfaf;
}

.searchTerm:focus {
  color: #ced3dc;
}

.searchButton {
  width: 40px;
  height: 36px;
  border: 1px solid #ced3dc;
  background: #ced3dc;
  text-align: center;
  color: #fff;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
  font-size: 20px;
}

/*Resize the wrap to see the search bar change!*/
.wrap {
  width: 30%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
