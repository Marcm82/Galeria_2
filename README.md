# Galeria_2
Galeria hecha con Javascript
- Queryselector
- Setattribute
- Addeventlistener

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    main{
        display: flex;
        padding: 10px;
        margin-bottom: 10px;
        gap: 10px;
        
    }
    .foto1,
    .foto2, 
    .foto3,
    .foto4 {
    width: 350px;
    border:1px solid #26ec03;
    margin-bottom: 10px;
    align-items: center;
    justify-content: center;
    }
    .gran{
        border:1px solid #26ec03;
        height: 100%;
    }
</style>
<body>
    <main>
        <section>
            <article class="foto1" id="sneaker1"><img src="IMG/sneaker_350_A.webp" width="85%"></article>
            <article class="foto2" id="sneaker2"><img src="IMG/sneaker_350_B.webp" width="85%"> </article>
            <article class="foto3" id="sneaker3"><img src="IMG/sneaker_350_C.webp" width="85%"> </article>
            <article class="foto4" id="sneaker4"><img src="IMG/sneaker_350_D.webp" width="85%"> </article>
        </section>
        <section>
            <article class="gran"><img src="IMG/sneaker_1200_A.webp"width="85%" id="contenidor"></article>
        </section>
    </main>
<script>
   let fotografia = document.querySelector("#sneaker1");
   let fotogran = document.getElementById("contenidor");
   function intercambia() {
    fotografia.setAttribute("src", "IMG/sneaker_1200_A.webp" )
   }
   fotografia.addEventListener("mouseover", this.intercambia);

   let fotografia2 = document.querySelector("#sneaker2");
  
   function intercambia() {
    fotografia2.setAttribute("src", "IMG/sneaker_1200_B.webp" )
   }
   fotografi2.addEventListener("mouseover", this.intercambia);

   let fotografia3 = document.querySelector("#sneaker3");
  
   function intercambia() {
    fotografia3.setAttribute("src", "IMG/sneaker_1200_C.webp" )
   }
   fotografia3.addEventListener("mouseover", this.intercambia);

   let fotografia4 = document.querySelector("#sneaker4");
   
   function intercambia() {
    fotografia4.setAttribute("src", "IMG/sneaker_1200_D.webp" )
   }
   fotografia4.addEventListener("mouseover", this.intercambia);
</script>
    
</body>
</html>
