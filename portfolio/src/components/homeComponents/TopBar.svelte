<script>
  import { Link } from "svelte-routing";
  function onOpenMenu() {
    document.getElementById("menu").style.opacity = "1";
    document.getElementById("menuIcon").style.display = "none";
  }
  function onCloseMenu() {
    document.getElementById("menu").style.opacity = "0";
    document.getElementById("menuIcon").style.display = "inline";
  }
</script>

<head>
  <link href="https://css.gg/css" rel="stylesheet" />
</head>
<section class="topBar" id="topBar">
  <div class="leftTopBarSide">
    <span href="#">Jeff Munyigi</span>
    <p>Software Engineer</p>
    <p></p>
  </div>

  <div class="rightTopBarSide">
    <Link to="/services" style="text-decoration: none;"
      ><span class="rightTopBarSideDetails">Services</span></Link
    >
    <span class="rightTopBarSideDetails" href="">Projects</span>
    <span class="rightTopBarSideDetails" href="">Contact</span>
    <button class="rightTopBarSideDetails giftButton">Gift me</button>
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <span class="menuIcon" id="menuIcon"
      ><i class="gg-menu" on:click={onOpenMenu}></i></span
    >
  </div>
</section>
<div class="menu" id="menu">
  <div class="menuBar">
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <i class="gg-close" on:click={onCloseMenu}></i>
  </div>
  <div class="menuItems">
    <span class="menuItem">Services</span>
    <span class="menuItem">Projects</span>
    <span class="menuItem">Contacts</span>
    <button class="giftButton">Gift me</button>
  </div>
</div>

<!-- <Menu {isMenuOpen} /> -->

<style>
  @import url("https://css.gg/css");
  .topBar {
    position: sticky;
    display: flex;
    background-color: rgb(235, 235, 235);
    padding: 5px;
    height: 50px;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    top: 0;
  }
  .leftTopBarSide {
    flex: 3;
    display: flex;
    align-items: center;
  }
  .leftTopBarSide span {
    font-family: Garamond, Baskerville, serif;
    font-size: 25px;
    color: #00808c;
    font-weight: 800;
    margin-left: 20px;
    margin-right: 20px;
    cursor: pointer;
  }
  .leftTopBarSide p {
    font-family: Georgia, serif;
    font-size: 14px;
    color: #333333;
    font-weight: 600;
    opacity: 0.7;
  }

  .rightTopBarSide {
    flex: 2;
    padding-left: 5px;
    text-align: center;
  }
  .rightTopBarSideDetails {
    font-size: 15px;
    font-family: Georgia, serif;
    padding-left: 10px;
    color: #333333;
    cursor: pointer;
  }
  .rightTopBarSideDetails:hover {
    text-decoration: none;
    color: #00808c;
  }
  .giftButton {
    background-color: #333333;
    color: white;
    border-radius: 10px;
    width: auto;
    margin-left: 10px;
  }
  .giftButton:hover {
    background-color: #00808c;
    color: white;
  }
  .menuIcon {
    display: none;
    cursor: pointer;
  }
  .menu {
    display: none;
  }
  .menuBar {
    background-color: rgb(225, 225, 225);
    height: auto;
    padding: 10px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
  }
  .menuItems {
    display: flex;
    flex-direction: column;
    align-items: right;

    padding: 10px;
    justify-content: flex-start;
    height: auto;
  }
  .menuItem {
    font-size: 15px;
    border-bottom: black 1px solid;
    color: #00808c;
    margin-bottom: 10px;
    padding-bottom: 10px;
  }
  .menuItem:last-child {
    border-bottom: none;
  }

  @media screen and (max-width: 1024px) {
    .rightTopBarSideDetails {
      display: none;
    }
    .leftTopBarSide {
      flex: 4;
    }
    .leftTopBarSide span {
      font-size: 22px;
    }
    .leftTopBarSide p {
      font-size: 12px;
    }
    .rightTopBarSide {
      flex: 1;
      padding-left: 5px;
      justify-content: center;
    }

    .menuIcon {
      display: inline;
    }
    .menu {
      position: absolute;
      height: auto;
      min-height: 250px;
      max-height: fit-content;
      background-color: rgb(235, 235, 235);
      border-radius: 10px;
      top: 5%;
      right: 3.5%;
      width: 300px;
      display: flex;
      flex-direction: column;
      opacity: 0;
      position: fixed;
      z-index: 1000;
    }
  }
  @media screen and (max-width: 600px) {
    .rightTopBarSideDetails {
      display: none;
    }
    .topBar {
      height: auto;
    }

    .menuIcon {
      display: inline;
    }
    .menu {
      position: fixed;
      height: auto;
      min-height: 150px;
      max-height: fit-content;
      background-color: rgb(235, 235, 235);
      border-radius: 10px;
      top: 1.75%;
      right: 0%;
      width: 200px;
      display: flex;
      flex-direction: column;
      opacity: 0;
      z-index: 1000;
    }
    .leftTopBarSide {
      height: auto;
    }
    .leftTopBarSide span {
      font-size: 18px;
    }
    .leftTopBarSide p {
      display: none;
    }
  }
</style>
