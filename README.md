onEvent("button1", "click", function( ) {
  console.log("Next Screen Clicked");
  setScreen("screen2");
});
onEvent("button2", "click", function( ) {
  setNumber("Text", input + "");
  input = getNumber("Text");
});
var input ="0" ;
onEvent("Text", "change", function( ) {
  input = getNumber("Text");
});
onEvent("button3", "click", function( ) {
  setNumber("Text", input + "0");
  input = getNumber("Text");
});
onEvent("button7", "click", function( ) {
  setNumber("Text", input + "1");
  input = getNumber("Text");
});
onEvent("button8", "click", function( ) {
  setNumber("Text", input + "2");
  input = getNumber("Text");
});
onEvent("button9", "click", function( ) {
  setNumber("Text", input + "3");
  input = getNumber("Text");
});
onEvent("button10", "click", function( ) {
  setNumber("Text", input + "4");
  input = getNumber("Text");
});
onEvent("button11", "click", function( ) {
  setNumber("Text", input + "5");
  input = getNumber("Text");
});
onEvent("button12", "click", function( ) {
  setNumber("Text", input + "6");
  input = getNumber("Text");
});
onEvent("button13", "click", function( ) {
  setNumber("Text", input + "7");
  input = getNumber("Text");
});
onEvent("button14", "click", function( ) {
  setNumber("Text", input + "8");
  input = getNumber("Text");
});
onEvent("button15", "click", function( ) {
  setNumber("Text", input + "9");
  input = getNumber("Text");
});
onEvent("Add", "click", function( ) {
  var originalInput = input;
  setText("Text", 0);
  input = 0;
  onEvent("equals", "click", function( ) {
    input = input + originalInput;
    setText("Text", input);
  });
});
onEvent("Subtract", "click", function( ) {
  var originalInput = input;
  setText("Text", 0);
  input = 0;
  onEvent("equals", "click", function( ) {
    input = originalInput - input;
    setText("Text", input);
  });
});
onEvent("Multiply", "click", function( ) {
  var originalInput = input;
  setText("Text", 0);
  input = 0;
  onEvent("equals", "click", function( ) {
    input = input * originalInput;
    setText("Text", input);
  });
});
onEvent("divide", "click", function( ) {
  var originalInput = input;
  setText("Text", 0);
  input = 0;
  onEvent("equals", "click", function( ) {
    input = originalInput / input;
    setText("Text", input);
  });
});
