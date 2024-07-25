<template>
  <div class="body">
    <div class="main">
      <img src="../src/assets/image-omelette.jpeg" alt="simple omelet">
      <div class="elements">
        <h1>
        Simple Omelette Recipe
      </h1>
      <p>
        An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs cooked 
        to perfection, optionally filled with your choice of cheese, vegetables, or meats.
      </p>
      <div class="prep">
        <h3>
          Preparation time
        </h3>
        <ul>
          <li>Total: 
            <p>Approximately 10 minutes</p>
          </li>
          <li>Preparation: 
            <p>5 minutes</p>
          </li>
          <li>Cooking: 
            <p>5 minutes</p>
          </li>
        </ul>
      </div>
      <h2>
        Ingredients
      </h2>
      <ul>
        <li>2-3 large eggs</li>
        <li>Salt, to taste</li>
        <li>Pepper, to taste</li>
        <li>1 tablespoon of butter or oil</li>
        <li>Optional fillings: cheese, diced vegetables, cooked meats, herbs</li>
      </ul>
      <div class="instructions">
        <h2>
        Instructions
        </h2>
        <ol>
          <li>Beat the eggs: 
            <p>In a bowl, beat the eggs with a pinch of salt and pepper until they are well mixed. 
            You can add a tablespoon of water or milk for a fluffier texture.</p>
          </li>
          <li>Heat the pan: 
            <p>Place a non-stick frying pan over medium heat and add butter or oil.</p>
          </li>
          <li>Cook the omelette: 
            <p>Once the butter is melted and bubbling, pour in the eggs. Tilt the pan to ensure 
            the eggs evenly coat the surface.</p>
          </li>
          <li>Add fillings (optional): 
            <p>When the eggs begin to set at the edges but are still slightly runny in the 
            middle, sprinkle your chosen fillings over one half of the omelette.</p>
          </li>
          <li>Fold and serve: 
            <p>As the omelette continues to cook, carefully lift one edge and fold it over the 
            fillings. Let it cook for another minute, then slide it onto a plate.</p>
          </li>
          <li>Enjoy: 
            <p>Serve hot, with additional salt and pepper if needed.</p>
          </li>
        </ol>
      </div>
      <h2>
        Nutrition
      </h2>
      <p>
        The table below shows nutritional values per serving without the additional fillings.
      </p>
      <ul class="nutrients">
        <li>Calories</li>
        <li>277kcal</li>
        <li>Carbs</li>
        <li>0g</li>
        <li>Protein</li>
        <li>20g</li>
        <li>Fat</li>
        <li>22g</li>
      </ul>
      </div>
    </div>
  </div>
</template>

<script>


</script>

<style>
.attribution{
  font-size: 11px;
  text-align: center;
}

.attribution a {
  color: hsl(228, 45%, 44%); 
}

/*fonts*/
@font-face {
  font-family: young-serif;
  src: url('../src/fonts/young-serif/YoungSerif-Regular.ttf');
}

@font-face {
  font-family: outfit-regular;
  src: url('../src/fonts/outfit/static/Outfit-Regular.ttf');
}

@font-face {
  font-family: outfit-bold;
  src: url('../src/fonts/outfit/static/Outfit-Bold.ttf');
}

/*eigen styling*/
/*doe de grid voor de ul laatste met n-thchild(odd) of even*/

li p{
  display: inline;
}

body{
  width: 900px;
  padding: 10rem 0 10rem 0;
  margin-left: auto;
  margin-right: auto;
  background-color: #F3E5D8;
  font-family: outfit-regular;
}

.body{
  background-color: #FFFFFF;
  max-width: 900px;
  padding-bottom: 50px;
  padding-top: 50px;
  border-radius: 2rem;
}

.main{
  background-color: #FFFFFF;
  padding: 500 px;
  max-width: 800px;
  margin: 0 auto;
}

.prep{
  background-color: #FFF7FC;
  padding: 2rem;
  border-radius: 0.5rem;
}

.nutrients{
  list-style-type: none;
}

.nutrients li {
  border-bottom: 1px solid black;
  padding-top: .75rem;
  padding-bottom: .75rem;
}

.nutrients li:last-child, .nutrients li:nth-child(7){
  border-bottom: 0px;
}

h1, h2 {
  font-family: young-serif;
  font-weight: 600;
}

h1{
  color: #2E2E2D;
}

h2, li, p{
  color: #834832;
}

h3{
  color: #723F54;
}

.instructions{
  border-top: 1px solid black;
  border-bottom: 1px solid black;
}

ol li, .prep ul li{
  font-family: outfit-bold;
}

ol li p, .prep ul li p{
  font-family: outfit-regular;
}

li{
  padding: 0 0 1rem 2rem;
}

li::marker {
  margin-right: 100px;
}

.nutrients{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(4, 1fr);
  padding: 0;
}

.main img{
  max-width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
  border-radius: 1rem;
}

@media (max-width:700px){
  body{
    width: 100%;
    padding: 0rem;
    margin: 0rem;
  }

  .main img{
  border-radius: 0rem;
  }

  .body{
    border-radius: 0rem;
    padding: 0rem;
  }

  .elements{
    padding: 2rem 4rem 4rem 4rem;
  }
}
</style>