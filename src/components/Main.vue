<template>
  <main class="flex-jc">

    <div class="container">
          <h2 id="intro">Since 200, weve been partnering with education leaders to <b class="bold">increase equity and achievement</b> for all students.</h2>

        <!-------- SERVICES OFFERED -------->
        <div class="cards mb-30">
            <div class="card">
                <img  src="../assets/svg/svg-0.svg" alt="">
                <h3>Online Coaching</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit 
                </p>
            </div>

            <div class="card">
                <img src="../assets/svg/svg-1.svg" alt="">
                <h3>Consultation</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit</p>
            </div>

            <div class="card">
                <img class="mb-30" src="../assets/svg/svg-2.svg" alt="">
                <h3>Life Programs</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit</p>
            </div>
        </div>
        <!-------- OBJECTIVES OBTAINED -------->
        <div class="cards-color mb-30">
          <div class="card-color" id="first">
              <span>6000</span>
              <span><i class="fas fa-plus"></i></span> 
              Students
            
          </div>
          <div class="card-color" id="second">
            <span>200</span>
            <span><i class="fas fa-plus"></i></span>
            Online Courses
            
          </div>
          <div class="card-color" id="third">
            <span>100</span>
            <span><i class="fas fa-percentage"></i></span>
            Happy Clients
            
          </div>
          
        </div>

        <!-------- RECENT COURSES -------->
        <h3>Recent Courses</h3>
        <p>Wheter you're considering a foundation course ora an undergraduated degree master's <br> or a PhD, academics is a place where students thrive.</p>

        <div class="cards mb-30">
            <!------- COURSE 1------>
            <div class="course-card">
                <div class="course-img">
                    <img  src="../assets/img/drawing.jpg" alt="">
                </div>
                

                <div class="card course">
                    <h3>UI Animation using Sketch 3, Principle App and Flinto</h3>
                    <p>This online photography course will teach you how to take amazing images and even sell... 
                    </p>
                    <p class="course-creator">Course by: University</p>
                </div>
            </div>
            <!------- COURSE 2------>
            <div class="course-card">
                <div class="course-img">
                    <img src="../assets/img/course-1-2.jpg" alt=""> 
                </div>
                

                <div class="card course">
                    <h3>The Ultimate Drawing Course - Beginner to Advanced</h3>
                    <p>This online photography course will teach you how to take amazing images and even sell...</p>
                    <p  class="course-creator">Course by: University</p>
                </div>
            </div>
            <!------- COURSE 3------>
            <div class="course-card">
                <div class="course-img">
                    <img src="../assets/img/pictures.jpg" alt="">
                </div>
                

                <div class="card course">
                    <h3>Your Complete Guido to Photography</h3>
                    <p>This online photography course will teach you how to take amazing images and even sell...</p>
                    <p  class="course-creator">Course by: University</p>
                </div>
            </div>
      </div>
    </div>
    
  </main>
</template>

<script>
export default {
  name: 'Main',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../styles/globals.scss';

main {
    text-align: center;
    
}
.container {
    
    flex-direction: column;
    justify-content: center;
    align-items: center;

    #intro {
        font-size: 30px;
        font-weight: 500 ;
        margin: 40px;
    }
    
    .bold {
            color: $main-c;
            font-weight: bold;
        }
    .cards {
        width: 100%;
        display: flex;
        justify-content: space-around;

        .card, .course-card {
            max-width: 350px;
            box-shadow: 11px -2px 52px -23px rgba(0, 0, 0, 0.281);
            -webkit-box-shadow: 11px -2px 52px -23px rgba(0, 0, 0, 0.342);
            -moz-box-shadow: 11px -2px 52px -23px rgba(0, 0, 0, 0.425);
               
            }

            .card {
                padding: 50px 30px;
                

                img{
                width: 80px;
                margin-bottom: 30px;
                }


            &.course {
                align-items: flex-start;
                box-shadow: none;


                > .course-img {
                    width: 100%;
                    height: 100%;

                    img {
                        width: 100px;
                        height: 100px;
                    }
                    
                }
            }
            &.course p, &.course h3 {
                text-align: start;
            }

            .course-creator {
                color: $main-c;
                font-size: 14px;
            }

        }
        .card:nth-last-of-type(){
            margin-right: 20px;
        }

    }

    .cards-color {
        width: 100%;
        display: flex;
        justify-content: space-around;
        .card-color {
            width: 400px;
            padding: 30px 0;
            margin-left: 100px;
            display: flex;
            align-items: center;
            background-repeat: no-repeat;
            background-position: left;
            text-align: start;
            font-size: 25px;

            &#first{
                background-image: url('../assets/img/counter-shape-1-1-1.png');
        
                > span {
                  color: $student-c;
                }

            }
            &#second{
                background-image: url('../assets/img/counter-shape-2-1-1.png');
                
                > span {
                  color: $main-c;
                }
            }
            &#third{
                background-image: url('../assets/img/counter-shape-3-1-1.png');
                
                > span {
                  color: $happy-c;
                }
            }

            > span {
                font-size: 40px;
                font-weight: bold;
                margin-right: 10px;
            }
        }
    }

    .course-card {
        .course-img {
            width: 100%;
            height: 200px;
            

            img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
        }
        
    }
        
}

</style>
