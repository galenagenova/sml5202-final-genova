<h1> Reading Week Material </h1>
<!DOCTYPE html>
<html>
<body>
  
<h2> 'Random' short sentences with <em>JavaScript </em> </h2>

<button onclick="makeSentence()">Click me</button>

<p id="demo"></p>

<script>
  function makeSentence() {
  
  var person = {
      names: ["George", "Sam", "Alex", "Fiona", "Sally", "Jennifer", "Nickole", "Amanda", "Hector", "Alice", "Benjamin", "Jane", "Austin", "Amy", "Sandra", "He", "She", "Vincent", "Arthur" ],
      verbes: ["speaks", "eats", "runs", "reads", "writes" ],
      adverbs: ["slowly", "fast", "with_passion", "rarely", "a lot" ],
      
      };
  
  name = person.names[Math.floor(Math.random() * person.names.length)];
  verb = person.verbs[Math.floor(Math.radom() * person.verbs.length)];
  adverb = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];
  
  document.getElementById("demo").innerHTML = name + " " + verb + " " + adverb;
  }
  </script>
  
  
  
  </body>
  </html>
  
  
  <!DOCTYPE html>
<html>
<body>
  
  <h2> All names with random(ish) verbs and adverbs: </h2>
   <button onclick="makeSentence()">Display</button>
   
     
   <p id="demo"></p>
   
   <script>
   function makeSentence() {
  
   var person = {
      names: ["George", "Sam", "Alex", "Fiona", "Sally", "Jennifer", "Nickole", "Amanda", "Hector", "Alice", "Benjamin", "Jane", "Austin", "Amy", "Sandra", "He", "She", "Vincent", "Arthur" ],
      verbes: ["speaks", "eats", "runs", "reads", "writes" ],
      adverbs: ["slowly", "fast", "with_passion", "rarely", "a lot" ],
      
      };
  var i;
  var text = "";
  for (i=0; i<person.names.length; i++) {
  
    name = person.names[i];
    verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
    adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];
    
      text += name + " " verb + " " + adv + "<br>";
      
      document.getElementById("demo").innerHTML = text;
  }
  
 }
 </script>
 </body>
 </html>
 
  
