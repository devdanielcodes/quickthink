<template>

    <div class="categories">

            <div class="shine"><h1>Categories</h1></div>

      
      

      <div class="cards-container">
        <div class="row-one" >

          <div class="row-one-a">
            <div class="music cat" id="roww">
              <span><img src="../assets/images/music.svg" alt=""></span>
              <p>Music</p>
            </div> 

            <div class="game cat">
              <span><img src="../assets/images/game.svg" alt=""></span>
              <p>Games</p>
              </div>
          </div>

          <div class="row-one-b ">

            <div class="art cat">
              <span><img src="../assets/images/art.svg" alt=""></span>
              <p>Art</p>
              </div>

            <div class="books cat">
              <span><img src="../assets/images/books.svg" alt=""></span>
              <p>Books</p>
              </div>
          </div>

        </div>

        <div class="row-two">

          <div class="row-two-a">

            <div class="gadgets cat">
              <span><img src="../assets/images/gadgets.svg" alt=""></span>
              <p>Gadgets</p>
              </div>
              
            <div class="shopping cat">
              <span><img src="../assets/images/shopping.svg" alt=""></span>
              <p>Shopping</p>
              </div>

          </div>

          <div class="row-two-b">

            <div class="sports cat">
              <span><img src="../assets/images/sport.svg" alt=""></span>
              <p>Sports</p>
              </div>

            <div class="math cat">
              <span><img src="../assets/images/math.svg" alt=""></span>
              <p>Math</p>
              </div>

          </div>

        </div>

        <div class="row-three">

          <div class="row-three-a">

            <div class="gifts cat">
              <span><img src="../assets/images/gifts.svg" alt=""></span>
              <p>Gifts</p>
              </div>

            <div class="videography cat">
              <span><img src="../assets/images/videography.svg" alt=""></span>
              <p>videography</p>
              </div>
          </div>

          <div class="row-three-b">

            <div class="news cat">
              <span><img src="../assets/images/news.svg" alt=""></span>
              <p>News</p>
              </div>

            <div class="cars cat">
              <span><img src="../assets/images/cars.svg" alt=""></span>
              <p>Cars</p>
              </div>

          </div>

        </div>

        <form class="form" >
            <input class="btn btn-anim" type="button" value="Create New Category">
        </form>
          
      </div>

       <Newsletter></Newsletter>

 <Footer></Footer>


    </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  methods: {
    greet: () => {
    }
  }
}
</script>

  <style scoped>




.shine {
  padding: 100px  0;
  width:100%;
  background:#1C1046;
  z-index:0;
  position: relative;
   overflow: hidden;
   margin-bottom: 50px;
   font-family: 'DM sans';
}

/* text */
.shine h1 {
  color:#fff;
  left:50%;
  transform:translate(-50%,-50%);
  position: absolute;
  display: inline-block;
  font-family:'open sans',sans-serif;
  letter-spacing:-1px;
  font-weight:bold;
  top:50%;
  width: 100%;
  font-size: 50px;
  text-align: center;
}

/* Shine */
.shine::after {
	content:'';
  top:0;
	transform:translateX(100%);
	width:100%;
	height:220px;
	position: absolute;
	z-index:1;
	animation: slide 1s infinite;
	 
  /* 
  CSS Gradient - complete browser support from http://www.colorzilla.com/gradient-editor/ 
  */
  background: -moz-linear-gradient(left, rgba(255,255,255,0) 0%, rgba(255,255,255,0.8) 50%, rgba(128,186,232,0) 99%, rgba(125,185,232,0) 100%); /* FF3.6+ */
	background: -webkit-gradient(linear, left top, right top, color-stop(0%,rgba(255,255,255,0)), color-stop(50%,rgba(255,255,255,0.8)), color-stop(99%,rgba(128,186,232,0)), color-stop(100%,rgba(125,185,232,0))); /* Chrome,Safari4+ */
	background: -webkit-linear-gradient(left, rgba(255,255,255,0) 0%,rgba(255,255,255,0.8) 50%,rgba(128,186,232,0) 99%,rgba(125,185,232,0) 100%); /* Chrome10+,Safari5.1+ */
	background: -o-linear-gradient(left, rgba(255,255,255,0) 0%,rgba(255,255,255,0.8) 50%,rgba(128,186,232,0) 99%,rgba(125,185,232,0) 100%); /* Opera 11.10+ */
	background: -ms-linear-gradient(left, rgba(255,255,255,0) 0%,rgba(255,255,255,0.8) 50%,rgba(128,186,232,0) 99%,rgba(125,185,232,0) 100%); /* IE10+ */
	background: linear-gradient(to right, rgba(255,255,255,0) 0%,rgba(255,255,255,0.8) 50%,rgba(128,186,232,0) 99%,rgba(125,185,232,0) 100%); /* W3C */
	filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00ffffff', endColorstr='#007db9e8',GradientType=1 ); /* IE6-9 */
}

