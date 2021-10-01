<template>
  <footer>
      <div class="footer-top">
            <div class="container">
                <div class="mail ">
                    <div class="input">
                        <input type="mail">
                        <button>submit</button>
                    </div>

                    <div class="insight">
                        <p>
                            <a href="#" id="underline">Insights is Pickwik</a> University's thought leadership publication for sharing knowlegde on management, technology and innovation.
                        </p>
                        <p><a href="">Take me there <i class="fas fa-chevron-right"></i></a></p>
                    </div>

                    <div class="footer-line"></div>



                </div>
                <div class="contacts">
                    <!-- CONTACT US -->
                    <ul>
                        <li><h3>Contact Us</h3>
                        </li>
                        <li><i class="fas fa-map-marker-alt"></i> 900 Wood Street, MI New York 48607
                        </li>
                        <li><i class="fas fa-phone-square-alt"></i> +56 345 678 000-09
                        </li>
                        <li><i class="fas fa-envelope"></i> info@example.com
                        </li>
                    </ul>

                    <!-- CONTACT US -->
                    <ul>
                        <li><h3>Support Us</h3>
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Privacy
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Terms
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Cookie Policy
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Sitemap
                        </li>
                    </ul>

                    <!-- CONTACT US -->
                    <ul>
                        <li><h3>Explore</h3>
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Accomodation
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Arts Academics
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Central Services
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Conferences and Events
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Food andDrink
                        </li>
                    </ul>

                    <!-- CONTACT US -->
                    <ul>
                        <li><h3>Visit</h3>
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Admission
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Contact US
                        </li>
                        <li><i class="fas fa-chevron-right"></i> FAQs
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Request Information
                        </li>
                        <li><i class="fas fa-chevron-right"></i> Privacy Notice
                        </li>
                    </ul>
                    
                </div>

            </div>
      </div>

      <div class="footer-bottom">
            <div class="container">
                <p>
                    © Copyright 2020 tophive. All Rights Reserved.
                </p>

                <ul>
                    <li><a href="">Privacy</a></li>
                    <li><a href="">Terms</a></li>
                    <li><a href="">Cookie Policy</a></li>
                    <li><a href="">Sitemap</a></li>
                    
                </ul>

            </div>

      </div>

  </footer>
</template>

<script>


export default {
  name: 'Footer',
  
}
</script>


<style lang="scss" scoped>
@import '../styles/globals.scss';
    footer {
        color: $f-link-c;
        height: 700px;
        width: 100%;

        .container {
                display: flex;
                justify-content: space-between;
                align-items: center;
                font-size: 16px;
        }

        .footer-top {
            width: 100%;
            height: 90%;
            background-color: $f-bg-c;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            > .container {
                flex-direction: column;

                .mail {
                    width: 100%;
                    position: relative;
                    
                    display: flex;
                    justify-content: space-around;
                    align-items: center;
                    box-shadow: 3px 0px 49px -14px rgba(0,0,0,0.75);
                    -webkit-box-shadow: 3px 0px 49px -14px rgba(0,0,0,0.75);
                    -moz-box-shadow: 3px 0px 49px -14px rgba(0,0,0,0.75);
                    padding: 60px 60px;
                    margin-bottom: 70px;


                    .input {
                        input, button {padding: 20px;
                        border: none;}

                        button {
                            background-color: $main-c;
                            color: #fff;
                            
                        }
                    }

                    .insight {
                        width: 60%;
                        

                        > p {
                            margin: 0;
                            color: $f-link-c;
                        }
                        
                        
                        a {
                        color: $main-c;
                        }
                        #underline {
                            border-bottom: 1px solid #fff ;
                        }

                        .fa-chevron-right {
                            color: #fff;
                        }
                    }

                    .footer-line {
                        width: 5px;
                        height: 100px;
                        position: absolute;
                        top: 40px;
                        left: 0;
                        background-color: #23374b;

                    }

                   
                }   
            }
            

            

            .contacts {
                width: 100%;
                display: flex;
                justify-content: space-between;
            }
            
            h3 {
                color: #fff;
            }

            ul {
                max-width: 200px;
                li {
                    margin-bottom: 20px;
                    cursor: pointer;
                }
            }
            
        }

        .footer-bottom {
            width: 100%;
            height: 10%;
            background-color: $f-bg-b-c;
            display: flex;
            
            

            .container {
                
                
                > p {
                    color: $f-link-c;
                    margin: 0;
                }

                ul {
                display: flex;
                list-style: none;
                li {
                    a {
                        color: $f-link-c;
                    }
                }

                li:not(last-child) {
                    margin-right: 20px;
                }
            }

            
                
            
            }
        }

    }

</style>