<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input  type="text" class="search-bar" placeholder="search......">
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">Namakkal, IN</div>
          <div class="date">Friday 19 March 2020</div>
        </div>
        <div class="weather-box">
          <div class="temp">27ºC</div>
          <div class="weather">Wind</div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      api_key: 'c0825b617850cd56d1a28266246d727f'
    }
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0; 
  box-sizing: border-box;
}
body{
  font-family: 'montserrat' , sans-serif;
}
#app{
    background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}
main {
  min-height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.144), rgba(0, 0, 0, 0.603));
}
.search-box{
  width: 100%;
  margin-bottom: 30px;
}
.search-box .search-bar{
  display: block;
  width: 100%;
  padding: 15px;
  color: #313131;
  font-size: 1.2em;
  appearance: none;
  outline: none;
  border: none;
  background: none;
  background-color: rgba(255, 255, 255, 0.788);
  border-radius: 0px 32px 0 32px;
  transition: 0.8s ease;
}
.search-box .search-bar:focus{
  background-color: rgba(255,255,255,0.75);
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
  border-radius: 32px 0 32px 0;
  transition: 0.8s ease;
}
.location-box .location{
  color: #fff;
  font-size: 2rem;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0,0,0,0.25);
}
.location-box .date{
  color: #fff;
  font-size: 25px;
  font-weight: 300;
  font-style: italic;
  text-align: center;
  text-shadow: 1px 3px rgba(51, 92, 228, 0.25);
}
.weather-box {
  text-align: center;
}
.weather-box .temp{
  display: inline-block;
  padding: 10px 25px;
  color: #fff;
  font-size: 102px;
  font-weight: 900;
  text-shadow: 3px 6px rgba(0, 0, 0, 0.26);
  background-color: rgba(255, 255, 255, 0.26);
  border-radius: 16px;
  margin: 30px 0px;
  box-shadow:3px 6px rgba(0, 0, 0, 0.253);
}
.weather-box .weather{
  color: #fff;
  font-style: italic;
  font-weight: 700;
  font-size: 48px;
  text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}
</style>
