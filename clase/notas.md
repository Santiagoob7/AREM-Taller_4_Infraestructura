# 🗒️ Registro de Trabajo en Clase - Taller 4

## 📆 Fecha de la sesión
6 de septiembre de 2026

## 👥 Integrantes presentes
* Jorge Steven Doncel Bejarano — Código: 282296 / [gevengood](https://github.com/gevengood) / [jorgedobe@unisabana.edu.co](mailto:jorgedobe@unisabana.edu.co)
* David Santiago Buendia Londoño — Código: 306487 / [Santiagoob7](https://github.com/Santiagoob7) / [davidbulo@unisabana.edu.co](mailto:davidbulo@unisabana.edu.co)

## 🧠 Actividades realizadas en clase
* **Análisis del caso base (RedExpress):** Se aplicó la metodología de 5 pasos sobre la infraestructura de RedExpress, agrupando los componentes en 4 zonas (*Clientes*, *Borde / Global*, *Región Bogotá* y *Región Medellín*) e identificando los tres riesgos principales: el Balanceador de Carga como punto único de falla (SPOF), la Base de Datos Distribuida con escritura única en Bogotá como cuello de botella de latencia, y la Región Medellín sin módulo de procesamiento propio como límite de escalabilidad geográfica.
* **Decisiones de modelado para el cliente real (Insuclínicos Ltda.):** Analizamos cómo estructurar el mapa de infraestructura para una empresa manufacturera que no usa servidores formales ni servicios cloud propios. Descartamos la librería C4 y optamos por zonas físicas y lógicas (*Nube Pública*, *Red Local LAN de Oficina* y *Planta de Producción*). Decidimos marcar con advertencias (⚠️) los computadores locales y el disco duro único como puntos críticos de falla y cuellos de botella de concurrencia.
* **Herramientas usadas:** draw.io para la diagramación de red y zonas, empleando conectores punteados para evidenciar el transporte manual/físico de órdenes hacia la planta.
* **Avance en clase:** Se completó el mapa borrador del caso base ([`mapa-borrador.drawio`](mapa-borrador.drawio)) y se elaboró la tabla de diagnóstico técnico priorizando el riesgo de disponibilidad y concurrencia del archivo Excel local en Insuclínicos.

## 🧩 Boceto inicial del modelo (Caso Base RedExpress)
* [Ver Mapa de Infraestructura Borrador — RedExpress (`mapa-borrador.drawio`)](mapa-borrador.drawio)

## 🔁 Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
| :--- | :--- | :--- |
| Configuración de repositorio y diagramación final (`entrega/mapa-final.drawio`) | David Santiago Buendia | 06/09/2026 |
| Redacción del informe técnico, tabla de diagnóstico y referencias (`entrega/informe.md`) | Jorge Steven Doncel | 07/09/2026 |
