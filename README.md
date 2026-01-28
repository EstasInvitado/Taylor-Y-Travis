
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <!-- Metadatos Open Graph -->
    <meta property="og:title" content="¡Estás invitado a nuestra boda ❤️! Taylor & Travis">
    <meta property="og:description" content="¡Boda Taylor y Travis! Mira todos los detalles aquí.">
    <meta property="og:image" content="https://github.com/EstasInvitado/Taylor-Travis/blob/main/portada.PNG?raw=true">
    <meta property="og:url" content="https://EstasInvitado.github.io/Taylor-Travis/">

    <title>Invitación de Boda — Taylor & Travis</title>

    <!-- Carga de la fuente Ballet desde Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Style+Script&display=swap" rel="stylesheet">
    <!-- Importa algunas fuentes de ejemplo de la categoría "Fancy" -->
    <link href="https://fonts.googleapis.com/css2?family=Fleur+De+Leah&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Mea+Culpa&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Fleur+De+Leah&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Castoro+Titling&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Gwendolyn&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Yrsa&display=swap" rel="stylesheet">

    <link href="https://fonts.googleapis.com/css2?family=Hi-Melody&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Grey+Qo&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Ballet:opsz@16..72&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Monsieur+La+Doulaise&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Luxurious+Script&display=swap" rel="stylesheet">


    <!-- Importar fuente Italianno desde Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Italianno&display=swap" rel="stylesheet">

    <!-- Puedes agregar más fuentes de Google Fonts si lo deseas -->

    <style>
        :root {
            /* Paleta neutra */
            
            
            --ink: #2b2b2b;
           
            --line: #d8d4cf;

            /* Imágenes: cámbialas por las tuyas */
            --hero: url('https://github.com/EstasInvitado/Taylor-Travis/blob/main/portada.PNG?raw=true');
            --img1: url('https://raw.githubusercontent.com/nellyaldana/Nelly-y-samuel/refs/heads/main/img13.png');
            --img2: url('https://github.com/nellyaldana/Nelly-y-samuel/blob/main/flores5.jpg?raw=true');
            
            --foto1: url('https://github.com/EstasInvitado/Taylor-Travis/blob/main/foto1.PNG?raw=true');
            --foto2: url('https://github.com/EstasInvitado/Taylor-Travis/blob/main/pareja4.png?raw=true');
            --foto3: url('https://github.com/EstasInvitado/Taylor-Travis/blob/main/pareja5.png?raw=true');

            --line-gap: 80px;
            /*linea imaginaria util para acomodar el itinerario, espacio total alrededor de la línea */


        }
        
        
 body {
            height: 100%
            margin: 0;
        }
        
  /* CONTENIDO DE PORTADA */      
.fondo {
  position: relative;
  height: 100vh;
  background-image: var(--foto2);
  background-size: cover;
  background-position: center;
}

.fondo::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.2); /* 0.5 = traslucidez */
}

.contenido {
  text-align: center;
  color: white;
  
}

/* TÍTULO */
.titulo {
  font-family: 'Ballet';
  font-size: 2rem;
  margin-top: 5.3vh; /* ← aquí está el 0.53 */
  margin-bottom: 18rem;
}

/* CONTENEDOR DE NOMBRES */
.nombres {
  margin-top: 2rem; /* dos renglones de separación */
    position: relative;
  width: 320px;      /* controla el diseño */
  margin: 3rem auto; /* centra el bloque completo */
  
}

/* CADA PALABRA EN SU PROPIO RENGLÓN */
.nombre {
  display: block;
  font-size: 2.5rem;
  margin: 1rem 0; /* brinco entre palabras */
}

.taylor,
.travis {
  letter-spacing: 0.18em;
}

/* TAYLOR A LA IZQUIERDA */
.taylor {
  font-family: 'Castoro Titling', serif;
  font-size: 2.5rem;
  text-align: left;
  
}

/* TRAVIS A LA DERECHA */
.travis {
  font-family: 'Castoro Titling', serif;
  font-size: 2.5rem;
  text-align: right;
}

/* ESPACIOS VERTICALES */
.taylor {
  margin-bottom: 3.8rem;
  animation: taylorIn 8s cubic-bezier(.22,.61,.36,1) 0.2s forwards;
}

.travis {
  margin-top: 4.8rem;
  animation: travisIn 7s cubic-bezier(.22,.61,.36,1) 0.4s forwards;
}

