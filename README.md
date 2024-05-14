# Semana-6
let claveAlmacenada = "1234"; 
function validarClave(claveIngresada) {
    if (claveIngresada === claveAlmacenada) {
        return true; 
    } else {
        return false; 
    }
}


function iniciarPrograma() {
    
    let claveUsuario = prompt("Por favor, ingrese su clave:");

    
    if (validarClave(claveUsuario)) {
        
        alert("Clave válida. Acceso permitido.");
        
    } else {
        
       alert("Clave incorrecta. Por favor, inténtelo de nuevo.");
        iniciarPrograma(); 
    }
}


iniciarPrograma();