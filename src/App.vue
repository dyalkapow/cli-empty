<template>
  <router-view/>
</template>

<style lang="scss">
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

$bg-color: rgba(10, 31, 42, 0.95);
$lime-green: #55af2a;


@font-face {
    font-family: 'Rubik';
    src: url('./assets/fonts/Rubik/Rubik-Regular.ttf') format('truetype'); 
    font-style: normal;
    font-weight: 400;
}

body {
    height: 100%;
    background: #eee;
    font-family: 'Rubik';
    background: $bg-color;
    color: #fff;
}

.auth {
   display: flex;
   flex-direction: column;
   align-items: center;
   width: 50%;
   margin: 20px auto;
   padding: 30px;
   transition: .5s ease;

   p {
      margin-top: 30px;
      transition: .5s ease;

      a {
         transition: .5s ease;
         line-height: 30px;
         border-bottom: 1px solid $lime-green;
         color: #fff;
         text-decoration: none;
         padding-left: 10px;
      }
   }

   &-btn {
      font-size: 13px;
      text-transform: capitalize;
   }

   &-type {
   margin-bottom: 30px;
   transition: .5s ease;
}
}

.input-value {
    padding: 10px;                              
    padding-left: 20px;
    border-radius: 10px;
    margin-bottom: 20px;
    outline: none;
    border: 1px solid #ccc;
    transition: .5s ease;
    
    &:focus {
        transition: .5s ease;
        box-shadow: 0 0 10px 3px #ccc;
    }

    &[type=number] {
        &::-webkit-outer-spin-button,
        &::-webkit-inner-spin-button {
            -webkit-appearance: none;
            margin: 0;
        }
    }
}

.submit-btn {
   color: #fff;
   background: #55AF2A;
   outline: none;
   border: 1px solid transparent;
   padding: 10px;
   transition: .5s ease;
   border-radius: 15px;
   letter-spacing: 2px;
   grid-column-start: 3;
   grid-column-end: 5;
   font-size: 16px;
   text-transform: uppercase;
   font-weight: 700;
   cursor: pointer;
   
   &:hover {
       text-shadow: 0 0 10px #fff;
       border: 1px solid #fff;
       transition: .5s ease;
   }
}
</style>
