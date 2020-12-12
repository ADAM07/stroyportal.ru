<template>
  <div id="app">
<header class="page-header">

  <nav class="main-nav">

     <div class="main-nav-region">
        <ul>
          <li><img alt="region" src="./assets/region.svg"><a href="#">Волгоградская область</a></li>
        </ul>
     </div>
    <div class="main-nav-list">
      <ul>
        <li><a href="#">Тендеры</a></li>
        <li><a href="#">Базы подрядчиков</a></li>
        <li><a href="#">Другие сервисы<img alt="Vue logo" src="./assets/vectorchevron.svg"></a></li>
      </ul>
    </div>
  </nav>
<div class="header-search">
  <div class="header-search-logo">
    <img alt="logo header" src="./assets/logo.png">
  </div>
  <div class="header-btn-katalog">
    <button>Каталог</button>
  </div>
  <div class="header-search-input">
    <input type="search" autocomplete="on" placeholder="Хочу найти...">
  </div>
  <div class="header-btn-spisok">
    <button></button>
  </div>
  <div class="header-search-avatar">
    <a href="#"><img alt="logo avatar" src="./assets/avatar.png"></a>
  </div>
</div>
</header>
  </div>
</template>



<style lang="scss">

$color:#708598;
$border:1px solid #ECEFF1;

#app {
  font-family: Open Sans, sans-serif;

  padding: 0;
  color: $color;
  max-width: 1280px;
 margin: 0 auto;
}


.main-nav{
  background-color:#FAFBFC;
  display: flex;
  justify-content: space-between;
  font-size: 12px;
  border-bottom: $border;
}

.main-nav-list ul{
  display: flex;

}



.main-nav-region{
  margin-left: 65px;
  height: 20px;
}

.main-nav-region ul li,
.main-nav-list ul li{
  list-style: none;
  margin-right: 24px;

}

.main-nav-region ul li a,
.main-nav-list ul li a{
  text-decoration: none;
  color: $color;
}
.main-nav-list ul li img{
  margin-left:6px ;
}

.main-nav-region ul li img{

  margin-right:8px ;
}

.header-search{
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 76px;
   border-bottom: $border;
  margin: 0;
  padding:0 ;
}

.header-search-logo{
  margin-left:85px ;
  width: 221px;
}

.header-btn-katalog button{
  font-size: 14px;
  font-weight:600;
  padding-left: 40px;
  border:none;
  background-color:#FED83D;
  width: 116px;
  height:40px;
  border-radius: 4px;
  background-image: url("./assets/katalog.svg");
  background-repeat: no-repeat;
  background-position: 20px;
}

.header-search-input input{
  width:526px;
  height:40px;
  border: 1px solid #ECEFF1;
  border-radius: 4px;
  background: url("./assets/search.svg") no-repeat 490px;

}

.header-search-input input::placeholder{
  color:#708598;
  font-size: 14px;
  font-weight: 400;
  padding-left: 14px;

}

.header-btn-spisok button{
  border:1px solid #ECEFF1;
  background-color:#FAFBFC;
  width: 111px;
  height:40px;
  border-radius: 4px;
  background: url("./assets/spisok.svg") no-repeat center;
}

</style>

<script>


export default {
  name: 'App',
  components: {

  }
}
</script>