/* Y PERFECTAMENTE CENTRADA */
.y {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

  font-family: 'Monsieur La Doulaise', cursive;
  font-size: 4rem;
  animation: yIn 1s cubic-bezier(.22,.61,.36,1) 0.6s forwards;
}
@keyframes taylorIn {
  from {
    transform: translateX(-50px);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

@keyframes travisIn {
  from {
    transform: translateX(50px);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

@keyframes yIn {
  from {
    transform: translate(-50%, -20%);
    opacity: 0;
  }
  to {
    transform: translate(-50%, -50%);
    opacity: 1;
  }
}



.music-player {
  position: absolute;
  bottom: 40px; /* ajusta para que quede arriba del scroll */
  left: 50%;
  transform: translateX(-50%);
  width: 90%;
  text-align: center;
}

.music-player audio {
  width: 100%;
}
.play-btn {
  background: transparent;
  border: 2px solid #fff;
  color: #fff;
  padding: 10px 20px;
  border-radius: 50px;
  cursor: pointer;
  font-weight: bold;
}
       
       

       

        
        /* Flecha scroll */
        .scroll-indicator {
            position: absolute;
            bottom: 8px;
            left: 50%;
            width: 26px;
            height: 26px;
            border-bottom: 2px solid #fff;
            border-right: 2px solid #fff;
            transform: translate(-50%, 0) rotate(45deg);
            opacity: .2;
            animation: bounce 2.6s infinite;
        }

    
/*elementos de "agradecimeintos"*/
/* SECCIÓN BLANCA CON TEXTURA */
.agradecimientos {
  background: #FFF;
  padding: 120px 0 30px 0;;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* TEXTURA EN EL FONDO */
.agradecimientos::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background-image: url('textura.png'); /* Pon aquí tu textura */
  opacity: 0.12;
  pointer-events: none;
}

/* CONTENEDOR */
.contenedor-agradecimientos {
  text-align: center;
  position: relative;
  z-index: 2;
  max-width: 900px;
  padding: 0 20px;
}

/* TEXTO PRINCIPAL (Castoro Titling) */
.texto-principal {
  font-family: "Castoro Titling", serif;
  font-size: 15px;
  line-height: 1.6;
  margin: 0;
  
}

/* TEXTO SECUNDARIO (Ballet) */
.texto-secundario {
  font-family: "Ballet", serif;
  font-size: 36px;
  margin-top: 60px;  /* 3 renglones de separación */
  margin-bottom: 60px; /* separación hacia nombres */
}

/* NOMBRES DE PADRES (Castoro Titling) */
.nombres-padres {
  font-family: "Castoro Titling", serif;
  
font-style: italic; /* cursiva */
  font-size: 22px;
  line-height: 0.6; /* Para dar el brinco y doble brinco */
}
.nombres-padres p {
  font-family: "Castoro Titling", serif;

  font-style: italic;
  font-size: 22px;
  margin: 0;
}

/* Separación normal (1 brinco) */
.nombres-padres p.salto {
  margin-bottom: 20px;
}

/* Separación doble (2 brincos) */
.nombres-padres p.doble {
  margin-bottom: 40px;
}
   

/*elementos de "cuenta regresiva"*/

.cuenta-regresiva {
  background: #ffffff;
  padding: 60px 0; 
  display: flex;
  justify-content: center;
  align-items: center;
}

.contenedor-regresiva {
  text-align: center;
}

/* TITULO Save the Date (Ballet, delgado) */
.titulo-save {
  font-family: "Ballet", serif;
  font-size: 46px;
  font-weight: 300;   /* delgado */
  margin-bottom: 40px;
   letter-spacing: 0.1em;
}
.titulo-save::after {
  content: "";
  display: block;
  margin: 1px auto 0;
  width: calc(100% - 120px);
  height: 12px;               /* más alto = más curva */

  border-bottom: 2px solid #555;
  border-radius: 0 0 100% 100%;
}

/* CUADRO NEGRO CON EFECTO 3D Y MARCO */
.cuadro-contador {
  background: #000;
  border: 3px solid #fff;
  padding: 30px 40px;
  display: inline-block;
  box-shadow: 8px 8px 20px rgba(0,0,0,0.6),
              -4px -4px 12px rgba(255,255,255,0.2);
  transform: translateZ(0);
}

/* CONTADOR */
.contador {
  display: flex;
  gap: 45px;
}

/* CADA BLOQUE */
.bloque {
  text-align: center;
}

/* NUMEROS (Castoro Titling) */
.numero {
  font-family: "Castoro Titling", serif;
  font-size: 40px;
  color: #ffffff;
  margin: 0;
}

/* UNIDADES */
.unidad {
  font-family: "Castoro Titling", serif;
  font-size: 16px;
  color: #ffffff;
  margin: 0;
}

       
        /*ade aqui hasta donde dice cuenta regresiva estoy intentando poner la galeria de fotos si no funciona quitar esta parte */
/*elementos foto*/

 .foto {
            padding: 25px 22px;
             background-color: #F5F5F5; /* gris claro elegante */
            
        }
    

 .g {
            border-radius: 1px;
            padding-top: 100%;
            position: relative;
            overflow: hidden;
            
            transform: scale(.98);
            opacity: 0;
        }

        .g::before {
            content: "";
            position: absolute;
            inset: 0;
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            transition: transform .6s ease;
        }

        /*este es para que se abra la fotito del cuadrito que esta en el centro img1*/

        .g:hover::before {
            transform: scale(1.16);
        }

        /*este numero de scale sirve para el zoom en la foto*/
        .g.i1::before {
            content: "";
            position: absolute;
            inset: 0;
            /* ocupa todo el contenedor */
            background-image: var(--foto1);
            background-size: cover;
            /* muestra la imagen entera */
            background-repeat: no-repeat;
            /* sin repetir */
            background-position: center;
            /* centrado */
             filter: grayscale(100%); 
        }

        .g.i2::before {
            content: "";
            position: absolute;
            inset: 0;
            /* ocupa todo el contenedor */
            background-image: var(--foto2);
            background-size: cover;
            /* muestra la imagen entera */
            background-repeat: no-repeat;
            /* sin repetir */
            background-position: center;
            /* centrado */
             filter: grayscale(100%);
        }

        .g.i3::before {
            content: "";
            position: absolute;
            inset: 0;
            /* ocupa todo el contenedor */
            background-image: var(--foto3);
            background-size: cover;
            /* muestra la imagen entera */
            background-repeat: no-repeat;
            /* sin repetir */
            background-position: center;
            /* centrado */
             filter: grayscale(100%);
        }



      .details {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    width: min(1200px, 95%);
    margin: 0 auto;
}   
.section.alt {
            padding: 25px 22px;
            
        }
        
         .details .section.alt p:nth-of-type(1) {
            font-family: "Castoro Titling", serif;
            font-size: 13px;
            /* primera línea */
        }
        


        .section.alt1 {
            background-image: var(--img1);
        }
        .section.alt2 {
            padding: 25px 22px;
            background: var(--bg-3);
        }






/* estilo para la palabra Lugar */
#ubicaciones {
 
    margin-bottom: 2rem;
}

#ubicaciones .h {
    font-family: "Ballet", serif;
    font-style: italic;
     letter-spacing: 0.2em;
    font-weight: 300;
    font-size: 50px;         /* ajusta tamaño */
    text-align: right;       /* alineado a la derecha */
    position: relative;
    color: #000;             /* si tu fondo es negro */
    margin-right: 10px;      /* separacion de la derecha */
}

/* línea antes de la palabra */
#ubicaciones .h::before {
     content: "";
  position: absolute;
  left: 0;
  top: 50%;

  width: calc(100% - 190px);
  height: 1px;               /* más alto = más curva */

  border-bottom: 2px solid #555;
  border-radius: 0 0 100% 100%;
  
}



 .card {
    position: relative;
    font-size: 20px;
    text-align: center;
    width: min(800px, 85vw);
    background: #fff;
    border: 1px solid #cbbfb2;
    padding: 40px;
    box-shadow: 0 20px 28px rgba(0, 0, 0, .06);
    max-width: 800px;
    box-sizing: border-box; /* IMPORTANTE */
    padding: 30px;
    border: 14px solid #fff;
}

.card::before {
  content: "";
  position: absolute;
  inset: 10px;
  border: 2px solid #d3d3d3;

 }




        .card-img {
            width: 100%;
            /* ocupa todo el ancho de su contenedor */
            max-width: 80px;
            /* ancho máximo reducido */
            height: auto;
            /* mantiene proporción */
            display: block;
            margin: 0 auto 16px;
            /* centrada y con espacio debajo */
            border-radius: 8px;
            /* opcional */
        }

        .details .card p:nth-of-type(1) {
            font-family: "Castoro Titling", serif;
            font-size: 13px;
            /* primera línea */
        }

        .details .card p:nth-of-type(2) {
            font-family: "Yrsa", serif;
            font-size: 13px;
            /* segunda línea */
        }
         .details .card p:nth-of-type(3) {
            font-family: "Yrsa", serif;
            font-size: 13px;
            /* segunda línea */
        }

        .details .card a:nth-of-type(1) {
            font-family: "Yrsa", serif;
            font-size: 13px;
            /* segunda línea */
        }


        .card h3 {
            font-family: "Luxurous Script";
            margin: 0 0 8px;
            font-weight: 400;
        }

        .card2 p {
            margin: 6px 0;
            color: #4d4a45;
        }
       

        .btn {
            display: inline-block;
  margin-top: 12px;
  padding: 10px 20px;

  background: linear-gradient(180deg, #6f6f6f, #5a5a5a);
  color: #ffffff;

  border: 0px solid #4f4f4f;
  border-radius: 1px;

  text-decoration: none;
  font-weight: 300;
  letter-spacing: 0.05em;

box-shadow:
    0 4px 8px rgba(0, 0, 0, 0.25),   /* sombra principal */
    0 1px 2px rgba(255, 255, 255, 0.15); /* luz superior */

  transition:
    transform 0.2s ease,
    box-shadow 0.2s ease;
        }

        .btn:hover {
             background: linear-gradient(180deg, #7a7a7a, #646464);
  transform: translateY(-2px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.15);
        }

        .btn.whatsapp {
            font-family: 'Yrsa', cursive;
            background: #a6a6a6;
            border-color: #997E77
        }

        /* Itinerario */
        .timeline {
            border-left: 2px solid var(--line);
            margin: 8px auto 0;
            max-width: 680px;
            padding-left: 30px;
        }

        .step {
            font-family: 'Baskerville';
            font-size: 15px;
            position: relative;
            margin: 18px 0;
            transform: translateY(20px);
            opacity: 0;
        }

        .step::before {
            content: "";
            position: absolute;
            left: -20px;
            top: 6px;
            width: 12px;
            height: 12px;
            background: #fff;
            border: 2px solid #cbbfb2;
            border-radius: 50%;
        }

       
        }

        .photos {
            font-weight: 800;
            font-size: clamp(208px, 4.3vw, 50px);
            text-align: center;
            margin: 500px;
            font-family: 'Fleur de Leah', cursive;

        }

       

        .itinerary {
           max-width: 80px;
            margin: 5px auto;
            position: relative;
            /* ⬅️ CLAVE */
            font-family: 'Monsieur La Doulaise', sans-serif;
             font-size: 30px;
              padding-top: 7px;
            
        }
        .titulo-itinerario {
         display: inline-block;
         transform: translateX(-80%); /* ⬅️ mueve a la izquierda */
  
          font-family: 'Ballet', cursive;
          font-weight: 300;
          font-size: 3.5rem;
          letter-spacing: 0.1em;
          
          color: #555;
}
.titulo-itinerario::after {
  content: "";
  position: absolute;

  left: 100%;           /* empieza justo después de la palabra */
  top: 50%;
  transform: translateY(-50%);

  width: 230px;         /* largo de la línea */
  height: 1px;

  border-bottom: 2px solid #555;
  border-radius: 0 0 100% 100%;
  margin-left: 15px;    /* espacio entre texto y línea */
}


     
        /* Línea base */
        /* Línea base (gris) */
        .line {
            position: absolute;
            left: 50%;
            width: 4px;
            height: 80%;
            /* ⬅️ ya NO es 100% */
            background: #ddd;
            transform: translateX(-50%);
              top: 220px;
        }

       

        /* Línea activa (coloreada) */
        .line-progress {
            position: absolute;
            left: 50%;
            width: 4px;
            height: 60%;
            /* controlada por JS */
            background: #000;
            transform: translateX(-50%);
             top: 220px;
 
        }


        .event {
            display: grid;
            grid-template-columns: 1fr var(--line-gap) 1fr;
            align-items: center;
            margin: 10px -140%; /* con el primer numero manipulo la longitud de lo largo verticalmente hablando del itinerario (el largo de la ralla de en medio)con el segundo numero (%) este estoy moviendo la posicion del itinerario*/
            position: relative;
            gap: 105px
        }



        .event-content {
            min-width: 80px;
            font-family: 'Yrsa';
            font-size: 15px;
            text-align: right;
           
            padding: 40px 20px 60px;

        }

        .event h3 {
            margin: 0;
            color: #000;
        }

        .event p {
            margin: 5px 0 0;
            color: #555;
            font-family: 'Ballet';
             font-size: 25px;
             font-weight: bold;
        }

        /* Punto */
        .dot {
            position: absolute;
            left: 50%;
            width: 18px;
            height: 18px;
            background: #000;
            border-radius: 50%;
            transform: translate(-50%, 0);
            z-index: 2;
            transition: background 0.3s;
        }

        .event.active .dot {
            background: #555;
        }

#galeria .title {
    font-family: 'Ballet', cursive;
    font-size: 38px;          /* tamaño mediano */
    text-align: center;
   
    margin: 1em;          /* separación = 2 renglones aprox */
    line-height: 1.3;         /* buena separación entre líneas */
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    cursive;
  font-weight: 400;
  font-style: normal;
}
        /* Icono */
        .icon {
            width: 80px;
            height: 80px;
            object-fit: contain;
        }
        

/* contenido de REGALOS */

.regalos {
  display: flex;
  justify-content: center;
  padding: 6rem 1rem;
}

.tarjeta-regalo {
  background: #000;
  color: #fff;
  padding: 3.5rem 2.5rem;
  max-width: 420px;
  width: 100%;
  text-align: center;

  border-radius: 1px;

  /* EFECTO FLOTANTE */
  box-shadow:
    0 25px 50px rgba(0, 0, 0, 0.45),
    0 10px 20px rgba(0, 0, 0, 0.35);

  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.tarjeta-regalo:hover {
  transform: translateY(-6px);
  box-shadow:
    0 35px 60px rgba(0, 0, 0, 0.55),
    0 15px 30px rgba(0, 0, 0, 0.4);
}

/* TÍTULOS */
.titulo-regalo {
  font-family: 'Castoro Titling', serif;
  font-size: 1.8rem;
  letter-spacing: 0.12em;
  margin-bottom: 1rem;
}

.subtitulo-regalo {
  font-family: 'Ballet', cursive;
  font-size: 2.2rem;
  margin-bottom: 2.5rem;
}

/* ICONO */
.icono-sobre {
  width: 90px;
  margin: 0 auto 2rem;
  display: block;
  filter: invert(1); /* NEGATIVO → BLANCO */
}

/* ALTERNATIVA */
.alternativa {
  display: inline-block;
  font-family: 'Castoro Titling', serif;
  font-size: 0.85rem;
  letter-spacing: 0.15em;

  background: #e0e0e0;
  color: #000;

  padding: 0.4rem 1rem;
  border-radius: 0px;

  margin-bottom: 1.8rem;
}

/* CUENTA */
.cuenta {
  font-family: 'Castoro Titling', serif;
  font-size: 0.95rem;
  letter-spacing: 0.08em;
  margin-bottom: 0.5rem;
}

.numero-cuenta {
  font-family: 'Castoro Titling', serif;
  font-size: 1rem;
  letter-spacing: 0.15em;
}

  /* Contenido del Dress code */
  /* CONTENEDOR */
.dresscode {
  text-align: center;
  padding: 6rem 1rem;
  
}

/* TITULOS BALLET */
.titulo-ballet {
  font-family: 'Ballet', cursive;
  font-size: 3.8rem;
  margin-bottom: 2rem;
   font-weight: 300;
}

/* ICONOS */
.iconos-dresscode {
  display: flex;
  justify-content: center;
  gap: 2.5rem;
  margin-bottom: 1.5rem;
}

.iconos-dresscode img {
  width: 70px;
  opacity: 0.8;
}

/* TEXTO CASTORO */
.texto-dresscode {
  font-family: 'Castoro Titling', serif;
  letter-spacing: 0.18em;
  font-size: 1rem;
  margin-bottom: 3rem;
}

/* DELIMITADOR ELEGANTE */
.delimitador {
  width: 120px;
  height: 2px;
  margin: 3rem auto;

  background: linear-gradient(
    to right,
    transparent,
    #b8b8b8,
    transparent
  );
}

/* PALETA */
.paleta-colores {
  display: flex;
  justify-content: center;
  margin-top: 2.5rem;
}

/* CIRCULOS */
.color {
  width: 65px;
  height: 65px;
  border-radius: 50%;
  margin-left: -15px; /* TRASLAPE */

  box-shadow: 0 8px 15px rgba(0,0,0,0.15);
  border: 0px solid #fff;
}

/* COLORES NUDE */
.c1 { background: #111827; }
.c2 { background: #6b7280; }
.c3 { background: #9ca3af; }
.c4 { background: #1e3a8a; }
.c5 { background: #60a5fa; }
.c6 { background: #e0f2fe; }


        /* Footer */
       .footer {
  text-align: center;
  font-size: 14px;
  letter-spacing: 0.08em;
  color: #6b7280;
  margin: 80px 0 40px;
}

.footer strong {
  font-weight: 500;
  color: #1f2933;
}

.footer .heart {
  margin: 0 6px;
  opacity: 0.6;
}

.footer .date {
  display: block;
  margin-top: 8px;
  font-size: 12px;
  letter-spacing: 0.15em;
  color: #9ca3af;
}

        
        .titulo-castoro {
  font-family: 'Castoro Titling', serif;
  font-weight: 400;
  letter-spacing: 0.22em;   /* elegante, respirada */
  text-transform: uppercase;
  font-size: 2rem;
}


        /* ---------- Animaciones base + apariciones al hacer scroll ---------- */
        @keyframes fadeIn {
            from {
                opacity: 0
            }

            to {
                opacity: 1
            }
        }

        @keyframes fadeUp {
            from {
                opacity: 0;
                transform: translateY(18px)
            }

            to {
                opacity: 1;
                transform: none
            }
        }

        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-40px)
            }

            to {
                opacity: 1;
                transform: none
            }
        }

        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(40px)
            }

            to {
                opacity: 1;
                transform: none
            }
        }

        @keyframes revealUp {
            from {
                opacity: 0;
                transform: translateY(40px) scale(.98)
            }

            to {
                opacity: 1;
                transform: none
            }
        }

        @keyframes shimmer {

            0%,
            100% {
                opacity: 0;
                transform: translateX(-40%) rotate(8deg)
            }

            50% {
                opacity: .35;
                transform: translateX(40%) rotate(8deg)
            }
        }

        @keyframes bounce {

            0%,
            100% {
                transform: translate(-50%, 0) rotate(45deg);
            }

            50% {
                transform: translate(-50%, 6px) rotate(45deg);
            }
        }

        /* estado "visible" al scrollear */
        .reveal.in {
            animation: fadeUp 800ms ease forwards;
        }

        .reveal-delay-1.in {
            animation-delay: 80ms;
        }

        .reveal-delay-2.in {
            animation-delay: 160ms;
        }

        .reveal-delay-3.in {
            animation-delay: 240ms;
        }

        .reveal-1.in {
            animation: slideInLeft 800ms ease forwards;
        }


        /* Responsive */
        @media (max-width: 900px) {
            .details {
                grid-template-columns: 1fr;
            }

            .gallery {
                grid-template-columns: 1fr;
            }

            @media (max-width: 640px) {
                .strips {
                    grid-template-columns: 1fr 1.2fr 1fr;
                    gap: 10px;
                }

                .strip {
                    height: 58svh;
                }

                .countdown {
                    grid-template-columns: repeat(2, 1fr);
                }

                .timeline {
                    padding-left: 14px;
                }
            }

            @media (prefers-reduced-motion: reduce) {
                * {
                    animation: none !important;
                    transition: none !important
                }
            }


            /* Aquí pones la regla */
            img {
                border-radius: 0 !important;
            }
    </style>
</head>

<body>

    <!-- PORTADA:  -->
    <header class="fondo" id="inicio">
   <div class="contenido">
    <h1 class="titulo">Nuestra Boda</h1>

    <div class="nombres">
      <div class="taylor">TAYLOR</div>
      <div class="y">Y</div>
      <div class="travis">TRAVIS</div>
    </div>
  </div>
 <!-- REPRODUCTOR DE MÚSICA -->
  <div class="music-player">
    <audio controls>
      <source src="ruta-de-tu-cancion.mp3" type="audio/mpeg">
      Tu navegador no soporta audio.
    </audio>
  </div>
  <i class="scroll-indicator" aria-hidden="true"></i>
    </header>
    
<!-- agradecimientos-->
<section class="agradecimientos" id="agradecimientos">
  <div class="contenedor-agradecimientos">
    <p class="texto-principal">
      Nos haría inmensamente felices que nos acompañes al inicio de nuestra vida juntos
    </p>

    <p class="texto-secundario">
      Con la bendición de Dios y nuestros padres
    </p>

    <div class="nombres-padres">
      <p class="salto">Papa Taylor</p>
      <p class="salto doble">Mama Taylor</p>
      <p class="salto">Papa Travis</p>
      <p class="salto">Mama Travis</p>
    </div>
  </div>
</section>



 <!-- CUENTA REGRESIVA -->

<section class="cuenta-regresiva" id="cuenta-regresiva">
  <div class="contenedor-regresiva">
    <h2 class="titulo-save">Save  the  Date</h2>

    <div class="cuadro-contador">
      <div class="contador">
        <div class="bloque">
          <p class="numero" id="dias">00</p>
          <p class="unidad">Días</p>
        </div>
        <div class="bloque">
          <p class="numero" id="horas">00</p>
          <p class="unidad">Horas</p>
        </div>
        <div class="bloque">
          <p class="numero" id="minutos">00</p>
          <p class="unidad">Minutos</p>
        </div>
        <div class="bloque">
          <p class="numero" id="segundos">00</p>
          <p class="unidad">Segundos</p>
        </div>
      </div>
    </div>
  </div>
</section>

 

    <section class="foto" id="galeria">
        
            <div class="title">
                "El amor nos encontró…<br> y decidimos no soltarnos" </div>
            <div class="g i1 reveal"></div>
       

    </section>
   

    <!-- ubicaciones -->
    <section class="section alt" id="ubicaciones">
        <h2 class="h">Lugar</h2>
        <div class="details">
            <!-- ubicacion de la iglesia -->
            <article class="card reveal">
                <img src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/iglesia1.png?raw=true" alt="Iglesia" class="card-img">
                <h3>Ceremonia</h3>
                <p><strong>06:00 PM</strong> — Iglesia nuestro señor</p>
                <p>Amanecer, Terrazas de San Bernardo, La Cueva, 22525 Tijuana, B.C., México</p>
                <a class="btn" target="_blank" href="https://maps.app.goo.gl/FxHejANH9JJGKAsA7">Ver mapa</a>
            </article><br>
            <!-- ubicacion del salon -->
            <article class="card reveal">
                <img src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/disco.png?raw=true" alt="Iglesia" class="card-img">
                <h3>Recepción</h3>
                <p><strong>07:00 PM</strong> — Salon las palmas</p>
                <p>Amanecer, Terrazas de San Bernardo, La Cueva, 22525 Tijuana, B.C., México</p>
                <a class="btn" target="_blank" href="https://maps.app.goo.gl/FxHejANH9JJGKAsA7">Ver mapa</a>
            </article>
        </div>
    </section>

    <!-- foto 3 -->
    <section class="foto" id="galeria">
        <div class="memories reveal">
            <div class="g i2 reveal"></div>
        </div>

    </section>


    <!-- intento de itinerario -->
    <section class="itinerary">
<h2 class="titulo-itinerario">Itinerario</h2>
        
            <div class="line"></div>
            <div class="line-progress" id="lineProgress"></div>

            <!-- EVENTO 1 -->
            <div class="event">
                <div class="dot"></div>
                <div class="event-content">
                    <h3>5 pm</h3>
                    <p>Ceremonia</p>
                </div>
                <img class="icon" src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/iglesia.png?raw=true">
            </div>

            <!-- EVENTO 2 -->
            <div class="event">
                <div class="dot"></div>
                 <img class="icon" src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/copas.png?raw=true">
                <div class="event-content">
                    <h3>7 pm</h3>
                    <p>Recepcion</p>
                </div>
               
            </div>

            <!-- EVENTO 3 -->
            <div class="event">
                <div class="dot"></div>
                <div class="event-content">
                    <h3>8 pm</h3>
                    <p>Ramo</p>
                </div>
                <img class="icon" src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/ramo.png?raw=true">
            </div>

            <!-- EVENTO 4 -->
            <div class="event">
                <div class="dot"></div>
                <img class="icon" src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/plato.png?raw=true">
                <div class="event-content">
                    <h3>9 pm</h3>
                    <p>Cena</p>
                </div>
                
            </div>

            <!-- EVENTO 5 -->
            <div class="event end">
                <div class="dot"></div>
                <div class="event-content">
                    <h3>10 pm</h3>
                    <p>Baile</p>
                </div>
                <img class="icon" src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/vestido.png?raw=true">
            </div>
            
            
</div> 
    </section>
    <!-- aqui acaba de itinerario -->

    <!-- Regalos -->
   <section class="regalos">
  <div class="tarjeta-regalo">

    <h2 class="titulo-regalo">Sugerencia de regalo</h2>

    <p class="subtitulo-regalo">Lluvia de sobres</p>

    <img 
      src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/sobre.png?raw=true" 
      alt="Sobre"
      class="icono-sobre"
    />

    <span class="alternativa">Alternativa</span>

    <p class="cuenta">
      <strong>BBVA</strong> – Cuenta de banco
    </p>
    <p class="numero-cuenta">1234567890</p>

  </div>
</section>


    <!-- GALERÍA -->
    <!-- foto 3 -->
    <section class="foto" id="galeria">
        <div class="memories reveal">
            <div class="g i3 reveal"></div>
        </div>
    </section>

    
    <section class="dresscode">

  <!-- DRESS CODE -->
  <h2 class="titulo-ballet">Dress Code</h2>

  <div class="iconos-dresscode">
    <img src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/vestido.png?raw=true" alt="Vestido">
    <img src="https://github.com/EstasInvitado/Taylor-Travis/blob/main/smoking.png?raw=true" alt="Smoking">
  </div>

  <p class="texto-dresscode">Formal</p>

  <!-- DELIMITADOR ELEGANTE -->
  <div class="delimitador"></div>

  <!-- PALETA -->
  <h2 class="titulo-ballet">Paleta de colores</h2>

  <div class="paleta-colores">
    <span class="color c1"></span>
    <span class="color c2"></span>
    <span class="color c3"></span>
    <span class="color c4"></span>
    <span class="color c5"></span>
    <span class="color c6"></span>
  </div>

</section>

    <!-- accion de confirmacion -->

    <section class="container" id="confirmar" style="background:linear(#F2EFED, #F2EFED)">
        <div class="container reveal" style="text-align:center">
            <h2 class="titulo-castoro">¿Nos acompañas?</h2>
            <p class="sub reveal">Confirma tu asistencia antes del<br>
                <strong>1 de octubre de 2025</strong>.
            </p>

            <p>
                <a class="btn whatsapp" href="https://wa.me/526647629596?text=¡Hola!%20Confirmo%20mi%20asistencia%20a%20la%20boda%20de%20Nelly%20y%20Samuel" target="_blank" rel="noreferrer noopener">Confirmar por WhatsApp</a>
            </p>
        </div>
    </section>

   <footer class="footer">
  <span class="love">Con amor</span>
  <span class="heart">♥</span>
  <strong>Taylor & Travis</strong>
  <span class="date">15 · 10 · 26</span>
</footer>


    <script>
        
        
        /* --------- Apariciones al hacer scroll --------- */
        const revealEls = document.querySelectorAll('.photos, .hero-text, .h, .monogram, .reveal, .tile, .card, .step, .g, .btn');
        const io = new IntersectionObserver((entries) => {
            entries.forEach(e => {
                if (e.isIntersecting) {
                    e.target.classList.add('in');
                    io.unobserve(e.target);
                }
            });
        }, {
            threshold: .18
        });
        revealEls.forEach(el => io.observe(el));

        /* --------- Cuenta regresiva --------- */
       // Fecha objetivo: 25 de junio de 2026
  const fechaObjetivo = new Date("June 25, 2026 00:00:00").getTime();

  function actualizarCuenta() {
    const ahora = new Date().getTime();
    const distancia = fechaObjetivo - ahora;

    const dias = Math.floor(distancia / (1000 * 60 * 60 * 24));
    const horas = Math.floor((distancia % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutos = Math.floor((distancia % (1000 * 60 * 60)) / (1000 * 60));
    const segundos = Math.floor((distancia % (1000 * 60)) / 1000);

    document.getElementById("dias").innerText = String(dias).padStart(2, "0");
    document.getElementById("horas").innerText = String(horas).padStart(2, "0");
    document.getElementById("minutos").innerText = String(minutos).padStart(2, "0");
    document.getElementById("segundos").innerText = String(segundos).padStart(2, "0");
  }

  // Actualiza cada segundo
  setInterval(actualizarCuenta, 1000);
  actualizarCuenta();

        /* --------- RSVP por WhatsApp + localStorage --------- */
        const events = document.querySelectorAll('.event');
        const endEvent = document.querySelector('.event.end');
        const lineProgress = document.getElementById('lineProgress');
        const itinerary = document.querySelector('.itinerary');

        // Altura máxima permitida (hasta el punto del evento 5)
        const maxHeight =
          endEvent.offsetTop +
          endEvent.querySelector('.dot').offsetTop +
          endEvent.querySelector('.dot').offsetHeight / 2;


        window.addEventListener('scroll', () => {
            let scrollTop = window.scrollY + window.innerHeight * 0.4;
            let start = itinerary.offsetTop;

            let newHeight = scrollTop - start;

            // Limitar crecimiento de la línea
            if (newHeight < 0) newHeight = 0;
            if (newHeight > maxHeight) newHeight = maxHeight;

            lineProgress.style.height = newHeight + 'px';

            // Activar / desactivar puntos
            events.forEach(event => {
                const eventTop = itinerary.offsetTop + event.offsetTop;
                if (scrollTop >= eventTop) {
                    event.classList.add('active');
                } else {
                    event.classList.remove('active');
                }
            });
        });
    </script>
</body>

</html>
