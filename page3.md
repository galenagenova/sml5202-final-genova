<h1> App Language (texting and social media dictionary) </h1>
 <p>
<br>
  <table>
    <tr> <th> Будем: </th> <th> бум </th> <td> We will be </td> </tr>
    <tr> <td> Вообще: </td> <td> ваще </td> <td> Not at all </td> </tr>
    <tr> <td> Естественно: </td> <td> ессно </td> <td> Naturally/Of course </td> </tr> 
    <tr> <td> Завтра: </td> <td> звтр </td> <td> tomorrow </td> </tr>
    <tr> <th> Интересно: </th> <th> интрс </th> <td> Interesting </td> </tr>
    <tr> <td> Кто-нибудь: </td> <td>  кто-нить </td> <td> Whoever </td> </tr>
    <tr> <td> Ладно: </td> <td> лана, лан </td> <td> Sure </td> </tr> 
    <tr> <td> Может быть: </td> <td> мб </td> <td> Maybe </td> </tr> 
    <tr> <th> Нормально: </th> <th> норм </th> <td> Normal/As usual </td> </tr>
    <tr> <td> Опять: </td> <td> о5 </td> <td> Again </td> </tr>
    <tr> <td> Почему: </td> <td> пчм </td> <td> Why </td> </tr> 
    <tr> <td> Смотри: </td> <td> см </td> <td> Look </td> </tr> 
    <tr> <th> Только: </th> <th> тока </th> <td> Only </td> </tr>
    <tr> <td> Хорошо: </td> <td> хор, оч хор </td> <td> Good </td> </tr>
    <tr> <td> Целую: </td> <td> чмок, кисс </td> <td> Kisses </td> </tr> 
    <tr> <td> Я считаю: </td> <td> я щетаю </td> <td> I consider </td> </tr> 
  </table>
  <br> 
  </p>
 
 <hr>
 <a href="https://cdni.rbth.com/rbthmedia/images/2019.10/original/5d9326fe15e9f90b3365e222.jpg" title="View Full Size">
<img
src="https://cdni.rbth.com/rbthmedia/images/2019.10/original/5d9326fe15e9f90b3365e222.jpg">
</a>
 <hr>
 
 <h1>Common slang words and phrases</h1>


<button type="button" class="new-quote button">Show sentance</button>
 <dl id="quote"></dl>


  
  
<script>
 
const endpoint = 'https://github.com/galenagenova/sml5202-final-genova/blob/master/datasets/idioms.json';

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
If you would like to practice you can follow the lik to our 
<a href="https://galenagenova.github.io/sml5202-final-genova/page5.html">exercises</a>.
<hr>
    
 
