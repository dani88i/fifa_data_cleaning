<h1>🧹 Data Cleaning and Transformation in Jupyter Notebook</h1>

<p>Este proyecto se enfoca en la limpieza y transformación de columnas específicas de un conjunto de datos para cumplir con los requisitos comunes de procesamiento de datos. A continuación, se explican los pasos y transformaciones aplicadas para asegurar que el conjunto de datos esté listo para su análisis y modelado. 🚀</p>

<h2>📑 Tabla de Contenidos</h2>
<ol>
  <li><a href="#verificacion-de-tipos-de-datos"> ✅ Verificación de Tipos de Datos</a></li>
  <li><a href="#separacion-de-la-columna-fecha"> 📅 Separación de la Columna Fecha</a></li>
  <li><a href="#limpieza-y-transformacion-de-las-columnas-valor-salario-y-clausula"> 💰 Limpieza y Transformación de las Columnas Valor, Salario y Cláusula de Rescisión</a></li>
  <li><a href="#eliminacion-de-caracteres-de-nueva-linea-en-la-columna-hits"> 🧽 Eliminación de Caracteres de Nueva Línea en la Columna Hits</a></li>
  <li><a href="#separacion-de-la-columna-equipo-y-contrato"> 📝 Separación de la Columna Equipo y Contrato</a></li>
</ol>

<h2 id="verificacion-de-tipos-de-datos">1. ✅ Verificación de Tipos de Datos</h2>
<p><strong>Objetivo:</strong> Asegurar que las columnas de <code>Height</code> y <code>Weight</code> tengan los tipos de datos apropiados para análisis numérico.</p>
<p><strong>Enfoque:</strong> Se inspeccionaron los tipos de datos de estas columnas usando métodos como <code>dtypes</code> de pandas para verificar si son numéricos. En caso de ser necesario, se realizó la conversión usando <code>astype(float)</code> para que los valores sean correctos. 🏋️‍♂️📏</p>

<h2 id="separacion-de-la-columna-fecha">2. 📅 Separación de la Columna Fecha</h2>
<p><strong>Objetivo:</strong> Dividir la columna que contiene información de fecha en tres columnas separadas: <code>Año</code>, <code>Mes</code>, y <code>Día</code>.</p>
<p><strong>Enfoque:</strong> Utilizamos <code>str.split()</code> para separar la fecha, y aseguramos que los tipos de datos resultantes fueran apropiados para un análisis adecuado. Esto facilita trabajar con datos temporales de manera más granular. 🕰️</p>

<h2 id="limpieza-y-transformacion-de-las-columnas-valor-salario-y-clausula">3. 💰 Limpieza y Transformación de las Columnas Valor, Salario y Cláusula de Rescisión</h2>
<p><strong>Objetivo:</strong> Transformar las columnas <code>Value</code>, <code>Wage</code> y <code>Release Clause</code> a valores enteros, eliminando caracteres no numéricos como símbolos monetarios.</p>
<p><strong>Enfoque:</strong> Se limpiaron estas columnas eliminando caracteres como <code>€</code> y <code>K</code> con <code>str.replace()</code>, y posteriormente se convirtieron los datos a enteros utilizando <code>astype(int)</code>. Esto permite realizar análisis cuantitativos precisos. 💶➡️💵</p>

<h2 id="eliminacion-de-caracteres-de-nueva-linea-en-la-columna-hits">4. 🧽 Eliminación de Caracteres de Nueva Línea en la Columna Hits</h2>
<p><strong>Objetivo:</strong> Limpiar la columna <code>Hits</code> eliminando los caracteres de nueva línea (<code>\n</code>) que interfieren con el formato.</p>
<p><strong>Enfoque:</strong> Se usó el método <code>str.replace()</code> para eliminar estos caracteres, dejando la columna en un formato limpio y fácil de usar. Esto ayuda a evitar problemas en la visualización o análisis de los datos. 🧼🧹</p>

<h2 id="separacion-de-la-columna-equipo-y-contrato">5. 📝 Separación de la Columna Equipo y Contrato</h2>
<p><strong>Objetivo:</strong> Dividir la columna <code>Team & Contract</code> en dos columnas separadas: <code>Team</code> y <code>Contract</code>, para una estructura de datos más clara.</p>
<p><strong>Enfoque:</strong> Se utilizó <code>str.split()</code> para dividir la columna según el separador adecuado (como un guion o espacio), logrando que los datos de <code>Equipo</code> y <code>Contrato</code> queden bien estructurados y fáciles de analizar. ⚽📝</p>

<p>¡Gracias por consultar el proyecto! Esperamos que estas transformaciones mejoren la calidad de tus datos para un análisis más eficiente. 📊🔧</p>
