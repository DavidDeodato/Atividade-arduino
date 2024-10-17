### Parte 1 - Piscar LED no Arduino Uno

Conforme solicitado na atividade 1, o código foi desenvolvido para acionar o LED integrado do Arduino Uno. Através do **pinMode()**, o pino do LED integrado (LED_BUILTIN) é configurado como saída. No loop principal, utilizamos a função **digitalWrite()** para alternar o estado do LED entre ligado (**HIGH**) e desligado (**LOW**), com um intervalo de 500 milissegundos entre cada mudança, controlado pela função **delay()**. Esse processo faz com que o LED integrado do Arduino pisque continuamente a cada 500ms.

<div align="center">
<sub>Figura 1 - led </sub><br>
<img src="arduino.jpeg" width="80%" ><br>
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>


Para ver o vídeo consulte [este link](https://youtube.com/shorts/Ly-zNU17j2g?si=9vx52OHsodNeXUFh).


## Código:



```c++


void setup() {
 
  pinMode(LED_BUILTIN, OUTPUT);

}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  
  delay(500);                      
  digitalWrite(LED_BUILTIN, LOW);   
  delay(500);                      
}
```