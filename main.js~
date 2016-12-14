var myHeading = document.querySelector('h1');
var pElement = document.querySelector('p');
myHeading.textContent = 'Hello Mohammed!';
alert('hello!');

function multiply(num1,num2) {
  var result = num1 * num2;
  return result;
}

function calculator(){
   firstNum = prompt('Enter first number');
   secondNum = prompt('Enter second number');
   myHeading.textContent = firstNum + 'X' + secondNum + '=' + multiply(firstNum,secondNum);
  // myHeading.textContent='hello';
}

document.querySelector('html').onclick = function(){  
  calculator();
}


var myButton = document.querySelector('button');

function setUserName() {
  var myName = prompt('Please enter your name.');
  localStorage.setItem('name', myName);
  pElement.textContent = myName;
}

if(!localStorage.getItem('name')) {
  setUserName();
} else {
  var storedName = localStorage.getItem('name');
 pElement.textContent = storedName;
}

myButton.onclick = function() {
  setUserName();
}

var qrcode = new QRCode(document.getElementById("qrcode"), {
	width : 100,
	height : 100
});

function makeCode () {		
	var elText = document.getElementById("text");
	
	if (!elText.value) {
		alert("Input a text");
		elText.focus();
		return;
	}
	
	qrcode.makeCode(elText.value);
	console.log(elText.value);
}


var QRButton = document.getElementById('qrcodebutton');

QRButton.onclick = function(){
	makeCode();
}
