# MP01-Documentacio



## 1. Instalació FOG

Primer fem una instal·lació d'un ubuntu server. Aquest no te interfície gràfica però no la necessitem.
Amb aquesta comanda descarreguem el servidor FOG:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/8dfd1323-52ab-4465-ae4a-a53b86998426)

Comprovo que el tinc:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/55d2004e-6fbf-44d0-a464-081f4cff3b5f)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/0790d990-65ab-4a92-a7be-d6fab51c5b9b)

i ara l'instal·lo:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/0f1aece4-a3a0-4c97-bc06-f62a7e496791)

i li dono la configuració necessaria:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/6032f9e7-95c3-43e9-b4f9-59da0049c4f0)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/d6685d63-2cd1-4539-b99c-f5a951000a54)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/7897acf6-2632-4ebf-8d97-d78982dc69b0)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/2a4c15e0-5b7a-4b9d-a2f7-e16a00d99bc1)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/5d01e1e3-f32e-4d17-9054-17bdd1769140)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/d47802d1-a199-4ea3-80f6-f525146ed13f)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/f4b59bd2-287c-46c5-86ae-91e8528d22a7)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/533dc4c2-37e2-4661-9a5b-483a54010694)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/4490fb56-5fb2-4afb-a9b5-0007833043cc)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/016de7fb-38e0-4a22-afbd-0e750d85b263)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/64de4711-905e-4cf9-8041-73f3f59b391e)

Ara s'acavarà d'instal·lar i ja el tindrem preparat per a treballar-hi.

## 2. Capturar desde el client un Windows

Al FOG management, anem a Images i clickem a Create New Image, aquí només detallem la informació retllevant de la imatge:

![Selecció_074](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/fc9418f8-a5f3-408a-b788-638a643f704e)

Després tanquem client i comencem a instal·lar la màquina Windows que capturarem:

![Selecció_096_install windows](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/1162b2a6-1178-4937-b0a9-bb1492a371ac)

Quan arribem a la sel·lecció de regió apretem Ctrl + Shift + F3 per entrar en Audit Mode (OOBE):

![Selecció_096](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/4826daa9-dc9f-4b0a-bd37-280de6092024)

Windows s’inicia, tanquem finestra de SysPrep:

![Selecció_097](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/e1e722d4-5c41-4c16-a952-14b0d1def305)

Descarreguem ADK:

![Selecció_098](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/6432b411-5740-4a8a-b8f1-0cc7d20efda0)

Instal·lem Deployment Tools:

![Selecció_099](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/424db2eb-8bda-4a32-b119-d33e763f3d8a)

Com es pot observar hem instal·lat Chrome i hem canviat el fons de pantalla a la màquina a capturar:

![Selecció_100](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/5072b9ab-39ae-430c-94f5-ed462df508fa)

Descarreguem FOG Client desde el dashboard de fog (http:/ip/fog/management):

![Selecció_101](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/ed84d79d-ec5d-42e7-85d8-5e35a2a87df1)

Sel·leccionem SmartInstaller:

![Selecció_102](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/f96001a9-41f7-4491-8978-e977a4544d7c)

Instal·lem i fiquem la IP del server:

![Selecció_103](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/b4a9edcf-a633-431f-8198-a7eaece70b5e)

Fiquem ISO de Windows i copiem els fitxers a una carpeta creada a C:, en aquest cas li direm customize/Win10:

![Selecció_104](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/799ed79e-a3bd-41b8-bb39-f3043e418038)


![Selecció_137](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/4174b62a-19bf-4b04-9383-1b51c147de10)

Convertim fitxer install.esd a install.wim amb Powershell:

![Selecció_105](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/4bd974ef-d079-4b6a-a2ad-004f084e4d56)

![Selecció_106](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/dc06c5be-944a-49e4-ba59-512c6e5fa2c4)

Creem un altra carpeta anomenada Distribution amb els següents directoris:

![Selecció_108](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/fac45a32-3d82-4ee9-ba96-8829ef2b8dc4)

Obrim SysPrep i obrim imatge de Windows, després generem fitxer de resposta:

![Selecció_110](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/58b2fadf-e51a-41b9-b228-e0ad932ae9d1)

Validem fitxer de resposta:

![Selecció_111](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/8f8f29f3-ace1-451c-b067-62128cfe6c8e)

El guardem i iniciem Sysprep a una terminal per crear la imatge Generalitzada de Windows 10:

![Selecció_112](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/8a10740a-c0cd-4d77-8908-fec18d1e2be4)

![Selecció_113](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/cfd6078a-6f54-477a-aa75-417de4eacc99)

Anem al Fog dashboard i creem una nova imatge que li direm Win10GeneralImage:

![Selecció_114](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/d1a2694f-1145-4441-b2d6-c0a0509aaa37)

Canviem ordre d’arrencada de la màquina amb Windows 10 per iniciar per xarxa:

![Selecció_115](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/b6b9dc87-c234-4f0a-85d3-c1eca6eb27bf)

