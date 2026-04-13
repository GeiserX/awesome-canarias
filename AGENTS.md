# AGENTS.md — awesome-canarias

## Propósito

Selección de software open source que da **soporte específico a las Islas Canarias** — su gobierno autonómico (Gobierno de Canarias), cabildos insulares, ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco son las Islas Canarias: el software debe dirigirse específicamente a esta comunidad autónoma o a sus islas y municipios.

## Ámbito

- **7 islas** del archipiélago canario: Tenerife, Gran Canaria, Lanzarote, Fuerteventura, La Palma, La Gomera, El Hierro.
- **2 provincias**: Santa Cruz de Tenerife (Tenerife, La Palma, La Gomera, El Hierro) y Las Palmas (Gran Canaria, Lanzarote, Fuerteventura).
- Principales ciudades: Santa Cruz de Tenerife, Las Palmas de Gran Canaria, San Cristóbal de La Laguna, Telde, Arona, Arrecife, Santa Lucía de Tirajana, Puerto del Rosario, Adeje, Granadilla de Abona, La Orotava, Puerto de la Cruz, Los Llanos de Aridane, Arucas, Gáldar, Icod de los Vinos, Güímar, Valverde.
- **Universidades**: ULL (Universidad de La Laguna), ULPGC (Universidad de Las Palmas de Gran Canaria).
- **Instituciones**: Gobierno de Canarias, Cabildo de Tenerife, Cabildo de Gran Canaria, ISTAC (Instituto Canario de Estadística), ITER (Instituto Tecnológico y de Energías Renovables), IAC (Instituto de Astrofísica de Canarias), GTC (Gran Telescopio de Canarias), SCS (Servicio Canario de la Salud), ACIISI (Agencia Canaria de Investigación, Innovación y Sociedad de la Información).

## Criterios de inclusión

### Incluir

- Software que interactúa con el **Gobierno de Canarias** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **cabildos insulares** (Tenerife, Gran Canaria, Lanzarote, Fuerteventura, La Palma, La Gomera, El Hierro).
- Herramientas para **ayuntamientos** de las Islas Canarias.
- Software de **universidades canarias** (ULL, ULPGC) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de Canarias (ISTAC, eDatos, datos.canarias.es).
- Software relacionado con el **IAC** (Instituto de Astrofísica de Canarias), el **GTC** (Gran Telescopio de Canarias) y observatorios del archipiélago.
- Herramientas del **ITER** (Instituto Tecnológico y de Energías Renovables de Tenerife).
- Software de **transporte** canario (TITSA, Guaguas Municipales, Fred Olsen, Armas, Binter).
- Herramientas de **cartografía y SIG** específicas de Canarias (IDECanarias, Grafcan).
- Software de **vulcanología y riesgos naturales** de Canarias (Cumbre Vieja, Timanfaya, Teide).
- Herramientas de **turismo y patrimonio** de las islas.
- Software de **medio ambiente y biodiversidad** canaria.
- Proyectos del **sistema sanitario canario** (SCS, hospitales).
- Software **educativo** específico de la región.
- Herramientas de **meteorología y clima** regional.
- Software de **energía y agua** regional (ITER, desaladoras, energías renovables).
- Proyectos de **smart cities** para ciudades canarias.
- Software sobre **deportes** canarios (CD Tenerife, UD Las Palmas, CB Gran Canaria).
- Herramientas de **agricultura y sector primario** canario (plátano de Canarias, viticultura).

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Canarias — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por canarios que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades canarias que podrían ser genéricos — incluir si tienen datos o configuración específica de Canarias.
- Software que cubre Canarias junto con otras regiones — incluir si Canarias es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución canaria** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-canarias» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades canarias (Reddit, foros de la ULL/ULPGC, Telegram de devs canarios, Python Canarias, Canarias.dev) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- La organización `eDatos` (Gobierno de Canarias / ISTAC) tiene 40+ repos, la mayoría parte del proyecto METAMAC con 0 estrellas. Los repos útiles son los clientes de datos: istacpy (10★), istacr (9★), istacqgis (4★), istacPowerBI (2★).
- `ISTAC` como organización tiene solo 2 repos: FRONTUR_forecast (3★) y SSM_forecast (2★, genérico).
- `pythoncanarias` es una comunidad activa con repos útiles: pycan-web (5★), pydeckard (7★ bot Telegram), eoi (22★ formación EOI).
- `canarias-dev` (15★) es el portal de la comunidad de desarrolladores canarios.
- La búsqueda de "tenerife", "gran canaria", "lanzarote" devuelve muchos resultados de turismo/viajes sin código relevante.
- El IAC no tiene organización GitHub propia; `guaix-ucm/fridadrp` es el pipeline de reducción de datos de FRIDA para el GTC.
- La ULL y ULPGC no tienen organizaciones GitHub oficiales activas.
- `dvarrui/osl.iespto` es la comunidad educativa de software libre del IES Puerto de la Cruz (activo 2026).
- Los repos sobre la erupción de Cumbre Vieja (La Palma 2021) están en eDatos: copernicus-cumbrevieja y dron-cumbrevieja.
- `eDatos/superhub` es un scraper de supermercados en Canarias (nicho pero Canarias-específico).
- `eDatos/opensdg-istac-data` contiene datos de indicadores ODS del ISTAC (activo 2025).
- Rate limits: la API de búsqueda de GitHub (30 req/min) se agota rápido. Usar `gh api repos/...` (core API, 5000/h) para verificar repos conocidos.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
