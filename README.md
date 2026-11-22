# Voltera · Entrega 5 — Arquitectura de IA

Documento de arquitectura del **Grupo 4** para la Entrega 5 de **ARTI-4208 · Arquitecturas de Nueva Generación** (MATI, Universidad de los Andes).

Tema de investigación asignado: **Tema 4 · MCP Server Protocol & Tool Integration**.

> La regla decide, el agente explica, la persona firma, el contrato liquida.

## Ver el documento

Publicado con GitHub Pages: **https://uniandesarquitectura.github.io/voltera-entrega5-doc/**

Es un solo archivo, `index.html`, sin dependencias de compilación. También se abre haciendo doble clic en local.

## Qué contiene

| Sección | Qué cubre |
|---|---|
| Diagrama | Las cinco capas, el flujo del ① al ⑦ y la banda de seguridad |
| 1 · El caso | Compra y venta de energía certificada en el mercado P2P, y por qué cambiamos de caso |
| 2 · Cuándo recomienda | La política de decisión determinista: vender, comprar o esperar |
| 3 · Componentes | Corte mínimo y lo que queda fuera de alcance, con su razón |
| 4 · Herramientas MCP | Los tres servidores, el contexto y los prompts |
| 5 a 9 | Flujo, seguridad, decisiones del tema, ArchiMate y escenarios de calidad |
| 10 a 12 | Experimento, límites conocidos y despliegue objetivo |
| 13 · Anexo | Direcciones de los contratos, unidades, secuencia de transacciones, parámetros y errores |
| 14 · Reparto | Orden de construcción y quién hace qué |

## Actualizarlo

```bash
git clone git@github.com:UniandesArquitectura/voltera-entrega5-doc.git
cd voltera-entrega5-doc
# editar index.html
git add -A && git commit -m "qué cambió" && git push
```

GitHub Pages reconstruye el sitio solo, en un minuto aproximadamente.

El contenido está escrito directo en el HTML, sin generador de sitios. Para cambiar texto, buscar la sección por su `id` (`#diagrama`, `#caso`, `#decision`, `#mcp`, `#anexo`…). El diagrama es un SVG embebido en la sección `#diagrama`: se edita con coordenadas, a mano.

## Nota sobre visibilidad

El sitio lleva `noindex` para no aparecer en buscadores, pero **cualquiera con el enlace puede verlo**. Tenerlo en cuenta antes de sustentar, porque otros grupos del curso trabajan sobre los mismos contratos.

## Código relacionado

Los contratos de la Entrega 4 están en `UniandesArquitectura/BlockchainVoltera`, desplegados en Polygon Amoy (chainId 80002). Las direcciones están en el anexo del documento. **Este repositorio solo contiene documentación: no toca los contratos.**
