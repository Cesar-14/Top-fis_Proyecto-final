# Documentación 
## Abstract: 
La siguiente escena fue realizada en Unity con la utilización shader graph incluyendo una animación de vértices llamado vertex shading para simular el efecto y movimiento natural del agua, así mismo también se utiliza este efecto para simula el viento por medio de vegetación incluida en escena, con la utilización de un modelo de luz custom tipo Toon.

## Introducción: 
Unity es un motor de desarrollo para la creación de videojuegos que ofrece multitud de funcionalidades para desarrolladores, que también se ha utilizado en realidad virtual, en proyectos de Arquitectura y Diseño y además en la edición y previsualización de miniseries. Permite crear escenas 2D y 3D y animaciones en tiempo real y con un renderizado de gráficos e imágenes que logra una gran calidad y una importante sensación de realidad, siendo esta última funcionalidad la razón por la que la escena realizada se ha hecho aquí.  
Usamos el efecto vertex shading porque es una herramienta que nos permite trabajar con la estructura de vértices de figuras modeladas en 3D, y realizar operaciones matemáticas sobre ella para poder así definir colores, texturas e incidencia de la luz, y a su vez esto nos da libertad para realizar diferentes efectos, que van desde la deformación de un objeto hasta la recreación de las olas del mar. 

## Desarrollo: 
Para la elaboración de este proyecto se llevó a cabo una investigación previa que nos facilitó el desarrollo de los requisitos solicitados para la escena. Comenzamos con la creación de un proyecto URP (Universal Render Pipeline) en Unity para manejar de forma efectiva el tipo de trabajo que se realizaría dentro del mismo. 

El primer requisito solicitado fue la elaboración de Agua con un efecto de animación de vértices por medio de vertex shading, por lo que se procedió a crear un plano al cual se le realizaría un shader graph, incluyendo en su estructuración lo siguiente: Wave normal, Wave animation, Vertex position gradient noise, Force normal, Depth black, Black force, Water color. E incluyendo las siguientes propiedades: Depth, Strenght, Clear water, Dark water, Normal 1, Normal 2, Water strenght, Desplacement y Smooth.  
Después se procedió a añadirle a este mismo los mapas de normales y el color para terminar de producir el aspecto de agua que necesita el plano para tomar el aspecto del agua ahora con movimiento. 
El segundo requisito solicitado fue simular el efecto del viento por medio de vegetación creada a partir de vertex shading, así que se procedió a realizar un objeto al cual se le añadió como textura una flor png y así pasamos al proceso de generar un código que permitirá manejar el movimiento en nivel de su densidad, velocidad e intensidad. 
Posteriormente se procedió a descargar un asset, llamado “Rocks and Boulders 2” desde la Unity Asset Store que nos permitiría darle un mejor aspecto visual a la escena y que acompañaría a nuestro trabajo para completar la escena con modelos y texturas de roca, y tierra.
Y finalmente se llevó a cabo el proceso de creación de un modelo de luz en el cual se utilizó el modelo Custom Lambert con efecto sidelight y un brillo Surface Diffuse Strenght en el agua y rocas. El modelo de luz Custom Lambert fue creado a partir de nosotros mismos, utilizando un subgraph para poder crear su código, este modelo es parecido al efecto de luz predeterminada que se aplica a cualquier material en unity, la diferencia es que al crearlo nosotros podemos controlar la intensidad de la luz al llegar al material. El efecto de luz sidelight o efecto de luz de lado funciona como el efecto de la luz a la orilla del material, creado de la misma manera que el modelo de luz custom.
Por último, agregamos un brillo Surface Diffuse Strenght que se refiere a como la luz afecta a los materiales y podemos controlar su intensidad, fue creado a partir de un subgraph para poder escribir su código.

