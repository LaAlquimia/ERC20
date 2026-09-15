# 🏛️ Evolución de la Programabilidad Descentralizada y Estándar ERC-20

> **Material de Cátedra e Investigación Técnica**  
> **Semillero de Investigación en Blockchain — Universidad de Antioquia (UdeA)**  
> Desarrollado por: **La Alquimia**

---

## 📌 Descripción General

Este repositorio reúne la investigación monográfica formal y el material de proyección pedagógico sobre la evolución de las tecnologías de registro distribuido (DLT) y la arquitectura de contratos inteligentes, desde la génesis de Bitcoin hasta la especificación técnica profunda del estándar **ERC-20 (EIP-20)** en la Máquina Virtual de Ethereum (EVM).

El proyecto ha sido concebido como material de referencia académica para estudiantes, investigadores y desarrolladores del **Semillero de Blockchain de la Universidad de Antioquia**, combinando rigor matemático-computacional con análisis de seguridad en producción.

---

## 📂 Contenido del Repositorio

| Archivo | Formato | Descripción |
| :--- | :--- | :--- |
| [`poster_clase_udea.html`](./poster_clase_udea.html) | HTML5 / CSS Imprimible | **Afiche Publicitario y Poster Académico:** Formato vertical de alta resolución (proporción publicitaria y A4 imprimible con `@media print`) para la Cátedra Abierta y Masterclass UdeA & La Alquimia (Viernes 2:00 PM). |
| [`reporte_erc20.md`](./reporte_erc20.md) | Markdown | **Monografía Técnica Completa (50+ KB):** Cronología evolutiva (Bitcoin, DLT, Ethereum, EVM), ontología de cuentas, especificación formal del estándar ERC-20, interfaces Solidity documentadas en NatSpec, vectores de ataque en mempool, desbordamientos, reentrancia y estándares complementarios. |
| [`presentacion_erc20.html`](./presentacion_erc20.html) | HTML5 / Vanilla JS | **Diapositivas Interactivas Universitarias (87 KB):** Presentación autocontenida de 18 diapositivas con la identidad visual institucional de la Universidad de Antioquia (UdeA), motor de navegación por teclado, soporte táctil (swipe), modo pantalla completa y vista en cuadrícula (overview). |
| [`CURSO_TOKENIZACION.md`](./CURSO_TOKENIZACION.md) | Markdown | **Programa Formativo Intensivo (4 Clases):** Diseño pedagógico gamificado y práctico para el Semillero UdeA (Remix IDE, evolución Truffle/Hardhat/Foundry, DeFi AMMs, hackeo defensivo de mempool y tokenización RWA). |

---

## 🖥️ Cómo Visualizar las Diapositivas (`presentacion_erc20.html`)

El archivo es **100% autocontenido** (no requiere instalar paquetes de Node.js ni configurar servidores web complejos).

### Opción 1: Apertura Directa
Haz doble clic sobre el archivo `presentacion_erc20.html` o ábrelo directamente desde tu navegador preferido (Chrome, Firefox, Safari, Edge, Brave).

### Opción 2: Servidor Local Rápido (Opcional)
Si deseas servirlo localmente mediante terminal:
```bash
# Con Python 3
python3 -m http.server 8000

# O con npx
npx serve .
```
Luego ingresa en tu navegador a: `http://localhost:8000/presentacion_erc20.html`

---

## ⌨️ Controles de Navegación de la Presentación

- **Avanzar Diapositiva:** `Flecha Derecha`, `Barra Espaciadora` o `AvPág`.
- **Retroceder Diapositiva:** `Flecha Izquierda` o `RePág`.
- **Inicio / Fin:** Teclas `Home` (primera diapositiva) y `End` (última diapositiva).
- **Modo Pantalla Completa:** Presiona `F` para activar o desactivar la vista completa para proyector.
- **Vista en Cuadrícula / Índice:** Presiona `O` o `Esc` para abrir el selector rápido de diapositivas.
- **Menú de Ayuda:** Presiona `?` en cualquier momento.
- **Dispositivos Móviles y Tablets:** Desliza el dedo horizontalmente (*swipe*) para cambiar de diapositiva.

---

## 🗺️ Mapa Temático del Reporte y Presentación

```mermaid
flowchart LR
    A["1. Bitcoin (2008)<br/>Modelo UTXO & Script"] --> B["2. Blockchain & DLT<br/>Consenso, Hashes & Merkle"]
    B --> C["3. Ethereum (2015)<br/>EVM & Smart Contracts"]
    C --> D["4. Estándar ERC-20<br/>EIP-20 & Fungibilidad"]
    D --> E["5. Operatividad & Seguridad<br/>Approve/TransferFrom & Attacks"]
    E --> F["6. Ecosistema & Futuro<br/>DeFi, RWAs & ERC-4337"]
```

1. **Bitcoin y el Dinero Programable:** Resolución del doble gasto, modelo de salidas no gastadas (UTXO) y limitaciones del lenguaje Bitcoin Script.
2. **Fundamentos Criptográficos y de Consenso:** Criptografía asimétrica (ECDSA secp256k1), hashes Keccak-256, árboles Merkle-Patricia y transición de PoW a PoS.
3. **Ethereum y la EVM:** La computadora mundial de Turing, modelo de cuentas (EOA vs Contract Accounts), Trie de almacenamiento y el Gas como solución al Halting Problem.
4. **Génesis y Especificación de ERC-20:** EIP-20, metadatos, funciones obligatorias (`totalSupply`, `balanceOf`, `transfer`, `approve`, `allowance`, `transferFrom`) y eventos indexados en el Bloom filter.
5. **Flujos Operativos y Riesgos de Seguridad:** Transferencia directa vs delegada, condiciones de carrera en mempool (front-running de approve), SafeMath vs Solidity 0.8+, patrones Checks-Effects-Interactions y arquitectura OpenZeppelin v5.
6. **Ecosistema y Horizontes Futuros:** Integración en DeFi, DAOs y RWAs; matriz comparativa (ERC-721, ERC-1155, ERC-4626) y abstracción de cuentas (ERC-4337).

---

## 🏛️ Créditos y Licencia

- **Institución:** Universidad de Antioquia (UdeA) — Medellín, Colombia.
- **Grupo:** Semillero de Investigación en Blockchain.
- **Autoría Técnica:** **La Alquimia**.
- **Licencia:** MIT License. Material de libre consulta, divulgación académica y desarrollo formativo.
