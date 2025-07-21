<script>
import InstagramLogoSvgComponent from "@/components/SvgComponents/InstagramLogoSvgComponent.vue";
import TelegramLogoSvgComponent from "@/components/SvgComponents/TelegramLogoSvgComponent.vue";
import GithubLogoSvgComponent from "@/components/SvgComponents/GithubLogoSvgComponent.vue";
import PhoneLogoSvgComponent from "@/components/SvgComponents/PhoneLogoSvgComponent.vue";

export default {
  name: "NavbarComponent",
  components: {
    InstagramLogoSvgComponent,
    TelegramLogoSvgComponent,
    GithubLogoSvgComponent,
    PhoneLogoSvgComponent
  }
}
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid flex-row justify-content-center align-items-center">
      <a class="navbar-brand" href="#">
        <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M0 20C0 8.95431 8.95431 0 20 0H40V20C40 31.0457 31.0457 40 20 40V40C8.95431 40 0 31.0457 0 20V20Z" fill="#8643DC"/>
          <path d="M16 10C16 4.47715 20.4772 0 26 0H40V13C40 18.5228 35.5228 23 30 23H16V10Z" fill="#FF59C1"/>
          <path d="M17.79 30L8.73 9H13.98L21.9 27.6H18.81L26.85 9H31.68L22.59 30H17.79Z" fill="white"/>
        </svg>
      </a>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav gap-3">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Service</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Work</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Blog</a>
          </li>
        </ul>
        <ul class="navbar-nav flex-row justify-content-center align-items-center gap-3">
          <li class="nav-item social-btn">
            <a class="nav-link" href="#">
                <InstagramLogoSvgComponent />
            </a>
          </li>
          <li class="nav-item social-btn">
            <a class="nav-link" href="#">
              <TelegramLogoSvgComponent />
            </a>
          </li>
          <li class="nav-item social-btn">
            <a class="nav-link" href="#">
                <GithubLogoSvgComponent />
            </a>
          </li>
          <li class="nav-item social-btn">
            <a class="nav-link" href="#">
              <PhoneLogoSvgComponent />
            </a>
          </li>
        </ul>

      </div>
    </div>
  </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap');
#navbarNav {
  display: flex;
  flex-direction: row;
  justify-content: end;
}
.social-btn:hover{
  background-color: #c5c5c5;
  border-radius: 50%;
}
.nav-link {
  font-family: "Red Hat Display", sans-serif;
  font-optical-sizing: auto;
  font-weight: 500;
  font-style: normal;
}
</style>