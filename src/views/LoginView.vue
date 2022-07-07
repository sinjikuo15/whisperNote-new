<template>
    <div class="flex justify-center py-8">
        <div class="flex w-11/12 border border-gray-100 rounded-lg justify-center ">
            <div class="flex justify-center w-full sm:w-8/12 md:w-6/12  text-center py-5">
                <div class="w-11/12 md:w-10/12 lg:w-8/12">
                    <figure class=" logo-wrap justify-center logo-center py-5">
                        <img  class="logo" src="../assets/wslogo.jpeg" alt="">
                    </figure>
                    <h1 class="font-black text-2xl md:text-3xl title ">登入您的帳號</h1>
                    <div class="flex justify-center pt-2">
                        <p class="sm:text-sm">或 &nbsp;</p>                     
                        <p class="font-bold text-indigo-500 sm:text-sm"> 開始您的14天試用</p>
                    </div>
                    <p class="pt-5 font-bold text-gray-700">快速登入</p>
                    <!-- 三個按鈕區 -->
                    <div class=" pb-5  flex justify-center sm:justify-between ">
                        <a class="sign-btn " href="">
                            <i class="fa-brands fa-facebook "></i> 
                        </a>                                             
                        <a class="sign-btn" href="">
                            <i class="fa-brands fa-twitter "></i>
                        </a>
                        <a class="sign-btn" href="">
                            <i class="fa-brands fa-line text-green-600"></i>
                        </a>
                    </div>
                    <!-- 分隔線 -->
                    <div class="flex justify-center">
                        <h1 class="w-11/12 sm:w-full  title-flex  ">或由信箱登入</h1>
                    </div>
                    <div class="flex justify-center">
                        <div class="w-11/12 sm:w-full">  
                            <h2 class="font-bold text-start text-gray-700 pt-4">信箱</h2>                    
                            <input class="w-full border border-gray-300 rounded-md  shadow focus:outline-blue-400 h-10" type="email">
                            <h2 class="font-bold text-start text-gray-700 pt-4">密碼</h2>                    
                            <input class="w-full  border border-gray-300 rounded-md  shadow focus:outline-blue-400 h-10" type="password">
                            <div class="flex sm:block md:flex justify-between py-4">
                                <div class="flex justify-center">
                                    <input type="checkbox" name="" id="">
                                    <p class="text-gray-700 font-bold"> 記住我</p>
                               </div>                               
                                <a href="">
                                    <p class="text-indigo-500 font-bold hover:underline">忘記您的密碼?</p>
                                </a>
                            </div>
                            <button class="w-full bg-indigo-500 hover:bg-indigo-400 text-gray-100 rounded-md font-bold p-2 mt-1 mb-1">登入</button>
                        </div>                        
                    </div>                 
                
                </div>                
            </div>
            <div class="md:w-6/12 house">
                
            </div>
        </div>        
    </div>
</template>


<style scoped>    
    .logo-wrap{
        width: 75px;
    }
    .logo{
        width: 100%;
    }
    .logo-center{
        margin:auto
    }
    .house{
        background-image: url(https://img01.sc115.com/uploads3/sc/jpgs/1912/hpic1808_sc115.com.jpg);
        background-repeat: no-repeat;
        background-position:center ;
        background-size:cover;
        border-radius: 0px 5px 5px 0px;
    }
    /* .title{
        font-family: 'Prompt', sans-serif;

    } */
    .sign-btn{
        width: 30%;       
    }
    .sign-btn :hover{
        transform: scale(1.3);
        transition: 0.5s;               
    }
    
    /* 分隔線 */
    .title-flex {
        display: flex;
        align-items: center;
        font-size: 1rem;
        color: gray;
        /* font-weight: bold; */
    }

    .title-flex::before,
    .title-flex::after {
        content: '';
        flex: 1;
        height: 0.5px;
        background: rgb(206, 206, 206);
    }

    .title-flex::before {
        margin-right: 0.6rem;
    }

    .title-flex::after {
        margin-left: 0.6rem;
    }
</style>
<script>
export default {
  name: "login",
};
</script>