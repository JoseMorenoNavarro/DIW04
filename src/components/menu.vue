<template>
  <section id="menu">
    <div class="barra">
      <div class="navegacion">           
        <nav>
            <ul>
                <li><a href="#">INICIO</a></li>
                <li><a href="#">ORDENADORES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">MÓVILES</a></li>
                <li><a href="#">TABLETS</a></li>
                <li><a href="#">MULTIMEDIA</a></li>
            </ul>
        </nav>
      </div>
      <div class="registro">
        <a class="singup" href="#">REGISTRO</a>
        <a class="login" href="#">INICIAR SESIÓN</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
#menu{
    background: #0090ED;
}
#menu a{
    text-decoration: none;
    font-weight: 700;
}
#menu .barra {
    display: flex;
    justify-content: space-between;
}
.barra .navegacion {
    display:flex;
    justify-content: flex-start;
    align-items: center;
}
.navegacion nav li {
    display: inline;
    list-style-type: none;    
    padding:1rem;
}
.navegacion nav li a{
    color: white;
}
.barra .registro{
    display:flex;
    justify-content: flex-end;
    align-items: center;
}
.registro a{    
    padding-left: 0.8rem;
    padding-right: 0.8rem;
    color:white;
}
.singup{
    background: #ED5C00;     
    padding:1rem;
}
.singup:hover, .login:hover{
    background-color: white;
    color:#0090ED;    
    padding:1rem;    
    padding-left: 0.8rem;
    padding-right: 0.8rem;
}
.navegacion nav li a:hover{
    color:#ED5C00;  
}

</style>