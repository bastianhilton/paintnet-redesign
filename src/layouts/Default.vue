<template>
  <div class="layout">
    <header class="header">
      <section data-bs-version="5.1" class="menu menu1 cid-sFGMsvHDIa" once="menu" id="menu1-1">


        <nav class="navbar navbar-dropdown navbar-fixed-top navbar-expand-lg">
          <div class="container-fluid">
            <div class="navbar-brand">
              <span class="navbar-logo">
                <a href="https://www.getpaint.net">
                  <img src="../assets//images/logo4.png" alt="Paint.net" style="height: 3rem;">
                </a>
              </span>

            </div>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-bs-toggle="collapse"
              data-target="#navbarSupportedContent" data-bs-target="#navbarSupportedContent"
              aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
              <div class="hamburger">
                <span></span>
                <span></span>
                <span></span>
                <span></span>
              </div>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav nav-dropdown" data-app-modern-menu="true">
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7" href="/">Home</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/features">Features</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/donate">Donate</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/download">Download</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/license">License</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/roadmap">Roadmap</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="https://forums.getpaint.net/" target="_blank">Forum</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="https://blog.getpaint.net">Blog</a></li>
                <li class="nav-item"><a class="nav-link link text-white text-primary display-7"
                    href="/contact">Contact</a>
                </li>
              </ul>
              <div class="icons-menu">
                <a class="iconfont-wrapper" href="https://twitter.com/rickbrewPDN" target="_blank">
                  <span class="p-2 mbr-iconfont socicon-twitter socicon"
                    style="color: rgb(255, 255, 255); fill: rgb(255, 255, 255);"></span>
                </a>



              </div>
              <div class="navbar-buttons mbr-section-btn"><a class="btn btn-primary display-4"
                  href="/download">Download</a></div>
            </div>
          </div>
        </nav>
      </section>
    </header>
    <slot />
    <section data-bs-version="5.1" class="footer7 cid-sFGSOnwtIp" once="footers" id="footer7-c">
      <div class="container">
        <div class="media-container-row align-center mbr-white">
          <div class="col-12">
            <p class="mbr-text mb-0 mbr-fonts-style display-7">
              © Copyright 2025 <a href="https://www.getpaint.net" class="text-white text-primary">Paint.Net</a> - All
              Rights Reserved
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<static-query>
  query {
  metadata {
  siteName
  }
  }
</static-query>

<style>

</style>