Sel·leccionem la següent opció:

![Selecció_116](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/19682a80-c78c-492d-8941-af7ec03d41ef)

Una vegada hem fet el registre tornem al FOG Dashboard, a Hosts per veure si s’ha guardat el registre:

![Selecció_117](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/b0849155-cef7-4068-a1ea-3c60f964d553)

Clickem a sobre i especifiquem la imatge que volem (la que hem creat previament: WIn10GeneralImage):

![Selecció_118](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/2be852a9-65eb-4873-bbbb-0c56e7605eec)

Task management i li donem a  l’icona de capturar:

![Selecció_119](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/6320eb98-195f-44b8-b343-6c95797a4e8f)

Iniciem la màquina de Windows 10 per xarxa i comença la captura:

![Selecció_121](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/77efdcc5-5f55-433e-8f44-d2e4ac78b260)

Ja la tenim capturada:

![Selecció_122](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/f9c16370-1805-4487-9d35-760e43e4d431)

Font: https://www.ceos3c.com/sysadmin/create-generalized-windows-10-image-deploy-fog-server/

## 3. Capturar desde el client un Ubuntu


Primer crearem la màquina de la qual farem la imatge. Hem de tenir en compte que totes les instal·lacions d'aquesta imatge estaran basades en aquesta màquina així que l'hem de configurar i equipar amb apps tenint això en compte.
En el nostre cas també afegirem alguna cosa extra per a que a les captures de pantalla es vegi que la instal·lació per FOG és genuïna

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/b864ec90-bae5-40db-8413-4c13efd70c26)

Un cop fet això tanquem la màquina i la tornem a engegar posant a l'ordre d'engegada la Xarxa en primer lloc per a connectar-nos al servidor FOG

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/8a0b8a66-030c-4c85-9cb7-15a63e6f289a)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/98d0b044-c664-4e30-9f6d-b5af5ec38e73)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/8566f654-afd5-4af3-92d5-e3e99338425b)

I posem la ip del servidor.

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/de4014c8-454c-4a85-bb99-f3d40c058c41)

Ara seleccionem la opció de "Perform Full Host Registration and Inventory" per a que la imatge quedi capturada al servidor FOG.

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/fbddefe8-c1e7-4a8a-a7d3-c5edbe03ad17)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/bd38c1f0-7b35-480c-82b6-cf49c46efee6)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/942a6118-a199-491c-a312-d20b506004f0)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/97736c80-0e9a-4611-987d-2b185c242541)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/33c698e4-f5c4-4deb-b946-e3f2293a7948)

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/764c1d0c-a54a-4884-8954-a7d30ba5a5fc)
![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/36f8e1a8-c18a-4fbf-b28e-57384d21d33e)
![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/e2fd5e1d-748c-466d-9c7a-ae79e0f40bf3)


Ara hauria d'estar preparada per a instal·lar a altres màquines.

# 4. Instal·lar imatge Ubuntu

Un cop capturada la imatge només hem de crear una nova màquina virtual d'ubuntu. En aquest cas no posarem cap imatge amb la que instal·lar el SO ja que aquest vindra del servidor FOG. Per tant a paràmetres tornem a posar la Xarxa al principi del "boot":

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/ab6dfdb2-2b23-4a62-8b50-aadce44c097e)


Llavors fem el "login" al servidor:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/6e0d0936-dac5-4e1d-812c-5a9b1ae33561)

Triem la opció de "Deploy" al menú i elegim la imatge que necessitem:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/64ebf59f-2d14-4e8b-9063-66ebabb2efb7)

I la instal·lació començarà:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/c18eb68e-e1b6-4017-b5c0-c6a8a5e2bfc7)

Un cop acabada tornem als paràmetres de la màquina, desactivem Xarxa del "boot sequence" i la tornem a engegar per a comprovar que la instal·lació ha estat un èxit:

![image](https://github.com/NorbertFalco/MP01-Documentacio/assets/114875463/b3baeb99-5ddc-4257-90b0-4150c64fe17a)

## 5. Instalar imatge Windows

Creem una màquina de 0 sense ISO, fiquem xarxa NAT igual que el servidor Fog:

![Selecció_130](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/7cdd3548-4d74-47ba-b0ef-f120736061af)

![Selecció_131](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/cfee3a29-2e07-4d5f-815b-cc234975b400)

Entrem al FOG i fiquem Deploy Image:

![Selecció_133](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/2a7ce316-17ee-469d-920e-337b6e840e4f)

Sel·leccionem la imatge de Windows:

![Selecció_132](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/36648fdf-449a-468e-b3e5-496897967084)

Comença a planxar-se:

![Selecció_134](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/1f4e7cd1-7dd1-43b3-aa60-a81c15a44b5d)

No s’ha guardat el fons de pantalla, però Chrome està instal·lat:

![Selecció_136](https://github.com/EricQC94/MP01-Documentacio/assets/113598440/3a34bda7-9749-4502-81d3-8491a6c09299)