/* animation */

@keyframes slide {
	0% {transform:translateX(-100%);}
	100% {transform:translateX(100%);}
}











  header h1{
  animation:aa  2s 0s 1 forwards;
  }
  @keyframes aa {
    from{
      opacity: 0;
    }
    to{
      opacity: 1;
    }
  }
   .cat{
     position: relative;
     cursor: pointer;

   }
  header {
    background-color: #1c1046;
  }

  header h1 {
    color: #fff;
    padding: 60px 0px;
    text-align: center;
    font-weight: bold;
    font-size: 50px;
    font-family: 'DM sans';
  }

  /* header:after {
    position: absolute;
    width: 100%;
    content:'';
    top:0;
    z-index: 20;
    animation: slide 1s infinite;
    background: linear-gradient(left, rgba(255,255,255,0) 0%, rgba(255,255,255,0.8) 50%, rgba(128,186,232,0) 99%, rgba(125,185,232,0) 100%);
    transform: translateX(100%);
  }

    @keyframes slide {
    0% {transform:translateX(-100%);}
    100% {transform:translateX(100%);}
  } */
.cards-container {
    display: grid;
    place-items: center;
    padding-top: 100px;
    position: relative;
  }
  
  .cards-container img {
    padding: 40px;
  }
  .row-one, .row-one-a, .row-one-b, .row-two, .row-two-a, .row-two-b, .row-three, .row-three-a, .row-three-b {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    text-align: center;
    font-family: 'DM sans';
    font-weight: bold;
    font-size: 21px;
    align-items: baseline;
    justify-content: center;
  }

  .row-one, .row-two, .row-three {
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    transition: 1s all;
  }

  .row-two, .row-three {
    margin-top: 70px;
  }

  span img {
    width: 200px;
    height: 170px;
  }

  .cards-container p {
    padding: 15px 0px 16px 0px;
  }
  .music{
    position: relative;
  }
  .music img {
    background-color: #ff4d55;
    border-radius: 8px 8px 0px 0px;
  }

  .game img {
    background-color: #ABAE03;
    border-radius: 8px 8px 0px 0px;
  }

  .art img {
    background-color: #00B704;
    border-radius: 8px 8px 0px 0px;
  }

  .books img {
    background-color: #574E76;
    border-radius: 8px 8px 0px 0px;
  }

  .gadgets img {
    background-color: #ff4da2;
    border-radius: 8px 8px 0px 0px;
  }

  .shopping img {
    background-color: #ab40ff;
    border-radius: 8px 8px 0px 0px;
  }

  .sports img {
    background-color: #ff9800;
    border-radius: 8px 8px 0px 0px;
  }

  .math img {
    background-color: #006484;
    border-radius: 8px 8px 0px 0px;
  }

  .gifts img {
    background-color: #4c4c4c;
    border-radius: 8px 8px 0px 0px;
  }

  .videography img {
    background-color: #04172a;
    border-radius: 8px 8px 0px 0px;
  }

  .news img {
    background-color: #18c5d9;
    border-radius: 8px 8px 0px 0px;
  }

  .cars img {
    background-color: #351a0a;
    border-radius: 8px 8px 0px 0px;
  }

  .music, .game, .art, .books, .gadgets, .shopping, .sports, .math, .gifts, .videography, .news, .cars {
    box-shadow: 0px 8px 20px rgba(28, 16, 70, 0.12);
    border-radius: 8px;
    margin-top: 20px;
    margin-right: 20px;
  }


.form {
  margin-top: 70px;
  margin-bottom: 100px;
}

.btn{
  width: 100%;
  padding: 20px;

  background: #18C5D9;
  color: rgb(255, 255, 255);
  outline: none;
  border: none;
  margin-top: 30px;
  cursor: pointer;
  border-radius: 8px;
  font-size: 20px;
  transition: all .5s;
}
.btn:hover{
  transform: rotate(-4deg);
}
  @media only screen and (max-width: 550px){
     .shine{
    padding: 60px;
  }
    .shine h1 {
      font-size: 30px ;
    }

    
  }

  </style>