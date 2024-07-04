# COMMAND EXECUTION

Si un atacante puede ejecutar código arbitrario en los sevidores, tus sistemas obviamente estas o van a ser comprometidos. Necesitamos tener una gran preocupación de como el servidor web interactua con el Sistema Operativo.

## PELIGROS

La injección de comandos es donde más seguridad necesitamos enfocar, es el ultimo paso para tener el control del sistema. Después de ganar acceso, el atacante puede intentar escalar privilegios en el servidor, instalar scripts maliciosos, o hacer una "botnet" al servidor.

## PROTECCIÓN

Si tu aplicacion coge servicios del mismo sistema operativo, tu necesitas estar seguro de los comandos y la seguridad en la aplicación, si no alguien que tiene intenciones maliciosas puede hacer instrucciones. Esta sección haremos formas para protegernos.

Intentemos que todos los comandos llamen a lo que tiene que llamar

Los programas de lenguaje modernos tienen interfaces para leer archivos, mandar emails y hacer servicios de operacion o funciones. Usar APIs siempre que sea posible, solo usar comandos de shell cuando sea absolutamente necesario. Esto reduce el numero de ataques y vectores para la aplicación y simplificar siempre el codigo base.

### INPUTS CORRECTAMENTE

Las vulnerabilidades por injección ocurren porque no hay una sanitación correcta. Si tu usas comandos de termina, estate seguro que los inputs que vayas a meter no sean potenciales caracteres maliciosos.

![image](https://github.com/pons-rgb/vuln/assets/174595469/1e7b28d0-4d52-418e-86eb-386338069d12)

Siempre es mejor, restringir los input y las expresiones regulares para mayor seguridad.

### RESTRINGUIR LOS COMANDOS PERMITIDOS

