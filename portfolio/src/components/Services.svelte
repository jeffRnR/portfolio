<script>
  import MainServices from "./servicesComponents/MainServices.svelte";
  import ToogleServices from "./servicesComponents/ToogleServices.svelte";
</script>

<body>
  <MainServices />
  <ToogleServices />
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
