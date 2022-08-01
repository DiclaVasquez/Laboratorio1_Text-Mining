# Laboratorio1_Text-Mining

## El modelo de color HSV

En el modelo de color HSV, un color se define por su tono (H), su saturación (S) y su luminosidad (V), por lo que se parece más a la percepción del color humano que a los modelos de color aditivos y sustractivos. Es fácil ajustar un color por su saturación y brillo.

• Tono: especifica el tono (color) establecido para el color. El tono se indica como un entero del 0 al 240, ambos incluidos. Este se remuestrea a partir de los valores de 0° a 360° en que se indica el tono como ángulo en sentido antihorario alrededor del cono de color. Los colores primarios y secundarios presentan los siguientes valores de tono: rojo = 0 (0°), amarillo = 40 (60°), verde = 80 (120°), cian = 120 (180°), azul = 160 (240°) y magenta = 201 (300°).

• Saturación: especifica la intensidad de saturación establecida para el color. La saturación se indica como un entero del 0 al 255, ambos incluidos (que representan del 0 al 100%). La saturación de un color hace referencia a la medida en que se aleja de un color neutro como el gris o, dicho de un modo más sencillo, su colorido. Cuando la saturación es de 255, el color presenta una saturación máxima. Cuando el valor de la saturación es 0, el color es no saturado y parece gris (a menos que el valor sea 0 ó 255, en cuyo caso aparece negro o blanco).

• Brillo: especifica la intensidad del blanco en el color. El valor se indica como un entero del 0 al 255, ambos incluidos (que representan del 0 al 100%). Un color con un valor establecido en 0 aparece negro. Un color con un valor establecido en 255 y una saturación de 0 aparece como blanco. Conversión al espacio de colores HSV En lugar de eso vamos a convertir los píxeles desde el espacio RGB al espacio HSV, en donde cada píxel se codifica también con tres valores, pero ahora con significado diferente: El canal H indica el tono (hue) del color (verde, rojo, azul, amarillo, etc). El tono es lo que tradicionalmente entendemos como "color". El canal S indica la saturación (saturation) de color Si un color es más saturado, es más "puro" Si es menos saturado, tiene más "gris" El canal V indica la luminosidad o intensidad (value) del pixel. V=0 indica un pixel negro V=1 indica un pixel blanco La función rgb_to_hsv del módulo matplotlib.colorsnos permite hacer justamente eso.

¿Cómo se utiliza el HSV?
El modelo de color HSV se utiliza cuando se seleccionan colores para pintura o tinta porque HSV representa mejor la forma en que las personas se relacionan con los colores que el modelo de color RGB.

La rueda de color HSV también se utiliza para generar gráficos de alta calidad. Aunque menos conocido que sus primos RGB y CMYK, el enfoque HSV está disponible en muchos programas de software de edición de imágenes de gama alta.

La selección de un color HSV comienza con la selección de uno de los tonos disponibles, que es la forma en que la mayoría de los seres humanos se relacionan con el color y, a continuación, el ajuste de los valores de sombra y brillo.
