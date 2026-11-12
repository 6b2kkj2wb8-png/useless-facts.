
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Useless Facts</title>
<style>
body {
  background: #10131a;
  color: white;
  font-family: Arial, sans-serif;
  text-align: center;
  padding: 100px 20px;
}
h1 { font-size: 48px; }
p { color: #aaa; }
button {
  padding: 15px 25px;
  border: none;
  border-radius: 20px;
  background: #9b8cff;
  cursor: pointer;
  font-weight: bold;
}
</style>
</head>
<body>

<h1>Useless Facts</h1>
<p>Facts you probably didn't need to know.</p>

<h2 id="fact">Click for a random fact.</h2>

<button onclick="newFact()">Another fact</button>

<script>
const facts = [
"Octopuses have three hearts.",
"Wombat poop is cube-shaped.",
"A day on Venus is longer than its year.",
"Bananas are berries.",
"Flamingos are naturally pink.",
"Some turtles can breathe through their backsides.",
"The Eiffel Tower gets taller in summer.",
"The dot on an i is called a tittle."
];

function newFact() {
 const random = Math.floor(Math.random() * facts.length);
 document.getElementById("fact").innerText = facts[random];
}
</script>

</body>
</html>
