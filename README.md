<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Karime ❤️</title>

<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:#111827;
    color:white;
    text-align:center;
}

.page{
    display:none;
    min-height:100vh;
    justify-content:center;
    align-items:center;
    flex-direction:column;
    padding:30px;
}

.page.show{
    display:flex;
}

button{
    padding:14px 24px;
    margin:10px;
    font-size:18px;
    border:none;
    border-radius:12px;
    cursor:pointer;
}

h1,h2,p{
    max-width:700px;
}
</style>
</head>

<body>

<div id="p1" class="page show">
    <h1>Mime ❤️</h1>
    <p>Me haces sentir muchas cosas por ti y no lo puedo contener más.</p>
    <button onclick="showPage('p2')">Continuar ❤️</button>
</div>

<div id="p2" class="page">
    <p>
        Desde hace tiempo lo he pensado mucho y no te lo había dicho por el miedo al rechazo.
    </p>
    <p><strong>28/2/26 ❤️</strong></p>
    <button onclick="showPage('p3')">Continuar ❤️</button>
</div>

<div id="p3" class="page">
    <p>
        Se que la distancia es el mayor impedimento para nuestro amor pero cuando dos almas se quieren dan todo por el otro.
    </p>
    <button onclick="showPage('p4')">Continuar ❤️</button>
</div>

<div id="p4" class="page">
    <p>
        Todos estos meses que he pasado contigo han sido maravillosos y me has traído pura felicidad a mi vida y te quería preguntar desde el fondo de mi corazón ❤️
    </p>

    <button onclick="showPage('p5')">Continuar ❤️</button>
</div>

<div id="p5" class="page">
    <h2>¿Te gustaría pasar la eternidad conmigo?</h2>

    <p>Lo que trato de decir es...</p>

    <h1>¿Quieres ser mi novia? ❤️</h1>

    <button onclick="showPage('final')">
        Sí, te amo ❤️
    </button>

    <button onclick="showPage('final')">
        Sí, te súper amo ❤️❤️
    </button>
</div>

<div id="final" class="page">
    <h1>⭐</h1>

    <p>
        Ten por seguro que siempre me vas a hacer el más feliz del mundo con tu compañía ❤️
    </p>

    <h2>
        Misión completada: Encontré a la persona que buscaba al otro lado del Atlántico ❤️
    </h2>
</div>

<script>
function showPage(pageId){

    let pages = document.querySelectorAll(".page");

    pages.forEach(function(page){
        page.classList.remove("show");
    });

    document.getElementById(pageId).classList.add("show");
}
</script>

</body>
</html>
