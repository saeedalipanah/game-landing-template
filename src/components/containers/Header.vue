<template>
  <header class="third-header-bg">
    <div class="bg"></div>
    <div class="container custom-container">
      <div class="header-top-area t-header-top-area d-none d-lg-block">
        <div class="row">
          <div class="col-sm-6">
            <div class="header-top-social">
              <ul>
                <li>Follow</li>
                <li>
                  <a href="#"><i class="fab fa-twitter"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fab fa-facebook-f"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fab fa-vimeo-v"></i></a>
                </li>
                <li>
                  <a href="#"><i class="fab fa-youtube"></i></a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-sm-6">
            <div class="header-top-login">
              <ul>
                <li>
                  <a href="#"><i class="far fa-edit"></i>Register</a>
                </li>
                <li class="or">or</li>
                <li>
                  <a href="#"><i class="far fa-edit"></i>sign in</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div id="sticky-header">
      <div class="container custom-container">
        <div class="row">
          <div class="col-12">
            <div class="main-menu menu-style-two">
              <nav>
                <div class="logo d-block d-lg-none">
                  <a href="index-4.html"
                    ><img src="img/logo/logo.png" alt="Logo"
                  /></a>
                </div>
                <div class="navbar-wrap d-none d-lg-flex">
                  <ul class="left">
                    <li class="show">
                      <a href="#">Home</a>
                    </li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Overview</a></li>
                    <li><a href="#">Community</a></li>
                  </ul>
                  <div class="logo">
                    <a href="index-3.html"
                      ><img src="img/logo/h3_logo.png" alt="Logo"
                    /></a>
                  </div>
                  <ul class="right">
                    <li>
                      <a href="#">Pages</a>
                      <ul class="submenu">
                        <li>
                          <a href="#">Upcoming Games</a>
                        </li>
                        <li><a href="#">Game Single</a></li>
                      </ul>
                    </li>
                    <li><a href="#">Store</a></li>
                    <li>
                      <a href="#">Blog</a>
                      <ul class="submenu">
                        <li><a href="#">News Page</a></li>
                        <li><a href="#">News Details</a></li>
                      </ul>
                    </li>
                    <li><a href="#">contact</a></li>
                  </ul>
                </div>
                <div class="header-action">
                  <ul>
                    <li class="header-search">
                      <a
                        href="#"
                        data-toggle="modal"
                        data-target="#search-modal"
                        ><i class="fas fa-search"></i
                      ></a>
                    </li>
                  </ul>
                </div>
              </nav>
            </div>
            <div class="mobile-menu-wrap d-block d-lg-none">
              <nav>
                <div id="mobile-menu" class="navbar-wrap d-block">
                  <ul>
                    <li >
                      <a href="#">Home</a>
                    </li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Overview</a></li>
                    <li><a href="#">Community</a></li>
                   
                  </ul>
                </div>
              </nav>
            </div>
            <div class="mobile-menu"></div>
          </div>
          <!-- Modal Search -->
          <div
            class="modal fade"
            id="search-modal"
            tabindex="-1"
            role="dialog"
            aria-hidden="true"
          >
            <div class="modal-dialog" role="document">
              <div class="modal-content">
                <form>
                  <input type="text" placeholder="Search here..." />
                  <button><i class="fa fa-search"></i></button>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="header-bottom-bg"></div>
  </header>
</template>
<script>
export default {
  mounted(){
    /*=============================================
    =     Menu sticky & Scroll to top      =
=============================================*/
window.addEventListener('scroll',  () => {
	var scrollY = window.scrollY;
	if (scrollY < 60) {
		document.querySelector("#sticky-header").classList.remove("sticky-menu");
	} else {
		document.querySelector("#sticky-header").classList.add("sticky-menu");
	}
});
  }
}
</script>