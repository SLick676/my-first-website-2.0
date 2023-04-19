<head>
    <style>
      body {
        font-family: tahoma;
        text-align: center;
      }
      header {
        letter-spacing: 6px;
        background: royalblue;
        padding: 20px;
        color: white;
      }
      h2 {
        font-size: 2em;
        width: 100%;
      }
      section {
        padding: 30px;
        margin-bottom: 40px;
      }
      .flex-container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
      }
      .card {
        border: 1px solid #ccc;
        background-color: ivory;
        margin: 25px;
        padding: 25px;
        box-shadow: 6px 6px 6px rgba(0, 0, 0, 0.3)
      }
      .icons {
        font-size: 8em;
        padding: 25px;
      }
      button, .button {
        background: royalblue;
        border: 0;
        color: white;
        padding: 10px;
        width: 100%;
        margin-bottom: 10px;
      }
      td {
        padding: 10px;
      }
      table {
        margin: auto;
      }
      #my-order{
        background-color: #29C1C4;
        padding: 25px;
        display: none;
      }
      @media (min width: 50em) {
        .card {
          flex-basis: 325px;
        }
        header h1 {
          font-size: 5em;
        }
      }
      .footer{
        padding: 30px;
        background: grey;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Awesome IndustriesInc.</h1>
      <h4>Cute Cupcakes for Best Besties</h4>
    </header>
    <section>
      <h2>WELCOME:</h2>
      <p>VISION: To create beautiful cupcakes for clients in the Randburg area</p>
      <br><br>
      <p>ABOUT US: Founded in 2018, by Thandi Ndlovo. We've served over 100 clients and delivered over 10,000 tasty treats.</p>
    </section>
    <section class="flex-container">
      <h2>SERVICES://</h2>
      <article class="card">
        <div class="icons "> &#10873</div>
        <h3>David Mukhura </h3>
        <p>Jnr. Web Developer Creates simple, beautiful websites for businesses in Soweto.</p>
        <button> Contact </button>
      </article>
      <article class="card">
        <div class="icons"> &#20584</div>
        <h3>Jack Russle </h3>
        <p>Jnr. Web Developer Creates simple, beautiful websites for businesses in Soweto.</p>
        <button> Contact </button>
      </article>
    </section>
         <section class="container" style="background color: deeppink;">
      <h2>OUR TEAM://</h2>
      <article class="card">
        <div class="icons "> &#10058</div>
        <h3>jack jonhson</h3>
        <p>Front-end Web Developer Creates simple, beautiful websites for businesses in Joburg CBD.</p>
        <button> Remove </button>
      </article>
      <article class="card">
        <div class="icons"> &#10081</div>
        <h3>junior jackson </h3>
        <p>Full stack Web Developer Creates simple, beautiful websites for businesses in Santon.</p>
        <button> Remove </button>
      </article>
    </section>
    <section>
      <h2> MY ORDER FORM: </h2>
      <form id="my-form">
        <table>
          <tr>
            <td> Name: </td>
            <td><input type="text" size="25" name="my-name"></td>
          </tr>
          <tr>
            <td> Address: </td>
            <td><input type="text" size="25" name="my-address"></td>
          </tr>
          <tr>
            <td> Favourite drink: </td>
            <td>
              <select name="my-drink">
                <option> Milk </option>
                <option> Coffee </option>
                <option> Tea </option>
              </select>
            </td>
          </tr>
          <tr>
            <td> Quantity: </td>
            <td><input type="number" name="my-qty" value="1" min="1" max="5">
              <small>(max 5)</small>
            </td>
          </tr>
          <tr> <br>
          </tr>
          <tr>
            <td colspan="2">
              <input class="button" type="button" value="Process Order" onclick="placeOrder();">
              <input class="button" type="reset" value="Clear">
            </td>
          </tr>
        </table>
      </form>
            <div id="my-order">
            </div>  
    </section>
    <script>
     function placeOrder(){
     var orderForm = document.getElementById("my-form");   
     results = "<h3>Success</h3> Here is your order.";
     results += "<br>Name:" +orderForm.elements["my-name"].value;   
     results += "<br>Address: " +
    orderForm.elements["my-address"].value; 
     results += "<br>I like to order: " +
    orderForm.elements["my-drink"].value;
     results += "<Quantity> + " +
    orderForm.elements["my-qty"].value; 
     var orderResults = document.getElementById("my-order"); 
     orderResults.style.display = "block";   
     orderResults.innerHTML = results;
      }
   </script>
    <footer>
       <div class= "footer">
         <h3>Thanks for visiting.</h3>
         <div class= container>
           <article class= "card">
             <h3>Get in touch.</h3>
             <p>       Probably the best place to buy     cupcakes in all of Joburg.
             </p>
           </article>
           <article class= "card">
             <h3>Contact Us:</h3>
             <p>We would love to hear from you.<br>
               Call or email us.</br>
               Mobile: 072345 633 //
               Tel: 012 343 3432
               </p>
               
           </article>
           </div>
         &copy Awesome Industries  Inc.
         </div>
     </footer>
  </body>  
  
  
                   
