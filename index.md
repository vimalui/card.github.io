<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <title>Frontend Mentor | Stats preview card component</title>
  
  <style>

    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Lexend+Deca&display=swap');

    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    a{
      text-decoration: none;
      color: #cea3e9;
      font-weight: 600;
    }
    :root{
      --heading-color: hsl(0, 0%, 100%);
      --txt-color: hsl(277, 64%, 61%);
      --para-color: hsla(0, 0%, 100%, 0.75);
    }
    body{
      font-size: 15px;
      font-family: 'Inter', sans-serif;
    }
    .container{
      max-width: 1440px;
      margin:auto;
      padding: 100px;
      background: hsl(233, 47%, 7%);
    }
    .attribution{
      max-width: 1440px;
      padding: 20px;
      text-align: center;
      background: #1b1938;
      color: #fff;
    margin:auto;
    }
    .flex-row{
      display: flex;
      width: 100%;
      align-items: center;
      overflow: hidden;
      border-radius: 10px;
      background: hsl(244, 38%, 16%);
    }
    .flex-col{
      width: 50%;
    }
    .flex-col:nth-child(1){
      padding: 75px;
    }
    .flex-col:nth-child(2){
      background: url(./images/image-header-desktop.jpg),linear-gradient(to right,hsl(277, 64%, 61%),hsl(277, 64%, 61%));
      background-size: cover;
      background-position: center;
      padding: 200px;
      position: relative;
      background-blend-mode: multiply;
    }
    h1{
      color: var(--heading-color);
      margin-bottom: 10px;
    }
    p{
      color:var(--para-color) ;
      line-height: 25px;
    }
    .text-color{
      color: var(--txt-color);
    }
    .our-achievements{
      display: flex;
    }
    .our-achievements div{
      padding: 20px;
    }
    .our-achievements div span:first-child {
      color: var(--heading-color);
      font-weight: 700;
      margin-bottom: 10px;
      text-align: center;
    }
    .our-achievements div span:last-child {
      color:var(--para-color);
      text-transform: uppercase;
      font-size: 13px;
      font-family: 'Lexend Deca', sans-serif;
    }
    @media (max-width: 1199.98px){
      .flex-col:nth-child(2){
        padding: 220px;
      }
    }
    @media (max-width: 991.98px) {
      .container{
        padding: 50px;
        margin: 0 auto;
      }
      .flex-row{
        flex-direction: column-reverse;
      }
      .flex-col{
        width: 100%;
      }
      .flex-col:nth-child(1){
        padding: 25px;
        text-align: center;
      }
      .flex-col:nth-child(2){
        padding: 130px;
      }
      h1{
        font-size: 23px;  
      }
      p{
        font-size: 13px;
        line-height: 23px;
      }
      .our-achievements{
        display: flex;
        flex-direction: column;
      }
      .our-achievements div {
          padding: 20px 0px 0px;
      }
    }


  </style>
</head>
<body>
  <div class="container">
    <div class="flex-row">
      <div class="flex-col">
        <h1>Get <span class="text-color">insights</span> that help your business grow.</h1>
        <p>Discover the benefits of data analytics and make better decisions reGarding revenue, customer experience, and overall efficiency.</p>
        <div class="our-achievements">
          <div><span>10k+</span> <br/> <span>companies</span></div>
          <div><span>314</span> <br/> <span>templates</span></div>
          <div><span>12m+</span> <br/> <span>queries</span></div>
        </div>
      </div>
      <div class="flex-col">
      </div>
    </div>
  </div>

  <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="http://www.linkedin.com/in/vimal-d">Vimal.D UI Developer</a>.
  </div>
</body>
</html>
