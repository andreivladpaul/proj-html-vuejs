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

                    
                    <ul v-for="(link,index) in links" :key="index">
                        <li><h3>{{link.title}}</h3></li>
                        <li v-for="(collegamento,index) in link.link" :key="index"><i class="fas fa-chevron-right"></i> {{collegamento}} </li>
                        
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
                    <li  v-for="(link,index) in linksBottom" :key="index"><a href="">{{link.title}}</a></li>
                    
                    
                </ul>

            </div>

      </div>

  </footer>
</template>

<script>


export default {
  name: 'Footer',
  data() {
      return {
          "links": [
            {
                'title': 'Contact Us',
                'link': ['Privacy','Terms','Cookie Policy', 'Sitemap']
            },
            {
               'title': 'Support Us',
               'link': ['Privacy','Terms','Cookie Policy', 'Sitemap']
            },
            {
               'title': 'Explore',
               'link': ['Accomodation','Arts Academics','Central Services', 'Conferences and Events', 'Food and Drink']
            },
            {
               'title': 'Visit',
               'link': ['Admission','Contact Us','FAQs', 'Request Information', 'Privacy Notice']
            }
        
        ],
        
        "linksBottom": [
            {
                'title': 'Privacy',
            },
            {
               'title': 'Terms'
            },
            {
               'title': 'Cookie Policy'
            },
            {
               'title': 'Sitemap'
            }
        
        ]
        
    }
  }
  
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
                            cursor: pointer;
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

                            &:hover {
                                color: #fff;
                            }
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

                 h3 {
                color: #fff;
                }

                 ul {
                     max-width: 200px;
                     li {
                         margin-bottom: 20px;
                         cursor: pointer;
                         
                         &:hover {
                                color: #fff;
                            }
                     }
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
                        
                        &:hover {
                                color: #fff;
                            }
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