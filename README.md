# Research
A research repository


<body>
  <input type="text" id="input" value="" placeholder="choice
  a number 1 to 5">
  <button id="cf">Confirm</button>
</body>


<script type="text/javascript">

  function RandomNum(x,y){    //This is a random number function used to generate a random number.
      return Math.round(Math.random()*(y-x)+x); //This formula was found through an online search, but the specific principles behind it are unclear.
    }
  let result = RandomNum(1,5); //This code is used to retrieve the result number using the previous function when the page is loaded.

  document.getElementById("cf").addEventListener("click",function(){ //This is adding an event listener to the confirm button.
    let input = document.getElementById("input").value; //After clicking, it retrieves the numerical value entered by the user.
    if (input==result){  //This code is used to verify if the user input matches the result. If the input is correct, it will trigger the following alert.
      alert("Yes, you r right. Refresh page and play again");
    }
    else{ alert("Wrong,type again");} //This code is the content that will be displayed if the input is incorrect.
     
    console.log(result); //This is the correct result that can be seen in the browser console, which can be considered as a cheating feature.
  })
      






</script>
