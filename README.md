# lab5-osec2-2023

## Requisitos

- Debe contar con un ambientes de acuerdo al LAB#5
- Este script debe ejecutarse en algun servidor de IPA (debe instalar git)  
- Debe estar autenticado a Kerberos ```kinit admin```
- Ha sido validado en RHEL 9.2

## USO:

### Listar todos las cuentas de los grupo solicitados o especificar el nombre del grupo 

```sh
./lab5.sh accounts all|group_name
```
### Obterner información de los otros puntos del Laboratorio 

```sh
./lab5.sh lab
```

### Obterner información de las replicas


```sh
./lab5.sh lab
```


Instrucciones de Entrega:

Ejecutar:

```
CARNET=111111
date > MD5.txt
./lab5.sh replica > ${CARNET}-lab5-sec1.txt &&  md5sum ${CARNET}-lab5-sec1.txt >> MD5.txt
./lab5.sh accounts all > ${CARNET}-lab5-sec2.txt && md5sum ${CARNET}-lab5-sec2.txt >> MD5.txt
./lab5.sh lab > ${CARNET}-lab5-sec3.txt && md5sum ${CARNET}-lab5-sec3.txt >> MD5.txt

tar -cvzf ${CARNET}-lab5.tgz MD5.txt ${CARNET}*
md5sum ${CARNET}-lab5.tgz
```
Subir al GES CARNET-lab5.tgz

