<script>
    export let pais;
    let p;
    const paises={
      "colombia":["Colombia", "Bogota", "51,52 millones", "peso colombianos", "1,142 millones de km²", "bandera_de_colombia.jpg"],
      "venezuela":["Venezuela", "Caracas", "28,2 millones","bolivar", "916,445 km²", "bandera_de_venezuela.jpg"],
      "ecuador":["Ecuador", "Quito", "17.8 millones", "dolar estado unidense", "256.370 km²", "flag_of_ecuador.svg.png"],
      "peru":["Peru", "Lima", "33,72 millones", "sol peruano", "1.285.215 km²", "bandera_de_peru.webp"],
      "brasil":["Brasil", "Brasili", "214,3 millones", "real brasileño","8,51 millones km²", "bandera_de_brasil.jpg"]
    }
    p = paises[pais];
  </script>
  
  <div class="main">
    <div class="col1">
      <img src="./src/assets/{p[5]}" alt="bandera_de_colombia" width="300" height="200">
    </div>
    <div class="col2">
      <div class="linea"> <strong>pais:</strong> {p[0]}</div>
      <div class="linea"> <strong>capital:</strong> {p[1]}</div>
      <div class="linea"> <strong>poblacion:</strong> {p[2]}</div>
      <div class="linea"> <strong>moneda:</strong> {p[3]}</div>
      <div class="linea"> <strong>extencion:</strong> {p[4]}</div>
    </div>
  </div>
  ²
  
  <style>
  
    .main{
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      grid-gap: 5px;
      grid-auto-rows: minmax(100px, auto);
      border-radius: 10px;
      border-style: solid;
      border-color: rgb(red, green, blue);
      border-width: 2px;
      margin: left;
      width: 600;
      box-shadow: 5px 5px 5px black;
      margin-right: 5px;
      margin-bottom: 10px;
    }
    .col1{
      grid-column: 1px;
      grid-row: 1px;
      margin: 5px;
      padding: 5px;
    }
    .col2{
      grid-column: 2;
      grid-row: 1;
      margin: 5px;
      padding: 5px;
      border-color: black;
      width: max-content;
    }
    strong{
      color: rgb(29, 129, 154);
      font-weight: bolder;
    }
    .linea{
      font-size: 20px;
      margin-bottom: 18px;
    }
  </style>