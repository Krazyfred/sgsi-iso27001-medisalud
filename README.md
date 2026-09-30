# SGSI para una cadena de clínicas privadas (ISO 27001 · MAGERIT)

Diseño de la primera versión de un **Sistema de Gestión de Seguridad de la Información (SGSI)** para *Medisalud Integral S.A.*, una empresa ficticia de clínicas privadas que trabaja con historiales clínicos, teleconsulta, imagen médica (PACS) y facturación electrónica.

📄 **[Informe completo (PDF, 22 págs.)](Informe_SGSI_Medisalud.pdf)**

> Trabajo en grupo de la asignatura *Garantía y Seguridad de la Información* (3º Grado en Ingeniería Informática, itinerario de Tecnologías de la Información, Universidad de Valladolid, diciembre 2025).

## Metodología

Análisis y gestión de riesgos siguiendo **MAGERIT v3** y el marco **ISO/IEC 27001**, teniendo en cuenta el **RGPD** y la **LOPDGDD**, ya que se tratan datos de salud (categoría especial).

1. **Contexto de la organización**: departamentos, infraestructura IT (VMware vSphere, OpenEMR, OsiriX PACS, A3 ERP, SQL Server, AWS/Azure, FortiGate, Snort, MFA con Duo), servicios y requisitos de acceso internos y externos.
2. **Catálogo de activos**: datos, servicios, software, hardware, redes, instalaciones y personal, valorados según su criticidad.
3. **Catálogo de amenazas**: desastres naturales, de origen industrial, errores y fallos no intencionados, y ataques intencionados.
4. **Análisis de riesgos**: riesgo = impacto × probabilidad (escala 1–5) y priorización con una matriz de riesgo.
5. **Salvaguardas**, organizadas por dimensión de seguridad (confidencialidad, integridad, disponibilidad y cumplimiento normativo) y por tipo de activo.
6. **Controles del SGSI**: organizacionales, técnicos, físicos, de comunicaciones y legales.

## Resultados destacados

- **Riesgos críticos (25/25):** abuso de privilegios de acceso y difusión de software dañino.
- **Riesgos altos (16/25):** denegación de servicio, suplantación de identidad, robo de información, fallo del servicio de comunicaciones y errores de los usuarios.
- **Salvaguardas clave:** MFA y control de acceso por roles, cifrado de discos y de datos personales, segmentación de red en VLAN, WPA3 y aislamiento de la wifi de invitados, *hardening* de VMware, copias de seguridad locales y en la nube con pruebas de restauración periódicas, y SAI y detección de incendios.

## Autores

Grupo P2-3: Luis Antón, **Alfredo del Val** ([@Krazyfred](https://github.com/Krazyfred)), Daniel Sanabria y Roi Suárez.