## Conclusiones: 
Para llevar a cabo eficazmente una escena realista y atractiva, los objetos en ella deben de ser afectados y manipulados a través de mecanismos como lo es el manejo de scripts o en este caso la estructuración de un shadergraph que nos permite simular los aspectos realistas de la naturaleza. Unity nos proporciona componentes que manejan esta simulación de física, nos permite ajustar parámetros para crear objetos que se comporten de forma pasiva de manera realista, es decir, que se muevan por efectos de simulación y colisión, que aspectos básicos y naturales como el viento y la luz afecte directamente a los objetos de forma físicamente realista.  
Al controlar la física desde los scripts, podemos darle a un objeto el dinamismo de un coche, una máquina, una pieza de tela, o como en este caso, agua, vegetación y viento. 

## Resultados: 
El resultado final fue una escena en la que se pone en practica el efecto del movimiento del agua, el movimiento de la vegetación natural por el aire y el uso de un modelo de luz custom. Todos estos procesos se llevaron a cabo de la manera correcta por lo que el proyecto tuvo resultados satisfactorios creando los efectos deseados.

## Referencias: 
-	Zucconi, A., & Lammers, K. (2016). Unity 5.x Shaders and Effects Cookbook [Libro electrónico]. https://books.google.es/books?hl=es&lr=&id=-llLDAAAQBAJ&oi=fnd&pg=PP1&dq=Unity+vertex+shading&ots=CXkE3K6nfc&sig=g8clSCaJaGoG29Wc0xaKV7jSJi0#v=onepage&q&f=false 

-	Wenfeng Hu, W. H., Zhe Wang, Z. W., Xin Fan, X. F., School of Computer Science Communication University of China. (2021, mayo). Contained Fluid Simulation Based on Game Engine: IEEE Xplore. https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7960052 

-	Canet Vidal, A. & Budapest University of Technology and Economics. (2017, junio). Development of a survival game in a Unity 3D environment. https://dugi-doc.udg.edu/handle/10256/14833 

-	Efecto de agua. (s. f.). programador clic. Recuperado 24 de mayo de 2021, de https://programmerclick.com/article/79961152513/ 

-	Tiptur Ravindra, T. & California State University. (2018). SIMULATION OF WATER. http://csus-dspace.calstate.edu/handle/10211.3/207679 

-	Doppioslash, C. (2017). Physically Based Shader Development for Unity. Apress. 

-	Halladay, K. (2019). Practical Shader Development: Vertex and Fragment Shaders for Game Developers. Apress. https://books.google.es/books?hl=es&lr=&id=ouORDwAAQBAJ&oi=fnd&pg=PR5&dq=Unity+WATER+WITH+VERTEX+SHADER&ots=ZLJedJ-fJE&sig=Ed4mtk5-trh-qZaIsbs4SgkxIcE#v=onepage&q=Unity%20WATER%20WITH%20VERTEX%20SHADER&f=false 

-	Bikmullina y E. Garaeva, "El desarrollo de técnicas de modelado de objetos 3D para su uso en los entornos de Unity", 2020 International Multi-Conference on Industrial Engineering and Modern Technologies (FarEastCon) , 2020, pp. 1-6, doi: 10.1109 /FarEastCon50210.2020.9271568. 

-	Busquets Duran, R. & Fundació Politècnica de Catalunya. (2014). Procedural Textures Generation Adaptation into a Unity tool. https://upcommons.upc.edu/handle/2117/174268 

-	Ejby Jensen, P. D., & Francis, N. (207–08). Interactive shader development. https://dl.acm.org/doi/10.1145/1274940.1274959 

-	Olano, M., Kuehne, B., & Simmons, M. (2003, julio). Automatic shader level of detail. ACM DL. https://dl.acm.org/doi/10.5555/844174.844176 

-	Alex Frasson, A.,  Engel, T. A., & Pozzer, C. T. (Universidade Federal de Santa Maria, Brazil, 2016). Improving Terrain Visualization Through Procedural Generation and Hardware Tessellation. http://www.sbgames.org/sbgames2016/downloads/anais/157677.pdf


