<script>
  import TopBar from "../homeComponents/TopBar.svelte";
</script>

<TopBar />
<section class="mainServices" id="mainServices">
  <div class="leftMainServicesSection">
    <span>About My Services</span>
    <p>
      Enhance your online engagement with comprehensive web solutions! I provide
      web development, custom web and mobile applications, and seamless
      database/API integration for existing web apps. Let's build your digital
      future.
    </p>
  </div>
  <div class="rightMainServicesSection">
    <img src="https://www.cmindssolutions.com/img/web-mobile-development.png" />
  </div>
</section>

<style>
  .mainServices {
    display: flex;
    flex-direction: row;
    height: auto;
    min-height: 500px;
    margin: 10px;
    align-items: center;
    justify-content: center;
  }
  .leftMainServicesSection {
    flex: 3;
    margin-left: 15px;
    margin-right: 15px;
    align-items: center;
    justify-content: center;
    max-width: 500px;
  }
  .leftMainServicesSection span {
    font-family: Garamond, Baskerville, serif;
    font-size: 40px;
    color: #00808c;
    font-weight: 700;
  }
  .leftMainServicesSection p {
    font-size: 20px;
  }
  .rightMainServicesSection {
    margin-left: 15px;
    margin-right: 15px;
    align-items: right;
  }
  .rightMainServicesSection img {
    height: 350px;
    width: 350px;
    align-items: right;
    justify-content: end;
    border: rgb(0, 128, 140, 0.75) 5px solid;
    border-radius: 50%;
    filter: blur(0px);
    object-fit: cover;
  }
  .rightMainServicesSection img:hover {
    animation: zoom-out 1s ease-in-out;
    filter: blur(0.9px);
  }

  @keyframes zoom-out {
    from {
      transform: scale(1);
    }
    to {
      transform: scale(0.97);
    }
  }
</style>
