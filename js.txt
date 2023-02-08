// FUNCION QUE APLICA EL ESTILO A LA OPCION SELEC EN EL MENU Y LA LA QUITA
function seleccionar(link){
    let opciones = document.querySelectorAll('#links a');
    opciones [0].className = ""
    opciones [1].className = ""
    opciones [2].className = ""
    opciones [3].className = ""
    opciones [4].className = ""
    link.className = "seleccionado";

    // DESAPARECE EL MENU QUE SE SELECCIONO
    let x = document.getElementById("nav");
    x.className = "";
}

// FUNCION DEL MENU RESDPONSIVE
function responsiveMenu(){
    let x = document.getElementById("nav");
    if (x.className === ""){
        x.className = "responsive";
    } else {
        x.className = "";
    }
}

// // SCROLLING PARA APLICAR LA ANIMACION DE LA BARRA DE HABILIDADES
// window.onscroll = function(){
//     efectoHabilidades()
// };
// // FUNCION QUE APLICA LA ANIMACION
// function efectoHabilidades(){
//     let skills = document.getElementById("skills");
//     let distancia_skills = window.innerHeight - skills.getBoundingClientRect().top;
//     if (distancia_skills >=300){
//         document.getElementById("html").classList.add("barra-progreso1");
//         document.getElementById("javascript").classList.add("barra-progreso2");
//         document.getElementById("bd").classList.add("barra-progreso3");
//     }
// }