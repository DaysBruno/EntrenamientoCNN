# EntrenamientoCNN
Codigo de procesamiento de imágenes usando una CNN para la detección de emociones usando expresiones faciales
En este repositorio se incluyen los códigos para la descarga de imágenes, entrenamiento de la CNN y uso de la misma. NINGUNO DE ESOS TRES ARCHIVOS ES DE MI AUTORÍA.
## Motivación
Durante la lectura del capítulo 2 Ethics of Artificial Intelligence de Bernd Carsten Stahl, Doris Schroeder, Rowena Rodrigues (de acceso libre) se trata el tema de la discriminación debido al sesgo existente durante el entrenamiento de los modelos empleados en IA con diferentes propósitos, debido a que durante el entrenamiento de los modelos que utilizan el reconocimiento facial, se les son proporcionadas, en su mayoría, imágenes de hombres caucásicos. Por lo que en particular, el modelo fue entrenado con pocas imágenes pero con un cantidad parecidad por emoción y con diversidad étnica. De esta forma se busca comparar el desempeño del modelo con esta base de datos y la base FER2013.
## Elementos en el repositorio
En este repostorio se encontrarán:
Código para descargar imágenes.
Código para entrenar la CNN.
Código para usar la CNN.
Código para transformar los pixeles de las imágenes en un archivo CSV en caso de querer crear una base nueva.
Archivo CSV editado en Excel para darle el mismo formato que tiene la base FER2013
La carpeta de imágenes que se utilizaron para entrenar el modelo.
La carpeta de imágenes que se utilizaron para probar el modelo. 

## Formato
El formato que debe tener la nueva base, en caso de querer crear una es la siguiente.
emotion, pixels, usage
Donde emotion son números enteros del 0 al 6, donde 0 = Enojo, 1 = Asco, 2 = Miedo, 3 = Felicidad, 4 = Tristeza, 5 = Sorpresa, 6 = Neutral,
pixels son los pixeles, son los valores que devuelve el código y usage toma los valores Training, PrivateTest y PublicTest.
El 80% de los datos llevan el valor Training, 10% Private Test y 10 % PublicTest, esto se asigna de manera aleatoria, es importante mezclar los datos obtenidos y después asignarles su uso. 
