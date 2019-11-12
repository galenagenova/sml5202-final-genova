<h1> Reading Week Material </h1>
<!DOCTYPE html>
<html>
<body>
  
<h2> 'Random' short sentences with <em>JavaScript </em> </h2>

<button onlick="makeSentence()"Click me</button>

<p id="demo"></p>

<script>
  function makeSentence() {
  var person = {
      names: ["George", "Sam", "Alex", "Fiona", "Sally", "Jennifer", "Nickole", "Amanda", "Hector", "Alice", "Benjamin", "Jane", "Austin", "Amy", "Sandra", "He", "She", "Vincent", "Arthur" ],
      verbes: ["speaks", "eats", "runs", "reads", "writes" ],
      adverbs: ["slowly", "fast", "with_passion", "rarely" ],
      };
  
  name = person.names[Math.floor(Math.random() * person.names.length)];
  verb = person.verbs[Math.floor(Math.radom() * person.verbs.length)];
  adverb = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];
  
  document.getElementById("demo").innerHTML = name + " " + verb + " " + adverb " ";
  }
  </script>
  
