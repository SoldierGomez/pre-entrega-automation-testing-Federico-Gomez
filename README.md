# README — Proyecto de automatización con pytest

## Propósito
Automatizar pruebas funcionales/end-to-end de la aplicación web [SauceDemo](https://www.saucedemo.com/) para verificar flujos críticos (login, búsqueda, formularios, compras, etc.) y detectar regresiones en cada despliegue.



## Tecnologías
- Python 3.10+  
- pytest  
- Selenium
- pytest-html (reportes)
- pip (gestor de dependencias)  
- Git (control de versiones)

## Requisitos previos
1. Python 3.10+ instalado.  
2. Navegador compatible (Chrome/Chromium o Firefox).  
3. Drivers del navegador instalados (ChromeDriver).

## Instalación de dependencias
1. Clonar el repositorio:
```bash
git clone git@github.com:SoldierGomez/pre-entrega-automation-testing-Federico-Gomez.git
cd git@github.com:SoldierGomez/pre-entrega-automation-testing-Federico-Gomez.git
```

2. Instalar dependencias:
```bash
pip install -r requirements.txt
```

## Cómo ejecutar las pruebas
1. Ejecutar todas las pruebas:
```bash
pytest tests/test_sausedemo.py
```
2. Ejecutar un archivo o test específico:
```bash
pytest tests/test_sausedemo.py::<NOMBRE_DEL_TEST>
```
3. Generar reporte HTML:
```bash
pytest tests/test_sausedemo.py --html=reports/report.html
```


## Estructura del proyecto
- tests/                — casos de prueba (por módulo/feature)  
- utils/                — helpers/utilidades (waits, data builders)  
- conftest.py           — fixtures de pytest 
- reporte_Tests.html    — reporte
- requirements.txt      — dependencias


## Contribuir
1. Crear branch: feature/<descripcion>
2. Añadir tests y documentación.
3. Abrir PR y asignar revisores.
4. Asegurarse que CI pasa y los reportes se generan.

## Contacto
- Contacto: fedenogues@gmail.com
