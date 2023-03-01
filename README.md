<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
    <title>CV</title>
    <style>
        .container{
            display:flex;
        }
        .right-column {
        width: 66.66%;
        padding: 10px;
      }
      .left-column{
        width:33,33%;
        padding:10px;
      }
      .hidden{
        display:none;
        border: solid black 1px;
      }
      .button-container {
  float: left;
  width: 50%;
  
}
    .info-button {
  display: block;
  margin: 10px 0;
  
}
    .info-box {
    display: none;
  float: left;
  width: 50%;
  padding: 10px;
  box-sizing: border-box;
  
}
        
      
    </style>
</head>
<body style="margin:10px;padding:30px">
 <div class="container">
    <div class="left-column" style="background-color: aquamarine;border:solid white 20px">
        <div style="margin:5px;padding:20px;padding-top:70px">
            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="No aparece la foto"/>
        </div>
        <div style="margin:5px;padding:20px;padding-top:70px">
            Jeanne Steeves
        </div>
        <div style="margin:5px;padding:20px;padding-top:70px">
            United States
        </div>
        <div style="margin:5px;padding:20px;padding-top:70px">
            Michigan
        </div>
        <div style="margin:5px;padding:20px;padding-top:70px">
            4193 Royal Ln
        </div>
        <div style="margin:5px;padding:20px;padding-top:70px">
    <!--contacto-->
    <div id="button-container">
       

        <button id="info-button">Contacto</button>
      </div>
       
      <div id="info-box">
        <p id=contac class="hidden">e-mail:
            jeanne.steeves@example.com</p>
        <p id="contac2" class="hidden">Telefono:
            (894) 759-5810</p>
      </div>
      
            </div>

    
    </div>
    
    <div class="right-column" style="border-bottom: 3px dotted black;"> 
        <div>
            <h2 style="border-bottom: 1px dashed black;padding:10px">Formación academica:</h2>
            <p>
                <h4>
                    Primaria:
                </h4>
                <h4>
                    Secundaria:
                </h4>
                
                <br>
                <button id="button1">Estudios universitarios:</button>
            </p>
            <br>
            <h4 id="additional-info1" class="hidden">
                Ingenieria Mecanica:
            </h4>
            <p id="additional-info6" class="hidden">
                Universidad de Rosario (FCEIA) ingreso...
            </p>
        </div>
        <div>
            <h2 style="border-bottom: 1px dashed black;padding:10px;">
                Idiomas:
            </h2>
            <p>
                <h4>
                    Ingles: 
                    
                </h4>
                <p>certificado FCE...</p>
                <h4>
                    Frances:
                </h4>
                <p> certificado...</p>
                <br>
                <button id="button2">Conocimiento Informal:</button>
            </p>
            <h4 id="additional-info2" class="hidden"> 
                Aleman:
            </h4>
            <p id="additional-info5" class="hidden">
                 Estadia en alemania...
                </p>
                <h4 id="additional-info7" class="hidden"> 
                    Italiano:...
                </h4>
                
            
        </div>
        <div>
            <h2 style="border-bottom: 1px dashed black;padding:10px;">
                Experiencia Laboral:
            </h2>
            <p>
                10 años trabajando en ... <br>
                5 años trabajando como...
                <br>
                <button id="button3">Experiencia de menor duracion</button>
            </p>
            <p id="additional-info3" class="hidden">
                5 meses trabajando de mesero en... <br>
                1 año trabajando en...
            </p>
        </div>
        <div>
            <h2 style="border-bottom: 1px dashed black;padding:10px;">
                Otras habilidadaes:
            </h2>
            <p>
                Gran habilidad con software... 
                 <br>
                Programacion en lenguaje... <br>

                <br>
                <button id="button4">
                    Mas Informacion
                </button>
            </p>
            <p id="additional-info4" class="hidden">Buen manejo de herramienta... <br>
                Carnet de conducir categoria...<br></p>
        </div>
    </div>
</div>
    </div>
    <script>
        const button1 = document.getElementById('button1');
        const additionalinfo1 = document.getElementById('additional-info1');
        const additionalinfo6 = document.getElementById('additional-info6');
        button1.addEventListener('click', function() {
          additionalinfo1.classList.toggle('hidden');
          additionalinfo6.classList.toggle('hidden');
        });
        </script>
        <script>
        const button2 = document.getElementById('button2');
        const additionalInfo2 = document.getElementById('additional-info2');
        const additionalInfo5 = document.getElementById('additional-info5');
        const additionalInfo7 = document.getElementById('additional-info7');
        button2.addEventListener('click', function() {
          additionalInfo2.classList.toggle('hidden');
          additionalInfo5.classList.toggle('hidden');
          additionalInfo7.classList.toggle('hidden');
        });
        </script>
        <script>
        const button3 = document.getElementById('button3');
        const additionalInfo3 = document.getElementById('additional-info3');
        button3.addEventListener('click', function() {
          additionalInfo3.classList.toggle('hidden');
        });</script>
        <script>
        const button4 = document.getElementById('button4');
        const additionalInfo4 = document.getElementById('additional-info4');
        button4.addEventListener('click', function() {
          additionalInfo4.classList.toggle('hidden');
        });
      </script>
      <script>
        const botcont= document.getElementById('info-button');
        const contac = document.getElementById('contac');
        const contac2 = document.getElementById('contac2');
        botcont.addEventListener('click', function() {
          contac.classList.toggle('hidden');
          contac2.classList.toggle('hidden');
        });
        </script>
</body>
</html>
