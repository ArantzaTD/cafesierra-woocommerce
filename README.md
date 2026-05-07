# ☕ CafeSierra — Tienda en Línea con WooCommerce

![WordPress](https://img.shields.io/badge/WordPress-6.9.4-21759B?style=flat&logo=wordpress)
![WooCommerce](https://img.shields.io/badge/WooCommerce-9.x-96588A?style=flat&logo=woocommerce)
![PHP](https://img.shields.io/badge/PHP-8.2.29-777BB4?style=flat&logo=php)
![MySQL](https://img.shields.io/badge/MySQL-8.4.0-4479A1?style=flat&logo=mysql)

## 📋 Descripción del Proyecto

**CafeSierra** es una tienda en línea funcional de comercio electrónico desarrollada con **WordPress 6.9.4** y **WooCommerce** como parte de la Práctica 7 de la materia *Desarrollo de Sitios Web* — BUAP FCC Otoño 2025.

La tienda está especializada en **café de especialidad mexicano**, ofreciendo productos de distintas regiones del país: Oaxaca, Veracruz y Chiapas, en diferentes presentaciones (grano, molido, instantáneo, cápsulas y kits de degustación).

---

## 🎯 Tema Elegido

**Café de especialidad mexicano** — CafeSierra conecta a consumidores con los mejores granos de café de origen nacional, con trazabilidad de región y proceso de tostado artesanal.

### Catálogo de productos:
| # | Producto | Categoría | Precio |
|---|----------|-----------|--------|
| 1 | Café en grano Oaxaca 500g | Café en grano | $189 MXN |
| 2 | Café Molido Veracruz 250g | Café molido | $129 MXN |
| 3 | Café Orgánico Chiapas 1kg | Café orgánico | $349 MXN |
| 4 | Café Instantáneo Sierra Gold 200g | Café instantáneo | $99 MXN |
| 5 | Cápsulas Nespresso x10 | Cápsulas | $149 MXN |
| 6 | Kit Degustación 3 Orígenes | Kits y regalos | $279 MXN |

---

## 🛠️ Tecnologías Utilizadas

- **CMS:** WordPress 6.9.4
- **E-commerce:** WooCommerce
- **Tema:** Storefront (oficial de WooCommerce)
- **SEO:** Yoast SEO
- **Seguridad:** Wordfence Security
- **Entorno local:** LocalWP 10.1.0
- **Servidor:** Nginx
- **Base de datos:** MySQL 8.4.0
- **PHP:** 8.2.29

---

## 🚀 Pasos para Ejecutar el Sitio en Local

### Requisitos previos
- Tener instalado [LocalWP](https://localwp.com/) en tu computadora
- Tener instalado un cliente MySQL (incluido en LocalWP)

### Instrucciones

**1. Clona el repositorio**
```bash
git clone https://github.com/TU_USUARIO/cafesierra-woocommerce.git
cd cafesierra-woocommerce
```

**2. Crea un nuevo sitio en LocalWP**
- Abre LocalWP
- Clic en **"+"** para crear nuevo sitio
- Nombre: `CafeSierra`
- Configuración: Preferred (PHP 8.2, Nginx, MySQL 8.4)
- Completa el asistente

**3. Reemplaza la carpeta wp-content**
- Ve a la carpeta de tu sitio en LocalWP:  
  `C:\Users\TU_USUARIO\Local Sites\cafesierra\app\public\`
- Reemplaza la carpeta `wp-content` con la del repositorio

**4. Importa la base de datos**
- En LocalWP → pestaña **Database** → **Open Adminer**
- Selecciona la base de datos de tu sitio
- Clic en **Importar** → selecciona el archivo `database/cafesierra.sql`

**5. Actualiza la URL del sitio**
- En Adminer, ve a la tabla `wp_options`
- Busca `siteurl` y `home`
- Cambia el valor a `http://cafesierra.local`

**6. Inicia el sitio**
- En LocalWP → clic en **"Start site"**
- Abre tu navegador en: `http://cafesierra.local`
- Panel de administración: `http://cafesierra.local/wp-admin`
  - Usuario: `admin`
  - Contraseña: la que configuraste al crear el sitio

---

## 📁 Estructura del Repositorio

```
cafesierra-woocommerce/
│
├── wp-content/
│   ├── themes/
│   │   └── storefront/          # Tema principal
│   ├── plugins/
│   │   ├── woocommerce/         # Plugin de e-commerce
│   │   ├── wordpress-seo/       # Yoast SEO
│   │   └── wordfence/           # Seguridad
│   └── uploads/                 # Imágenes de productos
│
├── database/
│   └── cafesierra.sql           # Base de datos exportada
│
└── README.md
```

---

## ⚙️ Configuración de WooCommerce

| Ajuste | Valor |
|--------|-------|
| País | México |
| Moneda | Peso mexicano (MXN) |
| Métodos de pago | Transferencia bancaria, Contra entrega |
| Envío nacional | Tarifa fija $80 MXN |
| Envío Puebla | Gratis |

---

## 🔒 Seguridad Implementada

- ✅ Wordfence Security (Firewall + Malware Scanner)
- ✅ Contraseñas seguras para usuarios admin
- ✅ WordPress y plugins actualizados a última versión
- ✅ Respaldo de base de datos SQL incluido en el repositorio

---

## 📈 SEO Aplicado

- ✅ Yoast SEO configurado con meta título y descripción
- ✅ Sitemap XML generado automáticamente
- ✅ URLs amigables (permalinks por nombre)
- ✅ Imágenes con texto alternativo descriptivo
- ✅ Estructura semántica H1/H2 en todas las páginas

---

## 👥 Integrantes del Equipo

| Nombre | Matrícula |
|--------|-----------|
| [Arantza Tenorio] | [202254883] |


---

## 📚 Materia

**Desarrollo de Sitios Web**  
M.C. Luis Yael Méndez Sánchez  
Facultad de Ciencias de la Computación — BUAP  
Primavera 2026
