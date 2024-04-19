# Comparing `tmp/outputstyles-0.1.2.tar.gz` & `tmp/outputstyles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outputstyles-0.1.2.tar", last modified: Sun Aug 27 22:42:38 2023, max compression
+gzip compressed data, was "outputstyles-0.1.3.tar", last modified: Fri Apr 19 20:47:23 2024, max compression
```

## Comparing `outputstyles-0.1.2.tar` & `outputstyles-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-27 22:42:38.135377 outputstyles-0.1.2/
--rw-rw-rw-   0        0        0     1101 2023-08-26 23:34:28.000000 outputstyles-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1470 2023-08-27 22:42:38.135377 outputstyles-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      942 2023-08-27 22:42:26.000000 outputstyles-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-27 22:42:38.129380 outputstyles-0.1.2/outputstyles/
--rw-rw-rw-   0        0        0       58 2023-08-26 23:46:15.000000 outputstyles-0.1.2/outputstyles/__init__.py
--rw-rw-rw-   0        0        0     4389 2023-08-27 18:41:26.000000 outputstyles-0.1.2/outputstyles/apply_styles.py
--rw-rw-rw-   0        0        0     2616 2023-08-27 18:41:41.000000 outputstyles-0.1.2/outputstyles/msg_print.py
--rw-rw-rw-   0        0        0     2006 2023-08-27 00:33:07.000000 outputstyles-0.1.2/outputstyles/variables.py
-drwxrwxrwx   0        0        0        0 2023-08-27 22:42:38.134377 outputstyles-0.1.2/outputstyles.egg-info/
--rw-rw-rw-   0        0        0     1470 2023-08-27 22:42:38.000000 outputstyles-0.1.2/outputstyles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-08-27 22:42:38.000000 outputstyles-0.1.2/outputstyles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-27 22:42:38.000000 outputstyles-0.1.2/outputstyles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-27 22:42:38.000000 outputstyles-0.1.2/outputstyles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-27 22:42:38.135377 outputstyles-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-08-27 22:41:34.000000 outputstyles-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.355644 outputstyles-0.1.3/
+-rw-rw-rw-   0        0        0     1101 2023-08-26 23:34:28.000000 outputstyles-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4590 2024-04-19 20:47:23.354645 outputstyles-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4036 2024-04-19 20:46:30.000000 outputstyles-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.340653 outputstyles-0.1.3/outputstyles/
+-rw-rw-rw-   0        0        0      527 2024-02-09 01:16:19.000000 outputstyles-0.1.3/outputstyles/__init__.py
+-rw-rw-rw-   0        0        0     5263 2024-04-19 19:58:21.000000 outputstyles-0.1.3/outputstyles/apply_styles.py
+-rw-rw-rw-   0        0        0     2551 2024-02-09 00:58:05.000000 outputstyles-0.1.3/outputstyles/msg_type.py
+-rw-rw-rw-   0        0        0     2107 2024-04-19 19:55:09.000000 outputstyles-0.1.3/outputstyles/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:47:23.354645 outputstyles-0.1.3/outputstyles.egg-info/
+-rw-rw-rw-   0        0        0     4590 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 20:47:23.000000 outputstyles-0.1.3/outputstyles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 20:47:23.356644 outputstyles-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2024-04-19 20:31:45.000000 outputstyles-0.1.3/setup.py
```

### Comparing `outputstyles-0.1.2/LICENSE` & `outputstyles-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `outputstyles-0.1.2/outputstyles/apply_styles.py` & `outputstyles-0.1.3/outputstyles/apply_styles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,147 @@
 """
 Funciones para aplicar los estilos al texto.
 """
 
-# Importar desde las variables, todos los estilos
-from outputstyles.variables import all_styles
+# Importar todos los estilos que se le pueden aplicar al texto.
+from outputstyles import all_styles
 
 
-def add_text_styles(text, styles=[]):
+def add_text_styles(text: str, styles: list = [], all_styles: dict = all_styles) -> str:
     """
     Aplicarles los estilos al texto.
 
     Parameters:
-    text (str): Texto al que se le van a aplicar los estilos
-    styles (list): Lista de estilos que se le van a aplicar al texto
+    text (str): Texto al que se le van a aplicar los estilos.
+    styles (list) [Opcional]: Lista de estilos que se le van a aplicar al texto.
+    all_styles (dict): Diccionario con todos los estilos posibles.
 
     Returns:
-    srt: Devuelve el texto con los estilos aplicados
+    srt: Devuelve el texto con los estilos aplicados.
     """
 
-    # Lista resultante de los estilos que se van a aplicar
+    # Comprobar que existan estilos en los argumentos y que sea una lista.
+    if not styles or type(styles) != list:
+        return text
+
+    # Lista resultante de los estilos que se van a aplicar.
     list_styles = []
 
-    # Recorrer todos los estilos pasados como argumentos e ir aplicandolos
+    # Resetear estilos al final del texto.
+    style_reset = all_styles["reset"]
+
+    # Aplicar los estilos.
     for style in styles:
-        # Tratar de asignar el estilo de turno
+
+        # Asignar el estilo de turno.
         try:
-            # Agregar el valor del estilo a la lista resultante
+
+            # Agregar el valor del estilo a la lista resultante.
             list_styles.append(all_styles[style])
 
-        # En caso de que no exista el estilo, lo imprimimos como un error
+        # En caso de que no exista el estilo (key), imprimimos un error.
         except KeyError:
+
+            # Definir los diferentes estilos del mensaje de error.
+            text_bold = all_styles["bold"]
+            text_error = all_styles["fg_red"]
+
+            # Imprimir mensaje de error.
             print(
-                f'No exite el estilo: \033[1;31m{style}{all_styles["reset"]}')
+                f'\033[{text_bold}mEstilo no válido:{style_reset}',
+                f'\033[{text_bold};{text_error}m{style}{style_reset}'
+            )
 
     # Concatenamos los estilos separados por ";" con el texto,
-    # además de agregarle "\033[" y "m" para que sea válido el código ANSI
+    # además de agregarle "\033[" y "m" para que sea válido el código ANSI.
     # Ej: \033[01;91mTexto
     text_with_styles = f'\033[{";".join(list_styles)}m{text}'
 
-    # Retornamos el texto con los estilos aplicados, al inicio y al final de este reseteamos los estilos
-    return f'{all_styles["reset"]}{text_with_styles}{all_styles["reset"]}'
+    # Retornamos el texto con los estilos aplicados,
+    # al inicio y al final reseteamos los estilos.
+    return f'{style_reset}{text_with_styles}{style_reset}'
 
 
-def create_arg(color=None, msg_format=None):
+def create_arg(color: str = "", msg_format: str = "") -> list:
     """
     Crear una Lista de los estilos que se le van a aplicar al texto
     en dependencia del tipo de mensaje.
 
     Parameters:
-    color (str): Color del texto (Valor por defecto es 'None')
-    msg_format (str): Formato del tipo de mensaje ('ico', 'btn', 'btn_ico')
+    color (str) [Opcional]: Color del texto.
+    msg_format (str) [Opcional]: Formato del tipo de mensaje ('ico', 'btn', 'btn_ico')
 
     Returns:
-    list (str): Devuelve una lista con los estilos a aplicar,
-    - Si no tiene ningún color, devuelve el estilo en Negrita (bold)
-    - Si no tiene formato o es de tipo icono, devuelve Negrita y el color del Texto (bold, fg_color)
-    - Si es de tipo Botón o Botón con Icono, devuelve Negrita, color del Texto y del Fondo (bold, fg_color, bg_color)
+    list: Devuelve una lista con los estilos a aplicar.
+    - Si no tiene ningún color o el formato no es válido, devuelve el estilo en Negrita [bold]
+    - Si es de tipo Botón, con Icono o no, devuelve Negrita, color del Texto y del Fondo [bold, fg_color, bg_color]
+    - Por defecto, devuelve Negrita y el color del Texto [bold, fg_color]
     """
 
-    # En caso de que no se especifique ningún color
-    if not color:
-        # Retornamos solamente el estilo en "Negrita"
+    # Comprobar si tiene color el texto y es un formato válido.
+    if not color or not msg_format in ["", "ico", "btn", "btn_ico"]:
+
+        # Texto en Negrita.
         return ["bold"]
 
-    # Si el mensaje tiene el Icono inicialmete o es solo el texto
-    if msg_format == "ico" or not msg_format:
-        # Retornamos el estilo en "Negrita" y el color del texto según el tipo de mensaje
-        return ["bold", f'fg_{color}']
+    # Mensaje de tipo Botón, ya sea con icono o no.
+    if msg_format in ["btn", "btn_ico"]:
+
+        # Texto en Negrita, color en blanco y fondo según el color del argumento.
+        return ['bold', 'fg_light_white', f'bg_{color}']
+
+    # Retornamos por defecto el texto en Negrita y con el color del argumento.
+    return ['bold', f'fg_{color}']
+
+
+def add_icono(text: str, msg_format: str = "", ico_code: str = "") -> str:
+    """
+    Agregarle un icono delante del texto del mensaje.
+
+    Parameters:
+    text (str): Texto al que se le va a agregar el icono.
+    msg_format (str) [Opcional]: Formato del tipo de mensaje ('ico', 'btn', 'btn_ico').
+    ico_code (str) [Opcional]: Código del icono que se va a agregar.
+
+    Returns:
+    srt: Devuelve el texto con icono o no según corresponda.
+    """
 
-    # Si el mensaje es de tipo Botón o de Botón con icono
-    elif msg_format == "btn" or msg_format == "btn_ico":
-        # Retornamos el estilo en "Negrita", el color del texto en blanco y color de fondo según el tipo de mensaje
-        return ["bold", f'fg_white2', f'bg_{color}']
+    # Comprobar si tiene icono el texto y es un formato válido.
+    if not ico_code or not msg_format in ["ico", "btn_ico"]:
+        return text
 
+    # Si es de tipo Botón con Icono el mensaje.
+    if msg_format == "btn_ico":
 
-# Función que retorna el código del Texto con los estilos aplicados según su formato
-def print_message(text, msg_format=None, message_data=None):
+        # Concatenamos el icono al inicio del texto, dejando un espacio al inicio y final.
+        return f' {ico_code} {text} '
+
+    # Concatenamos el icono al inicio del texto.
+    return f'{ico_code} {text}'
+
+
+def apply_styles(text: str, msg_format: str = "", message_data: dict = {}) -> str:
     """
-    Retornar el código del texto con los estilos aplicados, según el tipo de mensaje.
+    Retornar el texto con los estilos aplicados, según el tipo de mensaje.
 
     Parameters:
-    text (str): Texto al que se le van a aplicar los estilos
-    msg_format (str): Formato del tipo de mensaje ('ico', 'btn', 'btn_ico')
-    message_data (dic): Datos del tipo de mensaje (error_data, warning_data, success_data, info_data)
+    text (str): Texto al que se le van a aplicar los estilos.
+    msg_format (str) [Opcional]: Formato del tipo de mensaje ('ico', 'btn', 'btn_ico').
+    message_data (dict) [Opcional]: Datos del tipo de mensaje (error_data, warning_data, success_data, info_data).
 
     Returns:
-    srt: Devuelve el código del texto con los estilos aplicados
+    srt: Devuelve el texto con los estilos aplicados.
     """
 
-    # Si el mensaje tiene el icono inicialmente
-    if msg_format == "ico":
-        # Concatenamos el texto con el icono inicialmente
-        text = f'{message_data["ico_code"]} {text}'
-
-    # Si el mensaje es de tipo botón y con el icono inicialmente
-    elif msg_format == "btn_ico":
-        # Concatenamos el texto con el icono inicialmente, dejando un espacio al inicio y final
-        text = f' {message_data["ico_code"]} {text} '
-
-    # Lista de los estilos que se le van a aplicar al texto, según el tipo de mensaje
-    if message_data:
-        # Aplicar los estilos según los datos del tipo de mensaje
-        list_styles = create_arg(message_data['color'], msg_format)
-    else:
-        # Solo aplicar el estilo de Negrita al texto
-        list_styles = create_arg()
+    # Obtener los valores de los datos del mensaje.
+    ico_code = message_data.get("ico_code", "")
+    color = message_data.get("color", "")
+
+    # Agregar el icono en caso de que lo lleve.
+    text = add_icono(text, msg_format, ico_code)
+
+    # Obtener la Lista de los estilos que se le van a aplicar al texto.
+    list_styles = create_arg(color, msg_format)
 
-    # Retornamos el código del texto con los estilos aplicados
+    # Retornamos el código del texto con los estilos aplicados.
     return add_text_styles(text, list_styles)
```

