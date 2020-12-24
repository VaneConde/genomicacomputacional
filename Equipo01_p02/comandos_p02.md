
# Comandos de la Práctica 02
## Equipo 01 
### Integrante 1: Astrid Austria López
### Integrante 2: Xochitl Vanessa Conde Alonzo 
...

# Parte I. 

**Respuesta 1**

Tabla

| Plataforma/ compañía     | Longitud de reads (pb) | # reads x run   | Tiempo      | Costo x 10^6 bases | Error (%) | Química                 |                                                 |
|--------------------------|------------------------|-----------------|-------------|--------------------|-----------|-------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------
|primera generación        |                        |                 |             |                    |           |                         | 
| Sanger/life technologies | 800                    | 1               | 2 hrs       | $2400              | 0.3       | Dideoxy terminator      |                                   
|Segunda Generación        |                        |                 |             |                    |           |                         |                                 
| Illumina/ HiSeq          | 50 - 250               | 5x10^9          | 27-240 hrs  | ~$0.10             | 0.8       |Revesible terminators    |
| Roche/ 454               | 700                    | 1000000         | 1 - 2 día   | $10                | 1         |Pyrosequencing           |
|Tercera generación        |                        |                 |             |                    |           |                         |
| PACBio/ SMRT             | 2900                   |1x10^6           |<2 hrs       | $2                 | 12.9      |Real-time SMS            | 
| Nanopore/ Oxford         | >5000                  | 6x10^4          | 3 días      | <1                 | 34        |Real-time SMS            |
|Heliscopio/ Helicos       | 35                     | 7x10^9          |8 días       | $0,01              | 0.2       |Real-timw SMS            |

# Parte II

**Respuesta 1**

 para descomprimir:

 unzip ena_files1.zip
 
 gunzip ERR486827_1.fastq.gz

 gunzip ERR486827_2.fastq.gz

Para pasar de fastq a fasta:

 awk '{if (NR% 4 == 1) {printf (">% s \ n", substr ($ 0,2));} else if (NR% 4 == 2) print;}' ERR486827_1.fastq > secuencia1.fa

 awk '{if (NR% 4 == 1) {printf (">% s \ n", substr ($ 0,2));} else if (NR% 4 == 2) print;}' ERR486827_2.fastq > secuancia2.fa

**Respuesta 2** 

 ¿ambos archivos tienen la misma cantidad de secuencias? Sí
  
  grep -c "^>" secuencia1.fa
  
  398824

 grep -c "^>" secuancia2.fa

   398824

# Parte III

**Respuesta 1** 

para descomprimir:

 unzip FastQC-0.11.9.zip

para dar permisos de ejecución:

chmod +x fastqc 

#/Users/uliaus/Desktop/FastQC-0.11.9

 para el enlace simbólico: sudo ln -s /Users/uliaus/Desktop/FastQC-0.11.9/fastqc /usr/local/bin/fastqc

Para hacerlo ejecutable:
 
export PATH=$PATH:/Users/uliaus/desktop/FastQC

Creación de scritp*

**Respuesta 3**

Archivo html

file:///Users/uliaus/pruebanueva/ERR486827_1_fastqc.html
file:///Users/uliaus/pruebanueva/ERR486827_2_fastqc.html

#Descripcion de lecturas 


# Parte IV

**Respueta 1**

Secuencias crudas de Saccharomyces Saccharomyces species, S cerevisiae y S paradoxus. 

Secuencias expraidas de : https://www.ebi.ac.uk/ena/browser/view/PRJNA33187

**Respuesta 2**

Se utilizó el método Sanger para la secuenciación del genoma

https://www.sanger.ac.uk/research/projects/genomeinformatics/sgrp.html

**Respuesta 3**

**Respuesta 4**

cobertura= (398824*150*)/580000 = 103.1441

