<script>
  import { onMount } from "svelte";
  function toggleMore() {
    showMore = !showMore;
  }

  onMount(() => {
    const moreText = document.getElementById("moreText");
    if (moreText && moreText.scrollHeight <= moreText.clientHeight) {
      document.getElementById("toggleMore").style.display = "none";
    }
  });
  let showMore = false;
</script>

<head>
  <link href="https://css.gg/css" rel="stylesheet" />
</head>

<section class="aboutSection">
  <div class="leftAboutSection">
    <span>About Me</span>
    <p>
      Hello and welcome! I'm Jeff Jackson Munyigi, a passionate software
      engineer with a background in Informatics and computer science.

      {#if showMore}
        <br />
        Software solutions have become my tool for unlocking the potential of technology
        in building inovative and problem-solving systems for the good of society.
        I have honed my skills in web and mobile application development, crafting
        user-centric experiences that bridge the gap between technology and its users.
        To ensure the smooth operation of these systems, I possess in-depth knowledge
        of Linux server administration, allowing me to manage and secure the backbone
        of any digital project. And talk about intelligent systems, machine learning
        is part of my DNA, and it facilitates the integration of even broarder solutions
        to automate our lives.
        <br />I'm excited to showcase my projects and experiences gained through
        my journey in the industry.
        <p />
      {/if}
      <a href="" id="toggleMore" on:click|preventDefault={toggleMore}>
        {showMore ? " Read less" : " Read more..."}
      </a>
    </p>
  </div>
  <div class="rightAboutSection">
    <img
      src="https://github.com/jeffRnR/images/blob/main/pic.jpg?raw=true"
      alt="pic"
    />
  </div>
</section>

<style>
  @import url("https://css.gg/css");
  .aboutSection {
    display: flex;
    flex-direction: row;
    height: auto;
    min-height: 500px;
    margin: 10px;
    align-items: center;
    justify-content: center;
  }
  .leftAboutSection {
    flex: 3;
    margin-left: 15px;
    margin-right: 15px;
    align-items: center;
    justify-content: center;
    max-width: 500px;
  }

  .leftAboutSection span {
    font-family: Garamond, Baskerville, serif;
    font-size: 40px;
    color: #00808c;
    font-weight: 700;
  }
  .leftAboutSection p {
    font-size: 20px;
  }
  #toggleMore {
    color: #00808c;
    cursor: pointer;
    text-decoration: none;
    font-weight: 550;
  }
  .rightAboutSection {
    margin-left: 15px;
    margin-right: 15px;
    align-items: right;
  }
  .rightAboutSection img {
    height: 350px;
    width: 350px;
    align-items: right;
    justify-content: end;
    border: rgb(0, 128, 140, 0.75) 5px solid;
    border-radius: 50%;
    filter: blur(0px);
    object-fit: cover;
  }
  .rightAboutSection img:hover {
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
    .aboutSection {
      display: flex;
      flex-direction: column;
      height: auto;
      min-height: 450px;
    }
    .leftAboutSection span {
      font-size: 35px;
    }
    .leftAboutSection p {
      font-size: 20px;
    }
    .rightAboutSection img {
      height: 300px;
      width: 300px;
    }
  }
  @media screen and (max-width: 600px) {
    .aboutSection {
      height: auto;
      min-height: 400px;
    }
    .leftAboutSection span {
      font-size: 30px;
    }
    .leftAboutSection p {
      font-size: 15px;
    }
    .rightAboutSection img {
      height: 250px;
      width: 250px;
    }
  }
</style>
