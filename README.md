## Descripción
Una empresa de consultoría de ingeniería administra las redes eléctricas de varios hoteles. Cada red se modela como un grafo dirigido no ponderado (⁠Grafo& g⁠), donde los vértices (de {0} a {N-1}) son habitaciones o subestaciones del hotel, y los arcos dirigidos representan cables de alimentación de sentido único. El vértice 0 es siempre la Sala del Generador General.
Implemente en C++ las siguientes dos funciones globales externas:

1) ⁠void asegurarRespaldo(Grafo& g, int X): Determina si el sector crítico {X} es alcanzable desde el Generador General (0). Si al finalizar la exploración se detecta que {X} no está conectado, la función debe modificar el grafo agregando un arco dirigido directo desde el Generador General (0) hacia {X} para establecer una línea de respaldo.

2) ⁠int consultarDistanciaMinima(Grafo& g, int Y)⁠ (BFS): Encuentra la ruta que atraviese la menor cantidad de subestaciones intermedias desde el Generador General (0) hacia el sector {Y}, calcula y retorna esta cantidad mínima de conexiones. Si el sector {Y} es inalcanzable, retorna ⁠-1⁠.
