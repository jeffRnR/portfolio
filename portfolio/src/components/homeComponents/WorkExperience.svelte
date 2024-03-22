<script>
  import { onMount } from "svelte";
</script>

<head>
  <link href="https://css.gg/css" rel="stylesheet" />
</head>
<section class="workExperience">
  <span class="workExperienceTitle">Work Experience</span>
  <div class="workExperienceWrapper">
    <div class="workExperienceDetails">
      <div class="workTitle">
        <i class="gg-work-alt"></i>
        <span>Technical support</span>
      </div>

      <span class="workCompany">Cloudoon, Nairobi, Kenya</span>
      <span class="duration">March 2024 - Present</span>
      <div class="workLink">
        <a href="" target="_blank">Learn more...</a>
      </div>
    </div>

    <div class="workExperienceDetails">
      <div class="workTitle">
        <i class="gg-work-alt"></i>
        <span>IT Intern</span>
      </div>
      <span class="workCompany"
        >Brightening Academic Center, Nairobi, Kenya</span
      >
      <span class="duration">February 2023 - April 2023 </span>
      <div class="workLink">
        <a href="" target="_blank">Learn more...</a>
      </div>
    </div>

    <div class="workExperienceDetails">
      <div class="workTitle">
        <i class="gg-work-alt"></i>
        <span>IT Assistant</span>
      </div>
      <span class="workCompany"
        >Super Quality Snack Limited, Nairobi, Kenya</span
      >
      <span class="duration">January 2022 - April 2022</span>
      <div class="workLink">
        <a href="" target="_blank">Learn more...</a>
      </div>
    </div>
  </div>
</section>

<style>
  @import url("https://css.gg/css");

  .workExperience {
    background-color: rgb(235, 235, 235);
    display: flex;
    flex-direction: column;
    height: auto;
    margin-top: 20px;
    margin-bottom: 10px;
    padding: 10px;
  }
  .workExperienceTitle {
    font-family: Garamond, Baskerville, serif;
    font-size: 40px;
    color: #00808c;
    font-weight: 700;
    margin: 20px;
    margin-bottom: 20px;
  }
  .workExperienceWrapper {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-column-gap: 10px;
    /* animation: shootFromLeft 1s ease-in-out forwards; */
  }
  .workExperienceDetails {
    display: flex;
    flex-direction: column;
    background-color: #f9f6f6;
    margin: 10px;
    padding: 15px;
    height: 200px;
    width: auto;
    border-radius: 10px;
    box-shadow: 5px 5px 5px rgb(0, 0, 0, 0.2);
  }
  .workExperienceDetails:hover {
    border: #ebebeb 1px solid;
    box-shadow: 5px 5px 5px rgb(0, 0, 0, 0.4);
    cursor: pointer;
  }

  .workLink {
    display: flex;
    justify-items: flex-end;
    align-items: flex-end;
  }
  .workLink a {
    color: #00808c;
    text-decoration: none;
  }
  .workLink a:hover {
    color: #333333;
  }
  .workTitle {
    padding-top: 10px;
    padding-bottom: 10px;
    font-size: 20px;
    font-weight: 700;
    font-family: Georgia, serif;
    border-bottom: #333333 1px solid;
    display: flex;
    align-items: center;
    color: #333333;
  }
  .workTitle i {
    margin-right: 10px;
    color: #00808c;
  }
  .workCompany {
    font-size: 20px;
    margin-top: 10px;
    max-width: 250px;
    font-weight: 600;
    color: #330330;
    font-family: Garamond, Baskerville, serif;
  }
  .duration {
    font-size: 15px;
    margin-top: 10px;
    max-width: 200px;
  }
  @keyframes zoom-out {
    from {
      transform: scale(1);
    }
    to {
      transform: scale(0.97);
    }
  }

  @keyframes shootFromLeft {
    from {
      transform: translateX(-100%);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }

  @media screen and (max-width: 1024px) {
    .workExperienceTitle {
      font-size: 35px;
    }
    .workExperienceWrapper {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-column-gap: 2px;
    }
  }
  @media screen and (max-width: 600px) {
    .workExperienceTitle {
      font-size: 30px;
      text-align: center;
    }
    .workExperienceWrapper {
      display: flex;
      flex-direction: column;
    }
  }
</style>
