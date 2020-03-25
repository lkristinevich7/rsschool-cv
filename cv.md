# Liudmila Krystsinevich

## Contact
tel. +48791684043, e-mail lkristinevich7@gmail.com

## Summary
 I am a person passionate about technologies, who is looking for challenging opportunities to develop my skills and get new ones. I have a unique combination of strong technical skills and communication skills. I enjoy building sites and web applications using HTML, CSS, JS and React.js. Additionally I am capable to work with Excel and SQL. I am a fluent in English, Polish and Russian. Considering my soft skills I would like to emphasize exceptional organizational and communication skills. I am a highly-motivated person who is willing to go above and beyond on any project and to learn valuable skills on my own time. 
 
## Skills:
* HTML - advanced
* CSS - advanced
* JS - advanced
* JQuery - advanced
* Github - advanced
* npm - advanced
* Bootsrap - advanced
* SQL - advanced
* React.js - basic
* Saas - basic

## Code examples
```html, css, javascript
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Exchange Rate Calculator</title>
    <style>
        :root {
      --primary-color: #5fbaa7;
    }

    * {
      box-sizing: border-box;
    }

    body {
      background-color: #f4f4f4;
      font-family: Arial, Helvetica, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      padding: 20px;
    }

    h1 {
      color: var(--primary-color);
    }

    p {
      text-align: center;
    }

    .btn {
      color: #fff;
      background: var(--primary-color);
      cursor: pointer;
      border-radius: 5px;
      font-size: 12px;
      padding: 5px 12px;
    }

    .money-img {
      width: 150px;
    }

    .currency {
      padding: 40px 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .currency select {
      padding: 10px 20px 10px 10px;
      -moz-appearance: none;
      -webkit-appearance: none;
      appearance: none;
      border: 1px solid #dedede;
      font-size: 16px; 
      background: transparent;
      background-image: url('data:image/svg+xml;charset=US-ASCII,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20width%3D%22292.4%22%20height%3D%22292.4%22%3E%3Cpath%20fill%3D%22%20000002%22%20d%3D%22M287%2069.4a17.6%2017.6%200%200%200-13-5.4H18.4c-5%200-9.3%201.8-12.9%205.4A17.6%2017.6%200%200%200%200%2082.2c0%205%201.8%209.3%205.4%2012.9l128%20127.9c3.6%203.6%207.8%205.4%2012.8%205.4s9.2-1.8%2012.8-5.4L287%2095c3.5-3.5%205.4-7.8%205.4-12.8%200-5-1.9-9.2-5.5-12.8z%22%2F%3E%3C%2Fsvg%3E');
      background-position:  right 10px top 50%, 0, 0 ;
      background-size: 12px;
      background-repeat: no-repeat;
    }

    .currency input {
      border: 0;
      background: transparent;
      font-size: 30px;
      text-align: right;
    }

    .swap-rate-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .rate {
      color: var(--primary-color);
      font-size: 14px;
      padding: 0 10px;
    }

    select:focus,
    input:focus,
    button:focus {
      outline: 0;
    }

    @media (max-width: 600px) {
      .currency input {
        width: 200px;
      }
    }

  </style>
  </head>
  <body>
    <img src="img/money.png" alt="" class="money-img" />
    <h1>Exchange Rate Calculator</h1>
    <p>Choose the currency and the amounts to get the exchange rate</p>

    <div class="container">
      <div class="currency">
        <select id="currency-one">
          <option value="AUD">AUD</option>
          <option value="BGN">BGN</option>
          <option value="BRL">BRL</option>
          <option value="CAD">CAD</option>
          <option value="CHF">CHF</option>
          <option value="CNY">CNY</option>
          <option value="CZK">CZK</option>
          <option value="DKK">DKK</option>
          <option value="EUR" selected>EUR</option>
          <option value="GBP">GBP</option>
          <option value="HKD">HKD</option>
          <option value="HRK">HRK</option>
          <option value="HUF">HUF</option>
          <option value="IDR">IDR</option>
          <option value="ILS">ILS</option>
          <option value="INR">INR</option>
          <option value="ISK">ISK</option>
          <option value="JPY">JPY</option>
          <option value="KRW">KRW</option>
          <option value="MXN">MXN</option>
          <option value="MYR">MYR</option>
          <option value="NOK">NOK</option>
          <option value="NZD">NZD</option>
          <option value="PHP">PHP</option>
          <option value="PLN">PLN</option>
          <option value="RON">RON</option>
          <option value="RUB">RUB</option>
          <option value="SEK">SEK</option>
          <option value="SGD">SGD</option>
          <option value="THB">THB</option>
          <option value="TRY">TRY</option>
          <option value="USD">USD</option>
          <option value="ZAR">ZAR</option>
        </select>
        <input type="number" id="amount-one" placeholder="0" value="1" />
      </div>

      <div class="swap-rate-container">
        <button class="btn" id="change">Change</button>
        <div class="rate" id="rate"></div>
      </div>

      <div class="currency">
        <select id="currency-two">
          <option value="AUD">AUD</option>
          <option value="BGN">BGN</option>
          <option value="BRL">BRL</option>
          <option value="CAD">CAD</option>
          <option value="CHF">CHF</option>
          <option value="CNY">CNY</option>
          <option value="CZK">CZK</option>
          <option value="DKK">DKK</option>
          <option value="EUR" selected>EUR</option>
          <option value="GBP">GBP</option>
          <option value="HKD">HKD</option>
          <option value="HRK">HRK</option>
          <option value="HUF">HUF</option>
          <option value="IDR">IDR</option>
          <option value="ILS">ILS</option>
          <option value="INR">INR</option>
          <option value="ISK">ISK</option>
          <option value="JPY">JPY</option>
          <option value="KRW">KRW</option>
          <option value="MXN">MXN</option>
          <option value="MYR">MYR</option>
          <option value="NOK">NOK</option>
          <option value="NZD">NZD</option>
          <option value="PHP">PHP</option>
          <option value="PLN">PLN</option>
          <option value="RON">RON</option>
          <option value="RUB">RUB</option>
          <option value="SEK">SEK</option>
          <option value="SGD">SGD</option>
          <option value="THB">THB</option>
          <option value="TRY">TRY</option>
          <option value="USD" selected>USD</option>
          <option value="ZAR">ZAR</option>
        </select>
        <input type="number" id="amount-two" placeholder="0" />
      </div>
    </div>
    
  <script> 
    const currencyEl_one= document.getElementById('currency-one');
    const amountEl_one= document.getElementById('amount-one');
    const currencyEl_two= document.getElementById('currency-two');
    const amountEl_two= document.getElementById('amount-two');

    const rateEl = document.getElementById('rate');
    const swap= document.getElementById('swap');

    //Fetch exchange rates, updating DOM
    function calculate(){
        const curency_one = currencyEl_one.value
        const curency_two = currencyEl_two.value

        fetch(`https://api.exchangeratesapi.io/latest?base=${curency_one}`)

            .then(res=>res.json())
            .then(data=>{
                const rate= data.rates[curency_two];
                rateEl.innerHTML=`1 ${curency_one} = ${rate} ${curency_two} `
                amountEl_two.value = (amountEl_one.value * rate).toFixed(2)
            })        
    }
    //Events
    currencyEl_one.addEventListener('change', calculate);
    amountEl_one.addEventListener('input', calculate);
    currencyEl_two.addEventListener('change', calculate);
    amountEl_two.addEventListener('input', calculate);

    change.addEventListener('click', ()=>{
        temporary = currencyEl_one.value
        currencyEl_one.value = currencyEl_two.value;
        currencyEl_two.value= temporary 
        calculate()
    })

    calculate()
    
  </script>
  </body>
</html>
```
## Experience
You could take a look on some my works following the link bellow
[My portfolio link](https://liudmila-krystsinevich.000webhostapp.com/)

## Education
My highest degree is Master of Science in Supply chain Management at Cracow University of Economics, but also I would like to mention that I have been studying programming on my own more than a year and a half.

### Courses:
* School of Programming "Akademia 108"- Frond-end-developer course;
* "Programator" - Fullstack Developer - programming training course organized and financed by the EU (currently attedning);
* Udemy courses (Front-end, JS, React.js);
* Online books and reading official documentation;
* The Rolling Scopes course - as you know :) 

## English
I estamate my English level as B2. I have been practicing it at multinational corporation where I am currently working.



