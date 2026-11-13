\# Instalación y Configuración Inicial



Git es multiplataforma y puede instalarse en Windows, Linux y macOS. A continuación se detalla el proceso de instalación y configuración en entornos Windows.



\## Requisitos del sistema



| Componente | Requisito Mínimo | Recomendado | Estado |

| :--- | :---: | :---: | :---: |

| \*\*Sistema Operativo\*\* | Windows 10 / Linux / macOS | Windows 11 o Ubuntu 24.04 | :material-check-circle: |

| \*\*Espacio en disco\*\* | 150 MB libres | 500 MB libres | :material-check-circle: |

| \*\*Terminal\*\* | CMD / PowerShell | Windows Terminal / Git Bash | :material-check-circle: |

| \*\*Cuenta remota\*\* | No obligatoria en local | Cuenta en GitHub | :material-check-circle: |



\## Instalación desde la terminal (Windows)



Puedes instalar Git de forma rápida utilizando el gestor de paquetes oficial `winget` en PowerShell:



```powershell

winget install --id Git.Git -e --source winget

