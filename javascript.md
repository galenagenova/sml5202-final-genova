<button type="button" class="new-quote button">Show sentance</button>
 <dl id="quote"></dl>


  
  
<script>
 
const endpoint = 'https://galenagenova.github.io/SML5202-galena/datasets/idioms.json';

function getQuote() {
fetch(endpoint)
.then(function (response) {
return response.json();
})
.then(function(data){
let id = Math.floor(Math.random() * 7);
let idiom = (data.idioms[id].idiom);
let meaning = (data.idioms[id].meaning);
let example = (data.idioms[id].example);

document.querySelector("#quote").innerHTML = "<dt>" + idiom + "</dt>" + "<dd><strong>Example:</strong> " + example + "</dd><dd><strong>Meaning:</strong> " + meaning + "</dd>" ;

//console.log(data.idioms[id].idiom)
})
.catch(function () {
console.log("Error occurred");
});
}

const newQuoteButton = document.querySelector('.new-quote');
newQuoteButton.addEventListener('click', getQuote);

</script>

<br>
<hr>
For this practice we used this 
<a href="https://www.w3schools.com/html/tryit.asp?filename=tryhtml_default">page</a>
