<template>
 <div class="flex py-5">
    <!-- sidebar -->
    <div class=" sm:w-4/12 lg:w-3/12 xl:w-2/12 border border-gray-200 sidebar  pt-8 ">
      <div class="flex mr-3 ml-3 ">
        <figure class="logo-wrap w-2/12 ">
          <img class="logo" src="../assets/wslogo.jpeg" alt="">          
        </figure>
        <h1 class="w-9/12 text-2xl md:text-2xl font-black sidebar-title pl-1 pt-1 md:pt-2 xl:pt-1 logo-a">WhisperNote</h1>
      </div>
      <ul class="pt-5 ">
        <li class="">
          <a class="flex " href="">
            <div class="w-2/12 ">
              <i class="fa-solid fa-house md:text-xl home"></i>              
            </div>     
            <p class="w-9/12 md:text-xl">首頁</p>        
          </a>          
        </li>
        <li class="">
          <a class="flex" href="">
            <div class="w-2/12">
              <i class="fa-solid fa-calendar-days md:text-xl "></i>             
            </div>     
            <p class="w-9/12 md:text-xl">日記</p>        
          </a>          
        </li>
        <li class="">
          <a class="flex" href="">
            <div class="w-2/12">
              <i class="fa-solid fa-user md:text-xl"></i>             
            </div>     
            <p class="w-9/12 md:text-xl">角色</p>        
          </a>          
        </li>
        <li class="">
          <a class="flex" href="">
            <div class="w-2/12">
              <i class="fa-solid fa-users md:text-xl friends"></i>             
            </div>     
            <p class="w-9/12 md:text-xl ">朋友</p>        
          </a>          
        </li> 
        <li class="">
          <a class="flex" href="">
            <div class="w-2/12">
              <i class="fa-solid fa-file md:text-xl"></i>             
            </div>     
            <p class="w-9/12 md:text-xl">會員資料</p>        
          </a>          
        </li> 
        <li class="">
          <a class="flex" href="/signup">
            <div class="w-2/12">
              <i class="fa-solid fa-clipboard-check md:text-xl"></i>             
            </div>     
            <p class="w-9/12 md:text-xl">註冊</p>        
          </a>          
        </li> 
        <li class="">
          <a class="flex" href="">
            <div class="w-2/12">
              <i class="fa-solid fa-arrow-right-to-bracket md:text-xl login"></i>             
            </div>     
            <p class="w-9/12 md:text-xl">登入</p>        
          </a>          
        </li>              
       
      </ul>      
    </div>
    <!-- 右邊日記的部分 -->
    <div class="w-full sm:w-6/12 border border-gray-400">
      <div class="text-center flex justify-around  py-8 bg-gray-200  ">
        <h2 class="text-start text-2xl"> ＜ </h2>
        <h1 class="font-bold text-xl">6月 2022</h1>
        <h2 class="font-bold text-2xl"> ＞</h2>
        <div>
          <figure>
            <img src="" alt="">
          </figure>
        </div>
      </div>
      <div class="grid grid-flow-col text-center bg-gray-100 text-gray-400 border-t border-b border-gray-300 font-bold">
        <h3 class="w1/7">週日</h3>
        <h3 class="w1/7">週一</h3>
        <h3 class="w1/7">週二</h3>
        <h3 class="w1/7">週三</h3>
        <h3 class="w1/7">週四</h3>
        <h3 class="w1/7">週五</h3>
        <h3 class="w1/7">週六</h3>
      </div>
      <div class="grid grid-flow-col   ">
        <div class="w1/7 vc-day vc-weekday">1</div>
        <div class="w1/7 vc-day">2</div>
        <div class="w1/7 vc-day">3</div>
        <div class="w1/7 vc-day">4</div>
        <div class="w1/7 vc-day">5</div>
        <div class="w1/7 vc-day ">6</div>
        <div class="w1/7 vc-day vc-weekday">7</div>
      </div>
    </div>
  </div>
</template>

<style>
.sidebar{
height: 80vh;
border-radius: 10px 0px 0px 10px;
}
.sidebar-title{
  font-family: 'Prompt', sans-serif;
}
.sidebar ul li a{
  font-weight: 600;
  padding: 10px 15px 10px 15px;
  font-size: 1rem;
  color:rgb(109, 108, 108);
  margin-left: 12px;
  margin-right: 12px;
  border-radius: 10px;
}
.sidebar ul li a:hover{
  color: antiquewhite;
  background-color: rgb(246, 246, 246);
  color: black;
}
.logo-wrap{
  width: 50px;        
    }
.logo{
  width: 100%;
  }
/* svg位子微調 */
.home{
  position: relative;
  right:2px;
}
.friends{
  position: relative;
  right:4px;
}
.login{
  position: relative;
  right:4px;
}
/* 日記區 */
.vc-day {
  padding: 0 5px 3px 5px;
  border-right: 1px solid rgb(175, 175, 175);
  height: 80px;
  text-align: left; 
  background-color: white;
}
.vc-weekday{
  background-color: #eff8ff;
}


@media screen and (max-width:640px) {
    .sidebar {
        display: none;
    }
}
</style>