-	Vertex Shader - OpenGL Wiki. (2017, November 10). OpenGL Wiki. https://www.khronos.org/opengl/wiki/Vertex_Shader


-	Marinacci, J. (2019, February 28). Customizing Vertex shaders. Medium. https://medium.com/@joshmarinacci/customizing-vertex-shaders-86527c5693b2

-	Ureña, C. (n.d.). Evaluación del MIL mediante programación del cauce gráfico con GLSL. Universidad de Granada. Retrieved May 23, 2021, from https://lsi2.ugr.es/%7Ecurena/doce/vr/pracs.ext/05/

-	Rost, R. (2006, January 25). Vertex Shader | A Simple Shading Example in OpenGL Shading Language. Informit. https://www.informit.com/articles/article.aspx?p=446452&seqNum=2


-	Vertex Shaders | ISF Documentation. (n.d.). ISF Documentation. Retrieved May 23, 2021, from https://docs.isf.video/primer_chapter_5.html#vertex-shaders-vs-fragment-shaders

-	Vertex shader. (2011, September 25). Learn OpenGL ES. https://www.learnopengles.com/tag/vertex-shader/


-	Technologies, U. (n.d.). Unity - Manual: Vertex and fragment shader examples for the Built-in Render Pipeline. Unity. Retrieved May 26, 2021, from https://docs.unity3d.com/Manual/SL-VertexFragmentShaderExamples.html


-	Bellucci, F. (2018, October 1). Vertex Shader Tutorial for Unity. Febucci. https://www.febucci.com/2018/10/vertex-shader/


-	Zucconi, A. (2020, July 29). Vertex and fragment shaders in Unity3D. Alan Zucconi. https://www.alanzucconi.com/2015/07/01/vertex-and-fragment-shaders-in-unity3d/

-	Vertex Displacement. (2018, June 16). Ronja’s Tutorials. https://www.ronja-tutorials.com/post/015-wobble-displacement/


-	Technologies, U. (n.d.-a). Tipos de luz - Unity Manual. Unity. Retrieved May 26, 2021, from https://docs.unity3d.com/es/2018.4/Manual/Lighting.html


-	Technologies, U. (n.d.-b). Unity - Manual: Custom lighting models in Surface Shaders. Unity. Retrieved May 26, 2021, from https://docs.unity3d.com/Manual/SL-SurfaceShaderLighting.html

-	Flick, J. (2019, November 30). Directional Lights. Catlike Coding. https://catlikecoding.com/unity/tutorials/custom-srp/directional-lights/


-	Technologies, U. (n.d.-c). Unity - Manual: Custom Lighting models in Surface Shaders. Unity. Retrieved May 26, 2021, from https://dev.rbcafe.com/unity/unity-5.3.3/en/Manual/SL-SurfaceShaderLighting.html


-	Hedquist, A. (2018, January 23). Toon shader with a custom lighting model - Aaron Hedquist. Medium. https://medium.com/@aarhed/toon-shader-with-a-custom-lighting-model-276030c0338b


-	Unity Toon Shader Tutorial at Roystan. (n.d.). Roystan. Retrieved May 26, 2021, from https://roystan.net/articles/toon-shader.html


-	Kalupahana, D. (2019, June 20). Shaders in Unity — Lambert and Ambient - Deshan Kalupahana. Medium. https://medium.com/@deshankalupahana/shaders-in-unity-lambert-and-ambient-ceba9fab6cfa


-	Lindman, A. (2019, July 31). Custom Lighting in Shader Graph: Expanding your graphs in 2019. Unity Blog. https://blog.unity.com/technology/custom-lighting-in-shader-graph-expanding-your-graphs-in-2019

## Link de video del Proyecto:
https://drive.google.com/file/d/1R6sjp4o-6TR3CIca2jNdCfnZnGig61Sr/view

