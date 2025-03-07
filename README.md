# serialTerminal

Terminal Serial para el curso de sistemas físicos interactivos 1. La aplicación está disponible [aquí](https://juanferfranco.github.io/serialTerminal/).

## ¿Cómo te conectas a un dispositivo externo?

1. Debes desconectarte primero de cualquier aplicación que esté usando el puerto serial
2. Click en Configurar puerto:
   
   <img src="https://github.com/user-attachments/assets/83074daa-f2dc-47df-94f5-c33fbde790f9" alt="Configurar puerto" width="100">  

4. Deja las opciones por defecto como están y dale click a Conectar:

   <img src="https://github.com/user-attachments/assets/d258e919-cb9b-4b1b-8eb4-8b65dbc32c1c" alt="Opciones" width="300">  

4. Selecciona mbed Serial Port o micro:bit. Si todo sale bien deberás ver que el estado de la aplicación es Conectada:

   <img src="https://github.com/user-attachments/assets/6e13ec68-e3a4-468f-a18c-2c4ba3ff8fc5" alt="Opciones" width="300">  

## ¿Cómo puedes recibir datos?

En el cuadro de texto de recepción de datos podrás ver los datos cuando te lleguen. Ten en cuenta que siempre te llegarán bytes, pero con  
el menú de selección de Mostrar datos como, podrás escoger cómo quieres interpretar esos bytes. Por ejemplo, si seleccionas **Texto**, los bytes 
que lleguen serán interpretados según [esta tabla](https://www.asciitable.com/). Por tanto si el byte que recibes es un 41 (en hexadecimal) entonces 
se pintará una letra **A**. 

<img src="https://github.com/user-attachments/assets/8b83110b-70d6-4e9c-b4b6-7ead5125f33a" alt="Opciones" width="300">  

## ¿Cómo puedes transmitir datos?

Puedes transmitir datos en formato de texto y en hexadecimal. Si seleccionas el formato Texto, todos los caracteres que escribas se convertirán 
a los bytes correspondientes según [esta tabla](https://www.asciitable.com/) y se transmitirán por el puerto serial. Ten en cuenta que al añadir 
**\r** y/o **\n** podrás transmitir los bytes **0D** (**\r**) y/o **0A** (**\n**) junto con el texto que escribas. Estos caracteres son importantes 
para marcar el fin de la cadena de texto.

También podrás escribir directamente los bytes que deseas transmitir cambiando el formato a **Hexadecimal**.

Si activas **Echo local**, lo que envíes también se mostrará en el cuadro de texto de recepción de datos.

