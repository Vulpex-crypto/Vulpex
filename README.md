# Vulpex
una criptomoneda hecha para la comunidad de libre uso. 

Algoritmo: Scrypt
Tipo de bloque: Prueba de trabajo
Nombre de moneda: Vulpex
Abreviatura de moneda: VUX
Carta de dirección: V
Puerto RPC: 14747
Puerto P2P: 14748
Recompensa de bloque: 50 monedas
Bloque having: 210000 bloques
Suministro de monedas: 21000000 monedas
Bloques de vencimiento de Coinbase: 20 (+ 1 confirmación predeterminada)
Espaciado objetivo: 5 minutos
Tiempo objetivo: 10 minutos
Confirmaciones de transacciones: 6 bloques


Último bloque con recompensa 6930000
Tiempo hasta el último bloque 65 años, 10 meses, 17 días, 12 horas.

Use las siguientes instrucciones para extraer un bloque. Abra su billetera y asegúrese de que su billetera esté conectada con un nodo y que se sincronice.

para extraer bloques

Cierre su billetera y cree el archivo vulpex.conf en la carpeta "% APPDATA% \ vulpex \". Pegue el siguiente texto en vulpex.conf y guarde el archivo.

rpcuser=rpc_vulpex
rpcpassword=ce61ae811b0a8dfb643b89477
rpcallowip=127.0.0.1
rpcport=14747
listen=1
server=1

Abre tu billetera.

Extraer bloques en Windows

Cree un archivo .bat llamado mine.bat en la misma carpeta donde extrajo vulpex-cli.exe y pegue el siguiente texto en mine.bat.

@echo off
set SCRIPT_PATH=%cd%
cd %SCRIPT_PATH%
echo Press [CTRL+C] to stop mining.
:begin
 vulpex-cli.exe generate 1
goto begin 

Guarda el archivo y ejecutelo.

Extraer bloques en linux 

Cree un archivo .sh llamado mine.sh en la misma carpeta donde extrajo vulpex-cli.exe y pegue el siguiente texto en mine.sh

#!/bin/bash
c=1
while c=0
do
./vulpex-cli generate 1
done

Guarda el archivo y ejecutelo. 
