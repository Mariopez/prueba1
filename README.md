# prueba1
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title> CARD  CATS  FHOTO </title>
    
    
   </head>
  <body>
    <div class="wrapper">
      <div class="container center">
        <div class="card">
          <div class="front center">
             <img src="https://bit.ly/fcc-relaxing-cat" alt="fotos de gatos.">
            <h3>Front</h3>
            <p>3D Welcome !</p>
          </div>
          <div class="back center">
              <img src="https://bit.ly/fcc-relaxing-cat" alt="fotos de gatos.">
            <h3>back</h3>
            <p> CATS FHOTO </p>
          </div>
        </div>
      </div>
     
    </div>
  </body>
</html>

* {
        padding: 0;
        margin: 0;
        -webkit-box-sizing: border-box;
                box-sizing: border-box;
        font-family: "Poppins", sans-serif;
      }
      body {
        background-color: #40f558;
      }
      .wrapper {
        width: 19.75em;
        position: absolute;
        -webkit-transform: translate(-50%,-50%);
            -ms-transform: translate(-50%,-50%);
                transform: translate(-50%,-50%);
        top: 50%;
        left: 50%;
      }
      .container {
          position: relative;
        -webkit-perspective: 25em;
                perspective: 25em;
      }
      a {
        display: block;
        color: #ffffff4d;
        background-color: #4c199e9d;
        width: 100%;
        font-size: 1.2em;
        margin-top: 3em;
        text-align: center;
        padding: 2em 0;
        border-radius: 0.3em;
        text-decoration: none;
        font-weight: 600;
      }
      .card {
        height: 25em;
        width: 100%;
        -webkit-transform-style: preserve-3d;
                transform-style: preserve-3d;
        position: relative;
        -webkit-transition: 2s;
        -o-transition: 2s;
        transition: 2s;
        font-family: "Poppins", sans-serif;
        -webkit-animation: spin 12s infinite linear;
                animation: spin 12s infinite linear;
      }
      @-webkit-keyframes spin {
        100% {
          -webkit-transform: rotateY(360deg);
                  transform: rotateY(360deg);
        }
      }
      @keyframes spin {
        100% {
          -webkit-transform: rotateY(360deg);
                  transform: rotateY(360deg);
        }
      }
      .front,
      .back {
        background-color: #1c426d;
        font-size: 1.2em;
        height: 100%;
        width: 100%;
        -webkit-backface-visibility: hidden;
                backface-visibility: hidden;
        border-radius: 0.3em;
      }
      .back {
        position: relative;
        bottom: 100%;
        -webkit-transform: rotateY(180deg);
                transform: rotateY(180deg);
      }
      .center {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-align: center;
            -ms-flex-align: center;
                align-items: center;
        -webkit-box-pack: center;
            -ms-flex-pack: center;
                justify-content: center;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
            -ms-flex-direction: column;
                flex-direction: column;
        text-align: center;
      }
      .container h3 {
        font-weight: 500;
        letter-spacing: 0.08em;
      }
      .container p {
        color: #838094;
        font-size: 0.8em;
        font-weight: 300;
        letter-spacing: 0.05em;
      }
      img {
        width: 8em;
        margin-bottom: 2em;
      }
      @media screen and (max-width: 500px) {
        .container {
          font-size: 16px;
        }
      }
