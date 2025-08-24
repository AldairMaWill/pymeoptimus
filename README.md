# 🚀 PymeOptimus
<div align="center">

![PymeOptimus Logo](https://img.shields.io/badge/PymeOptimus-0.1.0-blueviolet)
![Python](https://img.shields.io/badge/Python-3.8%2B-green)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Contribuciones](https://img.shields.io/badge/Contribuciones-Bienvenidas-brightgreen)

</div>

## ⚡ Introducción
PymeOptimus es un lenguaje de programación de alto nivel construido sobre Python; Diseñado para hacer la programación accesible, intuitiva y poderosa para todos. Combina la simplicidad del lenguaje natural con la potencia de las mejores bibliotecas de Python, permitiendo crear desde scripts simples hasta aplicaciones de escritorio modernas con una curva de aprendizaje mínima.

## 🎯 ¿Por qué PymeOptimus?
En un mundo donde la demanda de Desarrolladores supera la oferta, PymeOptimus busca:

✔ Reducir la barrera de entrada a la programación

✔ Hacer el desarrollo más intuitivo y menos intimidante

✔ Mantener toda la potencia de Python y sus ecosistemas

✔ Permitir crear aplicaciones visualmente atractivas con mínimo esfuerzo

## 📖 Tabla de Contenidos
- [✨ Características](#-características)
- [🚀 Instalación Rápida](#-instalación-rápida)
- [🎯 ¿Por qué PymeOptimus?](#-por-qué-pymeoptimus)
- [📚 Primeros Pasos](#-primeros-pasos)
- [💫 Ejemplos Prácticos](#-ejemplos-prácticos)
- [🏗️ Arquitectura](#-arquitectura)
- [🤝 Contribuir](#-contribuir)
- [📄 Licencia](#-licencia)

## ✨ Características

### 🎯 Sintaxis Intuitiva y Bilingüe
```pyme
// Español
función saludar(nombre) {
    imprimir "¡Hola, " + nombre + "!"
}

// English
function greet(name) {
    print "Hello, " + name + "!"
}

// ¡Incluso mezclado!
función calculate_total(price, quantity) {
    retornar price * quantity
}
```
### 🎨 Interfaces Bonitas con una Línea
```pyme
// Crear una aplicación completa con interfaz moderna
crear app "Gestión de Tareas" tema: "superhero" {
    ventana principal {
        título: "Mis Tareas"
        tamaño: 1000x700
        
        contenido {
            columna {
                espaciado: 20
                padding: 30
                
                etiqueta "Lista de Tareas" con {
                    estilo: "h1"
                    color: "primario"
                }
                
                lista_tareas {
                    "Comprar leche" -> prioridad: "alta",
                    "Estudiar PymeOptimus" -> completada: verdadero,
                    "Hacer ejercicio" -> prioridad: "media"
                }
                
                botón "Nueva Tarea" con {
                    accion: => abrir_modal "nueva_tarea"
                    estilo: "éxito"
                    tamaño: "grande"
                }
            }
        }
    }
}
```
### 📊 Procesamiento de Datos Simplificado
```pyme
// Análisis de datos con sintaxis natural
datos = leer_csv "ventas_2024.csv"

resumen = analizar datos {
    grupo_por: "categoría"
    calcular: {
        "total_ventas": suma "monto",
        "promedio": promedio "monto",
        "num_transacciones": contar "id"
    }
    ordenar_por: "total_ventas" descendente
}

mostrar_tabla resumen
crear_grafico resumen tipo: "barras" título: "Ventas por Categoría"
```
## 🚀 Instalación Rápida
Requisitos Previos

- Python 3.8 o superior
- pip (gestor de paquetes de Python)

Instalación desde PyPI
```bash
# Instalación básica
pip install pymeoptimus

# Instalación con soporte completo de UI
pip install pymeoptimus[ui]

# Instalación completa con todas las características
pip install pymeoptimus[full]
```
Instalación desde Código Fuente
```bash
# Clonar el repositorio
git clone https://github.com/tuusuario/pymeoptimus.git
cd pymeoptimus

# Instalar en modo desarrollo
pip install -e .

# O instalar con extras
pip install -e .[ui,full]
```
Verificar la Instalación
```bash
# Ejecutar el REPL interactivo
pyme

# O probar con un archivo de ejemplo
pyme ejemplos/hola_mundo.pyme
```
## 🎯 ¿Por qué PymeOptimus?
### 🔍 Para Educadores y Estudiantes
```pyme
// Conceptos complejos se vuelven simples
// Python tradicional (15+ líneas)
class Estudiante:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    def es_mayor(self):
        return self.edad >= 18

est = Estudiante("Maria", 20)
print(est.es_mayor())

// PymeOptimus (4 líneas)
clase Estudiante {
    constructor(nombre, edad) {
        self.nombre = nombre
        self.edad = edad
    }
    es_mayor => self.edad >= 18
}

maria = Estudiante("Maria", 20)
imprimir maria.es_mayor()
```
### 💼 Para Desarrolladores de PYMEs
```pyme
// Automatización de procesos empresariales
función procesar_pedidos() {
    pedidos = obtener_pedidos_pendientes()
    
    para cada pedido en pedidos {
        si pedido.es_urgente() {
            enviar_notificacion(pedido.cliente, "Tu pedido está en proceso")
            actualizar_estado(pedido, "procesando")
        }
    }
    
    generar_reporte pedidos
}

// Ejecutar diariamente a las 9:00 AM
programar_tarea "procesar_pedidos" cada "día" a "9:00"
```
### 🎮 Para Creadores de Contenido
```pyme
// Crear un juego simple con PyGame
importar juego

crear juego "Aventura Espacial" {
    jugador = crear_nave {
        posición: 400x500
        velocidad: 5
        disparo: tecla "espacio"
    }
    
    enemigos = crear_oleada cantidad: 10
    
    actualizar cada_frame => {
        si tecla_presionada "derecha" { jugador.mover_derecha }
        si tecla_presionada "izquierda" { jugador.mover_izquierda }
    }
}
```
## 📚 Primeros Pasos
### 🎯 Tu Primera Aplicación
Crea un archivo hola_mundo.pyme:
```pyme
// Aplicación de escritorio completa
crear app "Mi Primera App" {
    ventana principal {
        título: "¡Hola PymeOptimus!"
        tamaño: 600x400
        
        contenido {
            columna {
                espaciado: 15
                padding: 25
                
                etiqueta "¡Bienvenido a la Programación!" con {
                    estilo: "h1"
                    color: "éxito"
                }
                
                campo_texto "Nombre" -> nombre_usuario
                
                botón "Saludar" con {
                    accion: => {
                        mensaje = "¡Hola " + nombre_usuario + "!"
                        mostrar_mensaje mensaje
                    }
                    estilo: "primario"
                }
                
                botón "Salir" con {
                    accion: => cerrar_aplicacion
                    estilo: "peligro"
                }
            }
        }
    }
}
```
Ejecútalo con:
```pyme
pyme hola_mundo.pyme
```
### 📖 Conceptos Básicos
Variables y Tipos
```pyme
// Declaración simple con inferencia
nombre = "Ana"           // Texto (String)
edad = 25                // Número entero (Int)
altura = 1.75            // Número decimal (Float)
activo = verdadero       // Booleano (True/False)

// Tipado explícito opcional
precio: decimal = 19.99
cantidad: entero = 42
mensaje: texto = "Hola"
```
Estructuras de Control
```pyme
// Condicionales
si edad >= 18 {
    imprimir "Eres adulto"
} sino si edad >= 13 {
    imprimir "Eres adolescente"
} sino {
    imprimir "Eres niño"
}

// Bucles
para i en rango(1, 6) {
    imprimir "Número: " + i
}

mientras activo {
    // Hacer algo...
    si condicion_parada {
        activo = falso
    }
}
```
Funciones
```pyme
// Función simple
función duplicar(numero) {
    retornar numero * 2
}

// Función con parámetros opcionales
función saludar(nombre, mensaje = "Hola") {
    retornar mensaje + ", " + nombre + "!"
}

// Función flecha (arrow function)
calcular_iva = (monto) => monto * 0.21
```
## 💫 Ejemplos Prácticos
### 📊 Aplicación de Gestión de Datos
```pyme
// Analizar y visualizar datos de ventas
importar analitica
importar visualizacion

datos = leer_excel "ventas_2024.xlsx"

// Limpiar y procesar datos
datos_limpios = datos.filtrar(fila => fila.monto > 0)
                     .transformar("fecha", => formatear_fecha(fila.fecha))

// Análisis avanzado
analisis = analizar datos_limpios {
    grupo_por: ["mes", "categoría"]
    calcular: {
        "ventas_totales": suma "monto",
        "ventas_promedio": promedio "monto",
        "num_transacciones": contar "id"
    }
    filtro: "región" == "Norte"
}

// Visualización interactiva
crear_dashboard {
    titulo: "Análisis de Ventas 2024"
    
    grafico_barras {
        datos: analisis
        x: "mes"
        y: "ventas_totales"
        grupo: "categoría"
    }
    
    grafico_torta {
        datos: analisis.agrupar_por("categoría")
        valores: "ventas_totales"
        etiquetas: "categoría"
    }
    
    tabla_datos {
        datos: analisis
        columnas: ["mes", "categoría", "ventas_totales", "ventas_promedio"]
        ordenar_por: "ventas_totales" descendente
    }
}
```
### 🌐 Aplicación Web Simple
```pyme
// Crear un servidor web con API REST
crear servidor puerto: 8000 {
    ruta "/" => {
        retornar vista "inicio" con {
            titulo: "Mi App Web",
            usuarios: obtener_usuarios()
        }
    }
    
    ruta "/api/usuarios" => {
        usuarios = obtener_desde_bd "SELECT * FROM usuarios"
        retornar json usuarios
    }
    
    ruta "/api/usuarios" metodo: "POST" => {
        datos = obtener_json_datos()
        resultado = insertar_en_bd "usuarios" datos
        retornar json { "éxito": verdadero, "id": resultado.id_insertado }
    }
}

// Cliente HTTP para consumir APIs
respuesta = enviar peticion {
    url: "https://api.mi-servicio.com/datos"
    metodo: "GET"
    headers: {
        "Authorization": "Bearer mi_token"
    }
}

si respuesta.exitoso {
    datos = respuesta.json()
    procesar_datos datos
} sino {
    imprimir "Error: " + respuesta.estado
}
```
### 🎮 Juego Simple con PyGame
```pyme
// Juego de plataformas básico
importar juego

crear juego "Aventura Pixel" {
    tamaño: 800x600
    fps: 60
    
    jugador = crear_personaje {
        posicion: 100x400
        velocidad: 5
        gravedad: 0.5
        salto: 12
        sprite: "heroe.png"
    }
    
    plataformas = [
        crear_plataforma posicion: 0x550 tamaño: 800x50,
        crear_plataforma posicion: 200x450 tamaño: 200x25,
        crear_plataforma posicion: 500x350 tamaño: 150x25
    ]
    
    enemigos = crear_oleada {
        cantidad: 5
        tipo: "fantasma"
        patrón: "movimiento_sinusoidal"
    }
    
    actualizar cada_frame => {
        // Movimiento del jugador
        si tecla_presionada "derecha" { jugador.mover_derecha }
        si tecla_presionada "izquierda" { jugador.mover_izquierda }
        si tecla_presionada "espacio" y jugador.en_suelo { jugador.saltar }
        
        // Verificar colisiones
        para cada plataforma en plataformas {
            si jugador.colisiona_con(plataforma) {
                jugador.detener_caida()
            }
        }
        
        // Actualizar enemigos
        para cada enemigo en enemigos {
            enemigo.mover_segun_patron()
            si jugador.colisiona_con(enemigo) {
                jugador.perder_vida()
            }
        }
    }
}
```
## 🏗️ Arquitectura
### 📁 Estructura del Proyecto
```text
pymeoptimus/
├── 📂 compiler/         # Núcleo del compilador
├── 📂 core/             # Librería core del lenguaje  
├── 📂 stdlib/           # Biblioteca estándar
├── 📂 frontend/         # Herramientas de interfaz
├── 📂 ide/              # Entorno de desarrollo
├── 📂 examples/         # Ejemplos de código
├── 📂 docs/             # Documentación
└── 📂 tests/            # Entorno de pruebas
```
### 🔄 Flujo de Compilación
1. Análisis Léxico: Código fuente → Tokens

2. Análisis Sintáctico: Tokens → AST (Abstract Syntax Tree)

3. Transformación: AST PymeOptimus → AST Python

4. Generación de Código: AST Python → Código Python ejecutable

5. Ejecución: Ejecución del código Python resultante

## 🤝 Contribuir
¡Nos encantan las contribuciones! Aquí cómo puedes ayudar:

### 🐛 Reportar Errores
1. Ve a Issues

2. Busca si el error ya fue reportado

3. Si no, crea un nuevo issue con:
   - Descripción clara del problema
   - Pasos para reproducirlo
   - Versión de PymeOptimus y Python
   - Capturas de pantalla si es aplicable

### 💡 Sugerir Nuevas Características
1. Abre un nuevo issue

2. Usa la plantilla "Feature Request"

3. Describe la característica en detalle

4. Explica por qué sería útil

## 📄 Licencia
Este proyecto está bajo la Licencia MIT - ve el archivo LICENSE para detalles.

## AMW
