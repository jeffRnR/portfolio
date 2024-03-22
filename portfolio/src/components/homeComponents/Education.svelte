<head>
  <link href="https://css.gg/css" rel="stylesheet" />
</head>

<section class="education">
  <div class="leftEducationSide">
    <span class="educationTitle">Education</span>
    <img
      src="https://img.freepik.com/free-vector/virtual-man-laptop-teaching-online_23-2148508675.jpg?size=626&ext=jpg&ga=GA1.1.749103614.1709293872&semt=ais"
      alt=""
    />
  </div>
  <div class="rightEducationSide">
    <div class="educationWrapper">
      <div class="educationDetails">
        <div class="educationDetail courseTitle">
          <span>Bachelors degree</span>
        </div>
        <div class="educationDetail course">
          <i class="gg-trophy"></i>
          <span>Bachelor of Science in Informatics and Computer Science </span>
        </div>
        <div class="educationDetail school">
          <i class="gg-readme"></i>
          <span>Strathmore University</span>
        </div>

        <div class="educationDetail location">
          <i class="gg-pin"></i>
          <span
            >Ole Sangale Rd, off Langata Road in Madaraka Estate
            <br />Nairobi, Kenya
          </span>
        </div>
        <div class="educationDetail educationDuration">
          <i class="gg-calendar-dates"></i>
          <span>From July 2020 - June 2024</span>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  @import url("https://css.gg/css");
  .education {
    display: flex;
    flex-direction: row;
    min-height: 450px;
    height: auto;
    margin: 10px;
    align-items: center;
    justify-content: center;
    width: auto;
  }
  .educationTitle {
    font-family: Garamond, Baskerville, serif;
    font-size: 40px;
    color: #00808c;
    font-weight: 700;
    margin-bottom: 20px;
    text-align: center;
    justify-content: start;
  }
  .leftEducationSide {
    margin-right: 20px;
    justify-content: flex-start;
    display: flex;
    flex-direction: column;
  }
  .leftEducationSide img {
    height: 350px;
    width: 350px;
    border: rgb(0, 128, 140, 0.75) 5px solid;
    border-radius: 50%;
  }
  .leftEducationSide img:hover {
    animation: zoom-out 1s ease-in-out;
    filter: blur(0.9px);
  }
  .rightEducationSide {
    display: flex;
    flex-direction: column;
    margin: 20px;
    height: 300px;
    justify-content: start;
    width: auto;
  }
  .educationDetails {
    display: flex;
    flex-direction: column;
    padding: 15px;
    height: auto;
    min-height: 250px;
    width: auto;
    border-radius: 10px;
    background-color: rgb(235, 235, 235);
    border-radius: 10px;
    padding: 10px;
    box-shadow: 5px 5px 5px rgb(0, 0, 0, 0.2);
    cursor: pointer;
  }
  .educationDetails:hover {
    border: #ebebeb 1px solid;
    box-shadow: 5px 5px 5px rgb(0, 0, 0, 0.4);
    cursor: pointer;
  }
  .educationDetail {
    display: flex;
    flex-direction: row;
    padding-left: 10px;
    margin-bottom: 10px;
    align-items: center;
  }
  .educationDetail i {
    margin-right: 10px;
    color: #00808c;
  }
  .educationDetail span {
    margin-left: 10px;
  }
  .courseTitle {
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
  .school,
  .course {
    font-weight: 500;
  }
  @keyframes zoom-out {
    from {
      transform: scale(1);
    }
    to {
      transform: scale(0.97);
    }
  }
  @media screen and (max-width: 1024px) {
    .education {
      display: flex;
      flex-direction: column;
    }
    .leftEducationSide img {
      height: 300px;
      width: 300px;
    }
  }
  @media screen and (max-width: 600px) {
    .education {
      display: flex;
      flex-direction: column;
    }
    .leftEducationSide img {
      height: 250px;
      width: 250px;
    }
  }
</style>
