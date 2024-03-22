<script>
</script>

<head><link href="https://css.gg/css" rel="stylesheet" /></head>

<section class="toogleServices">
  <div class="servicesTitles">
    <span id="website" class="servicesTitle">Website</span>
    <span id="web-app" class="servicesTitle"> Web-app</span>
    <span id="mobile" class="servicesTitle">Mobile</span>
    <span id="database" class="servicesTitle">Database</span>
  </div>

  <div class="websiteContainer">
    <div class="websiteContainerTop">
      <div class="websiteContainerTopWrapper">
        <div class="websiteContainerTopLeft">
          <span class="serviceName">Website Development</span>
        </div>
        <div class="websiteContainerTopRight">
          <p>
            Web development is all about bringing your vision for a website to
            life. I can translate your ideas into a user-friendly and visually
            appealing online presence. Think of me as the builder who works on
            both the inside and outside of your digital house. I can handle the
            design, like the layout and how it looks, and the technical stuff
            that makes it work smoothly, like adding forms or connecting to a
            database. Basically, I'll take care of everything to get your
            website up and running and looking great!
          </p>
        </div>
      </div>
      <div></div>
    </div>
  </div>

  <div class="web-appContainer"></div>
  <div class="mobileContainer"></div>
  <div class="databaseContainer"></div>
</section>

<style>
  .toogleServices {
    display: flex;
    flex-direction: column;
    height: auto;
  }
  .servicesTitles {
    display: flex;
    flex-direction: row;
  }
  .servicesTitle {
    background-color: rgb(235, 235, 235);
    cursor: pointer;
    margin-top: 10px;
    padding-left: 10px;
  }
  .websiteContainer {
    background-color: rgb(235, 235, 235);
    display: flex;
    flex-direction: column;
  }
  .websiteContainerTop {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: start;
  }
  .websiteContainerTopWrapper {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: start;
  }
  .websiteContainerTopLeft {
    flex: 1;
    margin-left: 15px;
    margin-right: 15px;
    margin: 15px;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .websiteContainerTopRight {
    flex: 1;
    margin-left: 15px;
    margin-right: 15px;
    align-items: center;
    justify-content: center;
    max-width: 500px;
  }
  .serviceName {
    font-family: Garamond, Baskerville, serif;
    font-size: 40px;
    color: #00808c;
    font-weight: 700;
    margin-bottom: 20px;
    text-align: center;
    align-items: flex-start;
    justify-content: flex-start;
  }
</style>
