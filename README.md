# unifox Start Your Business Today
UNIFOX (Start Your Business Today ) Design with (HTML , CSS, Bootstrap4,  jQuery and Java script) 
Html(code)
 <div class="home" id="home">
        <div class="overlay">
            <div class="navbar navbar-expand-lg navbar-light fixed-top">
                <div class="container">
                    <a class="navbar-brand" href="">
                        Unifox
                    </a>
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#main-nav"
                        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="collapse navbar-collapse" id="main-nav">
                        <ul class="navbar-nav ml-auto">
                            <li class="nav-item">
                                <a class="nav-link" href="">Home</a>
                            </li>
                            <li class="nav-item ">
                                <a class="nav-link" href="#about">About</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#services">Services</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#portfolio">Portfolio</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#prices">Prices</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#team">Team</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#testmonial">Testmonial</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#blog">Blog</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#contact">Contact</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="home-content text-center">
                <h1>Start Your Business Today</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem rem rerum nam recusandae
                    dicta maiores. Dignissimos nostrum, cumque numquam quae voluptatum qui.</p>
                <button type="button" class="btn btn-success">Start Now</button>
                <button type="button" class="btn btn-success">Discover me</button>
            </div>
        </div>
    </div>
    
    css (code)
    body{font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;}
/*start home*/
.home{
    height: 100vh;
    background-image: url("../images/home/skill-bg.jpg");
    background-size: cover;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-position: center;
    background-attachment: fixed;
    position: relative;
}
.home .overlay{
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background: rgba(0,0,0,0.6)}
/* .home .sticky-top{
    position: fixed;
    width: 100%;
} */
.home .navbar.green{background-color: #28a745;box-shadow: 0 2px 10px 0 #000;}
.home .navbar-light .navbar-brand{
    font-size: 30px;
    color: beige
}
.home .navbar-light .nav-item .nav-link {color: beige;}
.home .navbar-light ul li{
    margin-left: 10px;
    font-size: 18px;
    font-weight: 500;
    z-index: 1;
}
.home .navbar-light ul li a{transition: all 0.3s ease 0s}
.home .home-content{
    color: beige;
    margin-top: 225px;
    z-index: 1;
}
.home .home-content p{padding: 10px 250px;}
@media (max-width:922px){
    .home .home-content p{padding: 10px 0;}
}
.home .home-content button{
    margin-left: 20px; 
    color: beige;
}
.home .btn-success:hover {
   background-color: transparent;}
   
   JS(code)
   // Scroll to Top
$('.scrollTop').click(function(){
    $('body,html').animate({
        scrollTop : 0
    },500);
});

//smooth scroll

    $('.nav-item a').click(function(){
        
        $('body,html').animate({
            scrollTop : $($(this).attr('href')).offset().top - 80
        });
    });

});
