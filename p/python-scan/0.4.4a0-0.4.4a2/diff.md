# Comparing `tmp/python_scan-0.4.4a0-py3-none-any.whl.zip` & `tmp/python_scan-0.4.4a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 11418 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    36517 b- defN 23-May-03 18:03 python_scan-0.4.4a0.data/scripts/PORT_SCAN.py
--rw-rw-rw-  2.0 fat     2777 b- defN 23-May-03 18:27 python_scan-0.4.4a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 18:27 python_scan-0.4.4a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-03 18:27 python_scan-0.4.4a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      424 b- defN 23-May-03 18:27 python_scan-0.4.4a0.dist-info/RECORD
-5 files, 39811 bytes uncompressed, 10622 bytes compressed:  73.3%
+Zip file size: 12959 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    42776 b- defN 23-May-05 20:03 python_scan-0.4.4a2.data/scripts/PORT_SCAN.py
+-rw-rw-rw-  2.0 fat     2777 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      424 b- defN 23-May-06 09:06 python_scan-0.4.4a2.dist-info/RECORD
+5 files, 46070 bytes uncompressed, 12163 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: python_scan-0.4.4a0.data/scripts/PORT_SCAN.py
+Filename: python_scan-0.4.4a2.data/scripts/PORT_SCAN.py
 Comment: 
 
-Filename: python_scan-0.4.4a0.dist-info/METADATA
+Filename: python_scan-0.4.4a2.dist-info/METADATA
 Comment: 
 
-Filename: python_scan-0.4.4a0.dist-info/WHEEL
+Filename: python_scan-0.4.4a2.dist-info/WHEEL
 Comment: 
 
-Filename: python_scan-0.4.4a0.dist-info/top_level.txt
+Filename: python_scan-0.4.4a2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_scan-0.4.4a0.dist-info/RECORD
+Filename: python_scan-0.4.4a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_scan-0.4.4a0.data/scripts/PORT_SCAN.py` & `python_scan-0.4.4a2.data/scripts/PORT_SCAN.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 try:
     print("\n[♦] Identificando requisitos para la ejecución del programa...\n")
+    from host_discover import discove
     import subprocess
     import concurrent.futures
     import time
     import ctypes
     import string
     from datetime import datetime
     import re
@@ -24,20 +25,20 @@
           Fore.YELLOW + " Modulos importados correctamente, procediendo con la ejecución del programa")
     time.sleep(1)
     modules = True
 
 except Exception as e:
     # If there are any errors encountered during the importing of the modules,
     # then we display the error message on the console screen
-    print('Existen modulos necesarios que no tiene instalado... \n\n')
-    time.sleep(2)
+    print('Existen modulos necesarios que no tiene instalado... \n\n', e)
     exit()
 
-# Añadir más colores y intentar perfeccionar nmap args
+# Subir a pypi
 # añadir más opciones, como escaneo de webs (http-enum) / sqlinjection / brute force / etc...
+# Añadir Logs en el arhchivo (ip/puertos/vulns/etc...)
 
 if modules:
     nm = nmap.PortScanner()
     open_ports = []
 
 
 def verifi_tools():
