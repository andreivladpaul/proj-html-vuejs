<template>
    <header>
        <!------ NAVBAR SECTION ------->
        <nav class="flex-jc">
          <div class="container">
              <div class="logo">
                  <img src="../assets/img/Logo.jpg" alt="">
              </div>
              
              <ul>
                  <li><a href="#">Home</a></li>
                  <li><a href="#">About</a></li>
                  <li><a href="#">Academics</a></li>
                  <li><a href="#">Courses</a></li>
                  <li><a href="#">News</a></li>
                  
              </ul>
          </div>
          
      </nav>
      <!------ BANNER ------>
      <div class="banner">
          <img src='../assets/img/02_Landing-Page.jpg' alt="">
          <div class="banner-text">
              <h2>Professional Development For Coaches And Leaders</h2>
              <button>Learn More</button>
          </div>
      </div>
    
    
    </header>
  
</template>

<script>
export default {
    name:'Header'
}
</script>

<style lang="scss" scoped>
@import '../styles/globals.scss';


header{
    width: 100%;
    height: 100%;

   

    nav {
        width: 100%;
        height: 70px;
        background-color: $white;
    
    

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
    
        }

        img {
            position: absolute;
            top: 0;
            width: 120px;
            z-index: 99;
        }

        ul {
            list-style: none;
            display: flex;
            float: inline-end;

            li {
                a {
                color: $text;
                font-weight: bold; 
                text-decoration: none; 
                font-size: 14px; 
                }

            }
            li:not(last-child){
                margin-right: 50px;
            }
        }

    }
    .banner {
        width: 100%;
        height: 100%;
        position: relative;
        
        img {
            width: 100%;
            height: 100%;
        }
        

        .banner-text {
            position: absolute;
            text-align: center;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: $text;
            font-family: $cursive;
            font-size: 40px;

            >h2 {
                font-weight: 100;
            }

            button {
                background-color: transparent;
                border: 1px solid $text;
                color: $text;
                padding: 10px  20px;
                cursor: pointer;
                font-family: $cursive;
            }
        }

    }

}



</style>