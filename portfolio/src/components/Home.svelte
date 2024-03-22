<script>
  import TopBar from "./homeComponents/TopBar.svelte";
  import About from "./homeComponents/About.svelte";
  import WorkExperience from "./homeComponents/WorkExperience.svelte";
  import Education from "./homeComponents/Education.svelte";
  import Skills from "./homeComponents/Skills.svelte";
  import Footer from "./homeComponents/Footer.svelte";
</script>

<head>
  <link
    rel="icon"
    href="https://github.com/jeffRnR/images/blob/main/pic.jpg?raw=true"
  />
</head>

<body>
  <TopBar />
  <About />
  <WorkExperience />
  <Education />
  <Skills />
  <Footer />
</body>

<style>
  * {
    margin: 0;
    padding: 0;
    outline: 0;
    border: 0;
    appearance: 0;
    list-style: none;
    text-decoration: none;
    box-sizing: border-box;
  }
  body {
    display: flex;
    flex-direction: column;
    background-color: #f9f6f6;
    height: auto;
  }
  body::-webkit-scrollbar {
    display: none;
  }
</style>