### Comparing `outputstyles-0.1.2/outputstyles/variables.py` & `outputstyles-0.1.3/outputstyles/variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,105 @@
 """
-Variables con todos los Estilos que se le pueden aplicar a los textos
-y los datos de los diferentes tipos de mensajes
+Variables con todos los Estilos que se le pueden aplicar
+a los textos y los datos de los diferentes tipos de mensajes.
 """
 
 all_styles = {
-    # Formatos
+
+    # Modificadores.
     'reset': '\033[0m',
     'bold': '01',
     'disabled': '02',
     'italic': '03',
     'underline': '04',
     'blink': '05',
     'blink2': '06',
     'reverse': '07',
-    'invisible': '08',
+    'hidden': '08',
     'strike_through': '09',
 
-    # Colores del Texto
+    # Colores del Texto.
     'fg_black': '30',
     'fg_red': '31',
     'fg_green': '32',
     'fg_yellow': '33',
     'fg_blue': '34',
     'fg_magenta': '35',
     'fg_cyan': '36',
     'fg_white': '37',
-    'fg_black2': '90',
-    'fg_red2': '91',
-    'fg_green2': '92',
-    'fg_yellow2': '93',
-    'fg_blue2': '94',
-    'fg_magenta2': '95',
-    'fg_cyan2': '96',
-    'fg_white2': '97',
+    'fg_light_black': '90',
+    'fg_light_red': '91',
+    'fg_light_green': '92',
+    'fg_light_yellow': '93',
+    'fg_light_blue': '94',
+    'fg_light_magenta': '95',
+    'fg_light_cyan': '96',
+    'fg_light_white': '97',
 
-    # Colores del Fondo
+    # Colores del Fondo.
     'bg_black': '40',
     'bg_red': '41',
     'bg_green': '42',
     'bg_yellow': '43',
     'bg_blue': '44',
     'bg_magenta': '45',
     'bg_cyan': '46',
     'bg_white': '47',
-    'bg_black2': '100',
-    'bg_red2': '101',
-    'bg_green2': '102',
-    'bg_yellow2': '103',
-    'bg_blue2': '104',
-    'bg_magenta2': '105',
-    'bg_cyan2': '106',
-    'bg_white2': '107',
+    'bg_light_black': '100',
+    'bg_light_red': '101',
+    'bg_light_green': '102',
+    'bg_light_yellow': '103',
+    'bg_light_blue': '104',
+    'bg_light_magenta': '105',
+    'bg_light_cyan': '106',
+    'bg_light_white': '107',
 }
 """
 Contiene todos los estilos que se le pueden aplicar a los textos:
-- Formato (Bold, Underline, etc)
-- Color del Texto (Red, Black, Green, etc)
-- Color del Fondo (Red, Black, Green, etc)
+- Modificadores (Bold, Underline, etc).
+- Color del Texto (Red, Black, Green, etc).
+- Color del Fondo (Red, Black, Green, etc).
 """
 
 
 error_data = {
     "ico_code": "\u2718",
     "color": "red"
 }
 """
-Datos del Mensaje de tipo 'Error'
+Datos del Mensaje de tipo 'Error'.
 - Icono: \u2718
 - Color: Red
 """
 
 
 warning_data = {
     "ico_code": "\u26A0",
     "color": "yellow"
 }
 """
-Datos del Mensaje de tipo 'Warning'
+Datos del Mensaje de tipo 'Warning'.
 - Icono: \u26A0
 - Color: Yellow
 """
 
 
 success_data = {
     "ico_code": "\u2714",
     "color": "green"
 }
 """
-Datos del Mensaje de tipo 'Success'
+Datos del Mensaje de tipo 'Success'.
 - Icono: \u2714
 - Color: Green
 """
 
 
 info_data = {
     "ico_code": "\u24D8",
     "color": "blue"
 }
 """
-Datos del Mensaje de tipo 'Info'
+Datos del Mensaje de tipo 'Info'.
 - Icono: \u24D8
 - Color: Blue
 """
```

### Comparing `outputstyles-0.1.2/setup.py` & `outputstyles-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 # La descripción larga va a ser el mismo fichero README.md
 long_desc = Path("README.md").read_text()
 
 # Datos del paquete
 setup(
     name="outputstyles",
-    version="0.1.2",
+    version="0.1.3",
     author="Duniesky Salazar Pérez",
     author_email="<duniesky.salazar@gmail.com>",
     description="Applying styles to CLI output",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://github.com/dunieskysp/output_styles',
-    packages=find_packages(),
-    keywords=['python', 'output styles'],
+    packages=find_packages(
+        exclude=["module"]
+    ),
+    keywords=['python', 'outputstyles', 'CLI styles', 'text styles'],
     classifiers=[
-            "Development Status :: 3 - Alpha",
-            "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
+        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python :: 3",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ]
 
 )
```

