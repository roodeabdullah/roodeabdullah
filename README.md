<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="Style.css">
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE-edge">
        <meta name="viewport" content="width=device-width , initial-scale=1.0">
        <title>My Personal Web</title>
        <script src="https://kit.fontawesome.com/cfa6bcf5d6.js" crossorigin="anonymous"></script>
    </head>
    <body>
        <div id="header">
            <div class="container">
                <nav>
                    <img class="logo">
                <ul id="sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#About">About</a></li>
                    <li><a href="#CV">CV</a></li>
                    <li><a href="#intrested">My intrested</a></li>
                    <li><a href="#Contact">Contact</a></li>
                    <i class="fas fa-times" onclick="closemenu()"></i>
                </ul>
                <i class="fas fa-bars"onclick="openmenu()"></i>
                </nav>
                <div class="header-text">
                    <p>Hello, I'm </p>
                    <h1><span>Raghad Al-orf </span></h1>
                    <h6>Programmer</h6>
                </div>
            </div>
        </div>
        <!-- ------------------------ ABOUT PAGE ----------------- -->
        <div id="About">
            <div class="container">
                <!-- <div class="row"> -->
                    <div class="about-col-2">
                        <h1 class="title">About Me</h1>
                        <br><br><br><br>
                        <p>am a student at Imam Muhammad bin Saud Islamic University in the College of Business, specializing in business administration, track of management information systems</p>
                        <div class="tab-title">
                            <p class="tab-link actv-link" onclick="opentab('skills')">Skills</p>
                            <p class="tab-link" onclick="opentab('experince')">Experince</p>
                            <p class="tab-link" onclick="opentab('education')">Education</p>
                        </div>
                        <div class="tab-des actv-tab" id="skills">
                            <ul>
                                 <li><span>First</span><br>Oracle sql</li>
                                 <li><span>second</span><br>Microsoft access</li>
                                 <li><span>third</span><br>Microsoft excel</li>
                                 <li><span>Fourth</span><br>Data analysis</li>
                            </ul>
                        </div>
                        <div class="tab-des" id="experince">
                            <ul>
                                 <li><span>Job:</span><br>Vendor</li>
                                 <li><span>Company:</span><br>Plumbing and electricity</li>
                                 <li><span>Start and end date:</span><br>2019/05/30 - 2020/12/28</li>
                            </ul>
                        </div>
                        <div class="tab-des" id="education">
                            <ul>
                                 <li><span> Degree:</span><br>Bachelor's </li>
                                 <li><span>University:</span><br>IMSIU</li>
                                 <li><span>Graduation Date:</span><br> 2023/2024</li>
                            </ul>
                        </div>
                    </div>
            </div>
        </div>
        <div style="margin-right: 1200px;">
            <button class="btnback" onclick="location.href='#header';"><i class="fa-solid fa-house" style="color: #00aaff;"></i></i></button>
        </div>
        <BR>
              <!-- --------------CV PAGE------------ -->
          <div id="CV">
            <div class="container">
                <h1 class="title">CV</h1>
                <div style="margin-right:1000px">
                    <a href="RaghadabdEN.pdf" download="" class="btn btn2">Download CV</a>
                </div>
                <div class="cv-list">
                    <div>
                        <i class="fa-solid fa-magnifying-glass-chart"></i>
                        <h2>System Anlaysis</h2>
                        <p>i worked on a project in data analysis </p>
                        <a href="#">learn more</a>
                    </div>
                    <div>
                        <i class="fa-solid fa-code"></i>
                        <h2>information System</h2>
                        <p>i worked on a project in information System </p>
                        <a href="#">learn more</a>
                    </div>
                
                </div>
            </div>
          </div>    
          <div style="margin-right: 1200px;">
            <button class="btnback" onclick="location.href='#header';"><i class="fa-solid fa-house" style="color: #00aaff;"></i></i></button>
        </div>
        <BR><BR><BR><BR><BR><BR>
              <!-- -------------------INTRESTED PAGE-------------------->
  <div id="intrested">
    <div class="container">
        <h1 class="title"> My intrested</h1>
        <div class="work-list">
            <div class="work">
                <img src="DataAnalaysis.jpg" alt="">
                <div class="layer">
                    <h3>Data Anlaysis</h3>
                    <p>I am interested in the world of data and its analysis, especially data analysis using various types of languages and programming, whether tables or others, such as Microsoft Access and Oracle SQL</p>
                </div>
            </div>
            <div class="work">
                <img src="Codeing.jpg" alt="">
                <div class="layer">
                    <h3>Codeing</h3>
                    <p>I am interested in codeing Language </p>
                </div>
            </div>
        </div>
    </div>
  </div>
  <div style="margin-right: 1200px;">
    <button class="btnback" onclick="location.href='#header';"><i class="fa-solid fa-house" style="color: #00aaff;"></i></i></button>
</div>
<BR><BR><BR>
<!-- --------------------------Contact PAGE--------------------- -->
<div id="Contact">
    <div class="container">
        <div class="row">
            <div class="content-left">
                <h1 class="title">Contact Me</h1>
                <p>roodeabdullah@gmail.com</p>
                <p>0509588001</p>
            </div>
            <div class="content-right"></div>
            <form action="">
                <input type="text" name="Name" placeholder="Your Name" required>
                <input type="text" name="Email" placeholder="Example@gmail.com" required>
                <textarea name="Message" cols="30" rows="10" placeholder="Your message"></textarea>
                <button type="submit" class="btn btn2">Submit</button>
            </form>
        </div>
    </div>
</div>
<div style="margin-right: 1200px;">
    <button class="btnback" onclick="location.href='#header';"><i class="fa-solid fa-house" style="color: #00aaff;"></i></i></button>
</div>

<!-- -----------------------------------------JS CODE---------------------------------- -->
        <script>
            var tablinks = document.getElementsByClassName("tab-link");
            var tabDes = document.getElementsByClassName("tab-des");

            function opentab(tabname){
                for(tablink of tablinks){
                  tablink.classList.remove("actv-link");
                }
                for(tabDesc of tabDes){
                    tabDesc.classList.remove("actv-tab");
                }
                event.currentTarget.classList.add("actv-link");
                document.getElementById(tabname).classList.add("actv-tab");
            }
        </script>

        <script>
            var sidemenu = document.getElementById("sidemenu");
            function openmenu(){
                sidemenu.style.right = "0";
            }
            function closemenu(){
                sidemenu.style.right = "-200px";
            }
        </script>
    </body>
    <footer class="footer"> 
        <p class="footer-title">Copyrights @ <span>Raghad Abdullah</span></p> 
        <div class="social-icons"> 
         <a href="https://www.linkedin.com/feed/" target="_blank"><i class="fa-brands fa-linkedin"></i></a> 
         <a href="https://twitter.com/Graktang" target="_blank"><i class="fa-brands fa-square-x-twitter"></i></a> 
     </div> 
     </footer>
</html>
