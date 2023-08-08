![Tec de Monterrey](images/logotecmty.png)
# Act 0 - Familiarizándose con el ambiente de trabajo

## <span style="color: rgb(26, 99, 169);">¿Qué tengo que hacer?</span>
En este repositorio encontrarás los archivos de entrada, así como las salidas esperadas que podrás usar para probar tu implementación. También encontrarás un archivo "main.cpp". Ahí deberás implementar tu solución. En el archivo deberás colocar en la parte superior, en comentarios, tus datos. Por ejemplo:
```
// =========================================================
// File: main.cpp
// Author: Edward Elric - A00123456
// Date: 01/01/2021
// =========================================================
```
<span style="text-decoration: underline;">De manera individual</span>, desarrolla la solución del siguiente problema:

La crisis económica más reciente fue causada en parte por la forma en que los bancos hicieron préstamos a personas que no podían pagarlos y los revendieron a otros bancos como obligaciones. Obviamente, cuando la gente no pagaba sus préstamos, todo el sistema colapsaba.

La crisis fue tan profunda que afectó a países de todo el mundo, incluido Nlogonia, donde el honorable primer ministro Man Dashuva ordenó al presidente del Banco Central encontrar una solución. Se le ocurrió una idea brillante: si todos los bancos pudieran liquidar sus obligaciones únicamente con sus propias reservas monetarias, todos los bancos sobrevivirían y se evitaría la crisis.

Sin embargo, con el elevado número de debentures y bancos involucrados, esta era una tarea extremadamente complicada, por lo que pidió su ayuda para escribir un programa que, dados los bancos y los debentures impresos por ellos, determine si es posible que todos los bancos paguen. respaldar sus deudas utilizando únicamente sus reservas monetarias y créditos.

## <span style="color: rgb(26, 99, 169);">**Entrada**</span>
La primera línea contiene dos números enteros *B* y *N*, que indican el número de bancos (1 <= *B* <= 20) y el número de obligaciones impresas por los bancos (1 <= *N* <= 20). Los bancos se identifican con números enteros entre 1 y *B*. La segunda línea contiene *B* enteros R<sub>i</sub> separados por espacios, indicando las reservas monetarias de cada uno de los bancos B (0 <= R<sub>i</sub> <= 10<sup>4</sup>), para 1 <= *i* <= *B*). Las *N* líneas siguientes contienen cada una tres enteros separados por espacios: un entero *D*, que indica el banco deudor (1 <= *D* <= *B*), un entero C, que indica el banco acreedor (1 <= *C* <= *B* y *D* != *C*) y un número entero *V*, que indica el valor de la obligación (1 <= *V* <= 10<sup>4</sup>). 

## <span style="color: rgb(26, 99, 169);">**Salida**</span>
Tu programa debe imprimir una sola línea, que contenga un solo carácter: 'S', si es posible liquidar todas las obligaciones sin un rescate del Banco Central de Nlogonia, o 'N' si es necesario un rescate.

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada 1**</span>
```
3 3
1 1 1
1 2 1
2 3 2
3 1 3
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida 1**</span>
```
S
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada 2**</span>
```
3 3
1 1 1
1 2 1
2 3 2
3 1 4
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida 2**</span>
```
N
```

Para probar tu implementación, compila tu programa con el comando:
```
g++ -std=c++11 main.cpp -o app
```
Posteriormente, prueba con cada uno de los archivos de entrada de prueba que encontrarás en este repositorio (input1.txt, input2.txt, input3.txt, input4.txt). Los resultados que debes obtener se encuentran en los archivos llamados output1.txt, output1.txt, output1.txt y output1.txt. Para realizar las pruebas, puedes usar las siguientes líneas de código. Por ejemplo, si queremos probar con el archivo de prueba "input1.txt".
```
./app < input1.txt > mysolution1.txt
diff mysolution1.txt output1.txt
```
Si el segundo comando no tenga ninguna salida, sabrás que los resultados que obtuviste son los esperados. Recuerda actualizar tu repositorio (*git push*) cuando hayas terminado tu implementación.

Por último, realiza una investigación y reflexión en forma individual de la importancia y eficiencia del uso de los diferentes algoritmos de ordenamiento y búsqueda en una situación problema de esta naturaleza, generando un documento llamado **"ReflexAct1.3.pdf"**

## <span style="color: rgb(26, 99, 169);">**¿Bajo qué criterios se evalúa mi evidencia?**</span>

- **80%** - Para cada una de las funcionalidades se evaluará:

    - **Excelente (80%)** - pasa correctamente todos los casos de prueba.
    - **Muy Bien (60%)** - pasa correctamente el 75% de los casos de prueba.
    - **Bien (40%)** - pasa correctamente el 50% de los casos de prueba.
    - **Insuficiente (20%)** - pasa correctamente menos del 50% de los casos de prueba.


- **10%** - El código deberá seguir los lineamientos estipulados en el estándar de codificación: <span class="instructure_file_holder link_holder">[liga_estándar_codificación](estandar.pdf)</span>
- **10%** - Se respetenan los nombres de las funciones en la aplicación.
