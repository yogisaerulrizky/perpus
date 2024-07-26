
<template>
    <div class="row p-3 bg-primary text-while">
      <div class="col-lg-1">
        <img src="~/assets/img/Logo-SMK4.png" alt="logo SMKN4">
        </div>

      <div class="col-lg-11">
        <h1>Perpus digital</h1>
        <address>
          SMKN 4 Tasikmalaya
          Jl ,depok, sukamenak, Purbaratu
        </address>
       </div> 
    </div>
      
  
  <style>
  .header {
    display: flex;
    align-items: center;
    background-color: #0004ff;
    color: #ffffff;
   width: 100%;
  }
  
  .h-img > img {
    width: 115px;
    height: 135px;
    margin-left: 30px;
  }
  
  .teks-judul {
    margin-left: 20px;
  }
  @media (max-width: 750px) {
    .header {
      flex-direction: column;
      align-items: flex-start;
      text-align: center;
    }
  
    .h-img > img {
      width: 100px;
      height: 100px;
      margin-left: 0;
      margin-bottom: 10px;
    }
  
    .t-judul {
      margin-left: 0;
    }
  
    h1 {
      font-size: 1.5em;
    }
  }
  </style>
  