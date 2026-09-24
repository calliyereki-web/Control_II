
```text
# 📄 Proyecto de Reportes en LaTeX

Este repositorio contiene la plantilla y los archivos fuente en LaTeX para la elaboración de los reportes del curso.

```

---

## 🚀 Guía de inicio y clonación

La configuración inicial de este entorno se basó en el tutorial:

* 📹 **Video de referencia:** [GitHub LaTeX en VS Code [sencillo]](https://www.youtube.com/watch?v=IJV35V3H9Xc&utm_source=gemini)

> 💡 **Nota:** Para ver el proceso específico de clonación del repositorio en tu computadora usando GitHub Desktop y VS Code, consulta el video a partir del minuto **02:15**.

---

## 🛠️ Requisitos de software

Para trabajar y compilar los documentos localmente, asegúrate de tener instalado:

1. **Visual Studio Code** con la extensión **LaTeX Workshop**.
2. **MiKTeX** (o TeX Live).
3. **Git** o **GitHub Desktop**.

---

## ⚠️ Solución al error común de compilación (`latexmk` / Perl)

Al compilar por primera vez en Windows usando `latexmk`, es muy común que aparezca el siguiente error en la consola:

```text
Sorry, but latexmk did not succeed for the following reason:
  MiKTeX could not find the script engine 'perl' which is required to execute 'latexmk'.

Remedy:
  Make sure 'perl' is installed on your system.

The log file hopefully contains the information to get MiKTeX going again:
  C:\Users\\AppData\Local\MiKTeX\miktex\log\latexmk.log

For more information, visit: [https://miktex.org/kb/fix-script-engine-not-found](https://miktex.org/kb/fix-script-engine-not-found)

```

### 🔧 Solución

Este fallo ocurre porque `latexmk` requiere el motor de **Perl**, el cual no viene preinstalado por defecto en Windows. Para solucionarlo:

1. Abre **PowerShell** o **Símbolo del sistema (CMD)** como Administrador.
2. Ejecuta el siguiente comando para instalar Strawberry Perl:
```powershell
winget install StrawberryPerl.StrawberryPerl

```


3. Una vez terminada la instalación, **reinicia Visual Studio Code** para que detecte las nuevas variables de entorno (`PATH`).
4. Vuelve a compilar tu archivo `.tex` (`Ctrl + Alt + B`).

---

## 💬 Soporte

Si experimentas cualquier otro problema de compilación, conflicto con paquetes o dudas con Git, no dudes en contactarme.

```

```