@@ -83,15 +84,15 @@
             exit()
 
 
 def print_help():
     print(Fore.YELLOW + """
         ╔════════════════════════════════════════════════╗
         ║                                                ║
-        ║   --  Usabilidad 'PORT SCANNER' v0.4.4.a1 --   ║        
+        ║   --  Usabilidad 'PORT SCANNER' v0.4.4.a2 --   ║        
         ║                                                ║
         ╚════════════════════════════════════════════════╝""" +
 
           Fore.GREEN + "\n\nArgumentos de la herramienta:\n\n" +
           Fore.BLUE + "[♦]" + Fore.YELLOW + " Enter IP --> IP OBETIVO\n" +
     Fore.CYAN + """
             ║       
@@ -136,21 +137,23 @@
         else:
             try:
                 ports = int(ports)
                 if ports > 65535:
                     input('Has superado el número máximo de puertos.\n'
                           'Se reducirá a "65535" (numero máx. de puertos) -- [ENTER]')
                     ports = 65535
+                    write_file('[!] PORTS TO SCAN ---> 1-' + str(ports))
+                else:
+                    write_file('[!] PORTS TO SCAN ---> 1-' + str(ports))
                 break
             except ValueError:
                 print(Fore.RED + "Arguemnto inválido.\nPara obtener ayuda escriba --> '--help'")
 
 
 
-
 def port_scan_banner():
     print(Fore.GREEN + """\n
     
                                                                                 © 
  ██▓███   ▒█████   ██▀███  ▄▄▄█████▓     ██████  ▄████▄   ▄▄▄       ███▄    █ 
 ▓██░  ██▒▒██▒  ██▒▓██ ▒ ██▒▓  ██▒ ▓▒   ▒██    ▒ ▒██▀ ▀█  ▒████▄     ██ ▀█   █ 
 ▓██░ ██▓▒▒██░  ██▒▓██ ░▄█ ▒▒ ▓██░ ▒░   ░ ▓██▄   ▒▓█    ▄ ▒██  ▀█▄  ▓██  ▀█ ██▒
@@ -160,95 +163,215 @@
 ░▒ ░       ░ ▒ ▒░   ░▒ ░ ▒░    ░       ░ ░▒  ░ ░  ░  ▒     ▒   ▒▒ ░░ ░░   ░ ▒░
 ░░       ░ ░ ░ ▒    ░░   ░   ░         ░  ░  ░  ░          ░   ▒      ░   ░ ░ 
              ░ ░     ░                       ░  ░ ░            ░  ░         ░ 
                                                 ░                                                                                                 
                                                 
        [INFO] Herramienta para analizar puertos de una dirección IP 
              ║                                                 ║                                                                                             
-             ║                    v0.4.4.a1                    ║
+             ║                    v0.4.4.a2                    ║
              ╚══════► Escriba --help para obtener ayuda ◄══════╝
                     \n\n""")
 
 
+def host_disc_bann():
+    print(Fore.RED + '''\n
+                               .    .        s              ....             .       .                                 _                                 
+  .uef^"                  z`    ^%      :8          .xH888888Hx.        @88>          ^%                          u                                  
+:d88E              u.        .   <k    .88        .H8888888888888:      %8P        .   <k                  u.    88Nu.   u.                .u    .   
+`888E        ...ue888b     .@8Ned8"   :888ooo     888*"""?""*88888X      .       .@8Ned8"       .    ...ue888b  '88888.o888c      .u     .d88B :@8c  
+ 888E .z8k   888R Y888r  .@^%8888"  -*8888888    'f     d8x.   ^%88k   .@88u   .@^%8888"   .udR88N   888R Y888r  ^8888  8888   ud8888.  ="8888f8888r 
+ 888E~?888L  888R I888> x88:  `)8b.   8888       '>    <88888X   '?8  ''888E` x88:  `)8b. <888'888k  888R I888>   8888  8888 :888'8888.   4888>'88"  
+ 888E  888E  888R I888> 8888N=*8888   8888        `:..:`888888>    8>   888E  8888N=*8888 9888 'Y"   888R I888>   8888  8888 d888 '88%"   4888> '    
+ 888E  888E  888R I888>  %8"    R88   8888               `"*88     X    888E   %8"    R88 9888       888R I888>   8888  8888 8888.+"      4888>      
+ 888E  888E u8888cJ888    @8Wou 9%   .8888Lu=       .xHHhx.."      !    888E    @8Wou 9%  9888      u8888cJ888   .8888b.888P 8888L       .d888L .+   
+ 888E  888E  "*888*P"   .888888P`    ^%888*        X88888888hx. ..!     888&  .888888P`   ?8888u../  "*888*P"     ^Y8888*""  '8888c. .+  ^"8888*"    
+m888N= 888>    'Y"      `   ^"F        'Y"        !   "*888888888"      R888" `   ^"F      "8888P'     'Y"          `Y"       "88888%       "Y"      
+ `Y"   888                                               ^"***"`         ""                  "P'                                "YP'                 
+      J88"                                                                                                                                           
+      @%                                                                                                                                             
+    :" 
+                                [INFO] Herramienta para analizar puertos de una dirección IP                                                                                             
+                                     ║                    v0.4.4.a2                    ║
+                                     ╚══════► Escriba --help para obtener ayuda ◄══════╝
+    
+    \n''')
+
+
 def service_scan_bann():
     print(Fore.GREEN + """\n
 
 .▄▄ · ▄▄▄ .▄▄▄   ▌ ▐·▪   ▄▄· ▄▄▄ .    .▄▄ ·  ▄▄·  ▄▄▄·  ▐ ▄ 
 ▐█ ▀. ▀▄.▀·▀▄ █·▪█·█▌██ ▐█ ▌▪▀▄.▀·    ▐█ ▀. ▐█ ▌▪▐█ ▀█ •█▌▐█
 ▄▀▀▀█▄▐▀▀▪▄▐▀▀▄ ▐█▐█•▐█·██ ▄▄▐▀▀▪▄    ▄▀▀▀█▄██ ▄▄▄█▀▀█ ▐█▐▐▌
 ▐█▄▪▐█▐█▄▄▌▐█•█▌ ███ ▐█▌▐███▌▐█▄▄▌    ▐█▄▪▐█▐███▌▐█ ▪▐▌██▐█▌
  ▀▀▀▀  ▀▀▀ .▀  ▀. ▀  ▀▀▀·▀▀▀  ▀▀▀      ▀▀▀▀ ·▀▀▀  ▀  ▀ ▀▀ █▪                                                                                            
 \n""")
 
+
+def help_discover():
+    print(Fore.YELLOW + """
+            ╔════════════════════════════════════════════════╗
+            ║   --  Usabilidad 'HOST DISCOVER' v0.4.4.a2 --  ║        
+            ╚════════════════════════════════════════════════╝\n\n""" +
+
+          Fore.BLUE + "[♦]" + Fore.YELLOW + " Enter IP --> IP OBETIVO\n" +
+          Fore.CYAN + """
+                ║       
+                ╚════ EJEMPLO --> [♦] ENTER IP -> 192.168.1.0/24\n""" +
+
+          Fore.CYAN + """ 
+                ║       
+                ╚═► """ + Fore.BLUE + "[♦] " + Fore.YELLOW + "REQUERIMIENTO --> " + Fore.YELLOW + 'Mascara en formato CIDR\n\n')
+
+
+def graph_host():
+    print(Fore.BLUE + "\t[!] " + Fore.GREEN + '↓ EJEMPLOS ↓ \n')
+    print(Fore.LIGHTRED_EX + "\t\t║")
+    print("\t\t║══════► 192.168.1.0/24")
+    print("\t\t║")
+    print("\t\t╚══════► --help")
+    print(Fore.BLUE + '\n\n\t[♦] ' + Fore.YELLOW + 'Enter IP Range')
+
+
+def init_host():
+    now = datetime.now()
+    print(Fore.RED + "[!] " + Fore.YELLOW + "Escaneo de subred iniciado...\n")
+    print(Fore.RED + "[T] " + Fore.YELLOW + "", now, "\n")
+
+
+def host_discover():
+    clean()
+    host_disc_bann()
+    target = None
+    err = False
+    while not target:
+        clean()
+        host_disc_bann()
+
+        if err:
+            graph_host()
+            print(Fore.RED + "[!] Has introducido una máscara inválida...")
+
+            print("\t\t║")
+            target = input("\t\t╚═► " + Fore.RESET)
+
+        else:
+            # Printear ayuda la 1ª vez que se ejecute
+            graph_host()
+            print("\t\t║")
+            target = input("\t\t╚═► " + Fore.RESET)
+
+        # Printear ayuda
+        if 'help' in target:
+            clean()
+            host_disc_bann()
+            help_discover()
+            graph_host()
+
+            print("\t\t║")
+            target = input("\t\t╚═► " + Fore.RESET)
+
+        # Comprobar si está bien escrita la IP
+        else:
+            mask = re.findall("/([0-9]+)$", target)
+            mask = "".join(mask)
+
+            try:
+                mask = int(mask)
+
+                # Verificar que la mascara dentro de la lista no supere los 32 y sea int
+                if mask > 32:
+                    err = True
+                    target = None
+
+            # Verificar que sea un número
+            except ValueError:
+                err = True
+                target = None
+
+
+    clean()
+    host_disc_bann()
+    init_host()
+    discove(target)
+
+
 def init(now, target):
     # Inicio del analisis, tiempo y objetivo
     print(Fore.YELLOW + "-" * 55)
-    print(Fore.GREEN + "[X] " + Fore.YELLOW + "Objetivo -->" + Fore.RED + f" {target}" +
+    print(Fore.GREEN + "[♦] " + Fore.YELLOW + "Objetivo -->" + Fore.RED + f" {target}" +
           Fore.YELLOW + " <--> Nº ports" + Fore.RED + " {}".format(ports))
-    print(Fore.GREEN + "[X] " + Fore.YELLOW + "Analisis iniciado --> {}".format(now))
+    print(Fore.GREEN + "[♦] " + Fore.YELLOW + "Analisis iniciado --> {}".format(now))
     print("-" * 55)
 
 
+
 def graph(target):
     # Escaneo de puertos gráfico
     clean()
     port_scan_banner()
     num_ports()
     clean()
     port_scan_banner()
     # Banner
     scan(target)
 
 
-def funcions(target):
+def funcions():
+    clean()
     port_scan_banner()
     # Añadir funciones preguntando antes de los puertos.
     print(Fore.BLUE + "[♦]" + Fore.YELLOW + " Que herramienta quieres utilizar?")
     print(Fore.YELLOW + "-" * 50)
     print(Fore.BLUE + 'A:' + Fore.YELLOW + ' --> Port and vuln scan' + '\n \n'
-          + Fore.BLUE + 'B:' + Fore.YELLOW + ' --> Metasploit.\n')
+          + Fore.BLUE + 'B:' + Fore.YELLOW + ' --> Metasploit.\n\n'
+          + Fore.BLUE + 'C: ' + Fore.YELLOW + '--> Host Discovery\n')
     fun = None
     while not fun:
         fun = input(Fore.YELLOW + "         ╚═► ")
         if 'help' in fun:
             clean()
             port_scan_banner()
             print_help()
 
             print(Fore.YELLOW + "\nQue herramienta quieres utilizar?")
             print("-" * 50)
-            print('A: --> Port and vuln scan\n \nB: --> Metasploit.\n \nC: --> Fuzzing')
+            print(Fore.BLUE + 'A:' + Fore.YELLOW + ' --> Port and vuln scan' + '\n \n'
+                  + Fore.BLUE + 'B:' + Fore.YELLOW + ' --> Metasploit.\n')
             fun = None
-        elif fun in ['a', 'A']:
-            graph(target)
+        elif fun.lower() in ['a']:
+            enter_arguments()
             break
 
-        elif fun in ['b', 'B']:
+        elif fun.lower() in ['b']:
             input(Fore.YELLOW + "Esta funcion requiere que tengas instalado Metasploit [-ENTER-].")
             try:
                 os.system('msfconsole')
                 break
             except Exception as error:
                 print(Fore.RED + "ERROR: {}\nPrueba a reinstalar o instalar metasploit.".format(error))
+        elif fun.lower() in ['c']:
+            host_discover()
+
         else:
             print(Fore.RED + "Introduce una opción válida, has escogido '{}',"
                              " que no está entre las opciones disponibles".format(fun))
             fun = None
 
 
 def ping(ip_address):
     global alive
     while True:
         clean()
         port_scan_banner()
         # Confirmación con PING?
 
-        p = input(Fore.YELLOW + '\!] ¿Quieres hacer una confirmación con PING?\n\n' + Fore.GREEN
-                               + '\t[I] El host puede tener un FireWall bien configurado que bloquee este tipo de paquetes.\n'
-                                '\t     Si sabes que esta activo no ejecutes la confirmación.' + Fore.BLUE + ' [S/n] -->')
+        p = input(Fore.YELLOW + '[!] ¿Quieres hacer una confirmación con PING?\n\n' + Fore.GREEN
+                    + '\t[I] El host puede tener un FireWall bien configurado que bloquee este tipo de paquetes.\n'
+                    '\t     Si sabes que esta activo no ejecutes la confirmación.' + Fore.LIGHTRED_EX + '\n\t\t\t[S/n] -->')
 
         # En línea o no
         if p in ['S', 's']:
 
             """
             Pings the given IP address to check if it's active or not.
             """
@@ -300,15 +423,14 @@
                 time.sleep(0.08)
                 futures.append(executor.submit(scaning, port))
             # Excepciones del código
             except KeyboardInterrupt:
                 end = datetime.now()
                 elapsed = end - now
                 print(Fore.YELLOW + '\n\nAnálisis interrumpido en el puerto {}.'.format(port))
-                print(Fore.YELLOW + 'Final del análisis --> {}\n'.format(elapsed))
                 break
             except Exception as err:
                 print("Error inesperado : {}".format(err))
 
 
 def scan(target):
     try:
@@ -327,21 +449,23 @@
                     break
                 else:
                     print("Introduccion inválida...")
 
         # Inicio del analisis.
         clean()
         port_scan_banner()
+
         if alive:
             print(Fore.YELLOW + 'El HOST está en línea.')
         elif alive is None:
             print(Fore.YELLOW + 'No se ha realizado la confirmación con PING')
 
     except socket.gaierror:
         print(Fore.RED + "\nNo se ha encontrado el HOST")
+
     now = datetime.now()
     init(now, target)
 
     init_scan(target, now)
 
     # Final del analisis
     end = datetime.now()
@@ -355,14 +479,19 @@
 
 
 def ports_used(open_ports, target):
     # Creamos lista ordenada de puertos para el scaner
     p_str = [str(a) for a in open_ports]
     p_str = (",".join(p_str))
     print(Fore.GREEN + "\n\nLos puertos abiertos son: {}".format(open_ports))
+
+    text = "[!] OPEN PORTS: {}".format(p_str)
+    write_file(text)
+
+    # Iniciamos check services
     check_serv(target, p_str, open_ports)
 
 
 def serv_search():
     while True:
         serv = input(Fore.BLUE + "\n[♦]" + Fore.YELLOW +
                      r" ¿Quieres ejecutar un analisis completo a los puertos abiertos? [S/n] --> ")
@@ -376,15 +505,15 @@
                 exit()
             else:
                 break
 
 
 def graph_serv(init_scan_service):
     service_scan_bann()
-    print("\n" + "-" * 50)
+    print(Fore.GREEN + "\n\n" + 54 * "═" + "►")
 
     print(Fore.YELLOW + """Escaneando versiones de servicio... 
         ╚══════► Esto puede tardar un poco, vale la pena.\n""")
     print("\nAnálisis iniciado --> {}".format(init_scan_service))
     print("-" * 50 + "\n")
 
 
@@ -428,14 +557,16 @@
         else:
             first = None
             know = None
 
 
 def graph_args():
     print(Fore.BLUE + "\n   [♦] " + Fore.YELLOW + "Introduce los argumentos de nmap que desees")
+    print(Fore.BLUE + "\n   [I] " + Fore.YELLOW + "No introduzcas la IP ni los puertos")
+
 
 def process_args():
     # Printear grafico
     graph_args()
 
     args = None
     # Bucle para introducir argumentos válidos
@@ -453,103 +584,99 @@
         except KeyboardInterrupt:
             return False
         except Exception:
             print(Fore.RED + "[!] Ha ocurrido un error, arguentos de nmap predeterminados")
             return False
 
 
-def check_args(args, default_args):
+def check_args(args, default_args, target, p_str):
     clean()
     service_scan_bann()
 
     if not args:
         return default_args
-    arguments = ["nmap", args]
+    arguments = ["nmap", target, '-p' + p_str, args]
 
     try:
         print(Fore.YELLOW + "\n\t [!] Comprobando Argumentos...")
         subprocess.check_output(arguments, timeout=5)
         print(Fore.BLUE + "\n\t [+] Argumentos comprobados correctamente...")
         return args
 
     except subprocess.TimeoutExpired:
-        print(Fore.RED + "[!] Error... definiendo argumentos predeterminados")
+        print(Fore.RED + "[!] Error... argumentos inválidos")
         time.sleep(2)
         return default_args
     except subprocess.CalledProcessError:
         print(Fore.RED + "[!] Error... definiendo argumentos predeterminados")
         time.sleep(2)
         return default_args
-    except Exception as e:
-        print(e)
+    except Exception as err:
+        print(err)
         time.sleep(2)
         return default_args
 
+
 def check_serv(target, p_str, open_ports):
     # Preguntamos si quiere analisis de versiones de servicio
     serv_search()
 
     # Hora del inicio
     init_scan_service = datetime.now()
 
-    # banner del escaneo de servicios
-    graph_serv(init_scan_service)
-
     # Argumentos de NMAP default
     default_args = "-p {} --script vuln -sS --min-rate 5000 -sC -sV -Pn --version-intensity 3 -n -A -O".format(p_str)
 
     args = know_nmap()
 
     # Comprobar los buenos comandos
-    args = check_args(args, default_args)
+    args = check_args(args, default_args, target, p_str)
 
 
     # Inicio de análisis de nmap
     clean()
-    service_scan_bann()
 
     # Inicio del escaneo
-    print(Fore.GREEN + "\n═══════════════════════════════════════════════════►\n")
-    print(Fore.BLUE + "\n\t[♦] " + Fore.YELLOW + "Escaneo de NMAP iniciado...")
-    print(Fore.BLUE + "\n\t[I] " + Fore.YELLOW + "Argumentos utilizados --> \n\t[{}]".format(args))
-    print(Fore.GREEN + "\n\n═══════════════════════════════════════════════════►")
+    graph_serv(init_scan_service)
+    print(Fore.BLUE + "   [I] " + Fore.YELLOW + "Argumentos utilizados \n\t[{}]".format(args))
+    print(Fore.GREEN + "\n" + 54 * "═" + "►")
 
     nm.scan(target, arguments=args)
     end_service_scan = datetime.now()
     dict_serv = {}
 
     for p in open_ports:
         p = int(p)
 
         print(Fore.YELLOW + "Analisis puerto nº{} \n".format(p))
         # Recolectamos información del escaneo de servicion anterior y procesamos los datos .
         # Introducer N/D a los que no se encuentren.
         try:
             state = nm[target]['tcp'][int(p)]['state']
-        except Exception as e:
+        except Exception:
             state = "N/D"
         try:
             name = nm[target]['tcp'][int(p)]['name']
-        except Exception as e:
+        except Exception:
             name = "N/D"
         try:
             product = nm[target]['tcp'][int(p)]['product']
-        except Exception as e:
+        except Exception:
             product = "N/D"
         try:
             version = nm[target]['tcp'][int(p)]['version']
-        except Exception as e:
+        except Exception:
             version = "N/D"
         try:
             extrainfo = nm[target]['tcp'][int(p)]['extrainfo']
-        except Exception as e:
+        except Exception:
             extrainfo = "N/D"
         try:
             cpe = nm[target]['tcp'][int(p)]['cpe']
-        except Exception as e:
+        except Exception:
             cpe = "N/D"
         try:
             all_host = nm[target]['hostscript']
         except KeyError:
             all_host = None
         # Añadimos al diccionario para la búsqueda de vulners
         if product == "":
@@ -629,25 +756,25 @@
             return ip_vendor
         else:
             return [data for data in ip_vendor]
 
     # Imprimimos la informacion del sistema
     print(Fore.YELLOW + "\nINFORMACIÓN DEL SISTEMA OBJETIVO")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE + "\nSISTEMA " + Fore.YELLOW + "-->" + Fore.GREEN + f" {name_os}")
+    print(Fore.BLUE + "SISTEMA " + Fore.YELLOW + "-->" + Fore.GREEN + f" {name_os}\n")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE +"\nPrecisión " + Fore.YELLOW + "--> " + Fore.GREEN + f"{accuracy}")
+    print(Fore.BLUE + "Precisión " + Fore.YELLOW + "--> " + Fore.GREEN + f"{accuracy}\n")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE + "\nVendedor " + Fore.YELLOW + "--> " + Fore.GREEN + f"{vendor}")
+    print(Fore.BLUE + "Vendedor " + Fore.YELLOW + "--> " + Fore.GREEN + f"{vendor}\n")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE +"\nCPE " + Fore.YELLOW + "--> " + Fore.GREEN + f"{sys_cpe}")
+    print(Fore.BLUE + "CPE " + Fore.YELLOW + "--> " + Fore.GREEN + f"{sys_cpe}\n")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE + "\nIP " + Fore.YELLOW + "--> " + Fore.GREEN + f"{ip}")
+    print(Fore.BLUE + "IP " + Fore.YELLOW + "--> " + Fore.GREEN + f"{ip}\n")
     print(Fore.GREEN + "═" * 50 + "►", "\n")
-    print(Fore.BLUE + "\nMAC & Vendor " + Fore.YELLOW + "--> " + Fore.GREEN + f"{how_print()}")
+    print(Fore.BLUE + "MAC & Vendor " + Fore.YELLOW + "--> " + Fore.GREEN + f"{how_print()}")
 
     elapsed = (end_service_scan - init_scan_service)
     print(Fore.GREEN + "\n" + "-" * 50)
     print(Fore.GREEN + "Tiempo transcurrido duante el analisis -> {}".format(elapsed))
 
     vlnsrch(dict_serv)
 
@@ -854,17 +981,20 @@
                         continue
                     else:
                         print("\nDirección IPv4 inválida.")
                         time.sleep(2)
                         ip = None
                 if ip is not None:
                     try:
+                        write_file('[*] ¡¡Port Scan iniciado!!\n')
+                        write_file("[!] TARGET ---> " + ip)
                         target = socket.gethostbyname(ip)
                         clean()
-                        funcions(target)
+                        graph(target)
+
                     except socket.gaierror:
                         print('Direccion IPv4 inválida')
                         time.sleep(2)
                         ip = None
 
             else:
                 print(Fore.RED + "Dirección IPv4 inválida")
@@ -879,24 +1009,43 @@
                 ║
                 ╠══════► Tipología   --> <name_script>   
                 ║  
                 ╚══════► EJEMPLO 	 --> port_scaner """)
             time.sleep(2.5)
 
 
+def get_user_path():
+    return "{}/".format(Path.home())
+
+
+def write_file(text):
+    userpath = get_user_path()
+    location = userpath + "/Desktop/"
+    filename = "scan.log"
+
+    with open(location + filename, "a", encoding="utf-8") as log:
+        now = str(time.ctime())
+        log.write("\n<<< " +now + " >>> " + text)
+
+
 def main():
     try:
+        text = """
+        PREPARING SCAN PORTS
+════════════════════════════════════\n"""
+        # Creamos archivo y añadimos el inicio
+        write_file(text)
         # Empezamos código limpiando pantalla
         clean()
         # Miramos si eres admin / root
         is_admin()
         # Verificamos NMAP
         verifi_tools()
         # Iniciamos la herramienta
-        enter_arguments()
+        funcions()
 
     # Salida con CTRL + C
     except KeyboardInterrupt:
         print("\n\nSaliendo del programa...")
         exit()
```

## Comparing `python_scan-0.4.4a0.dist-info/METADATA` & `python_scan-0.4.4a2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-scan
-Version: 0.4.4a0
+Version: 0.4.4a2
 Summary: Herramienta para escaneo de puertos/vulners/explits en una IP
 Home-page: https://github.com/TownPablo/PORT_SCANNER
 Author: __TownPablo__
 Author-email: pablodiez024@proton.me
 License: MIT
 Keywords: port scan,seguridad,redes
 Description-Content-Type: text/markdown
```

