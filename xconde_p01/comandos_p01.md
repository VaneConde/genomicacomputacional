#Genómica Computaional 
## Práctica 01 - manejo de datos de secuenciación masiva (Bash)
#Comandos de la practica 01 
## Xochitl Vanessa Conde Alonzo 

# Parte  I
** Respuesta 1**

#/bin/bash 
#~/c/Users/Vanessa/genomicacomputacional/xconde_01/comandos_p01.md

[echo] [$SHELL]

/usr/bin/bash

**Respuesta 2**

#~/c/Users/Vanessa/genomicacomputacional/xconde_01

[mkdir] [data fitered raw_data meta scripts figures archive ]

**Respuesta 3**
#~/c/Users/Vanessa/genomicacomputacional/xconde_01/

[mv] [filtered data]
[mv] [raw_data data]

**Respuesta 4**
 Para que un proyecto este bien organizado, se necesita un 
arreglo en el cual los datos y documentos esten en un mismo sitio 
dependiendo de su clasificación en este caso data contiene datos genéticos, 
este se puede dividir en raw_data, filtered , genotypes etc.: En meta se 
almacenan los metadatos, información de las muestras o cualquier documento 
que sirva para procesar los datos; En Scripts se guardan los scripts 
necesarios para un analisis; Los codigos para realizar figuras se colocaran en figure; en archive se colocan los scripts y resultados que se pueden o no utilizar. 

# Parte II
#~/c/Users/Vanessa/genomicacomputacional/xconde_01/scripts/delay.sh 
[nano] [][delay.dh]
#!/bin/bash 
[echo] "Después de la parte I. necesito un descanso de exactamente 30 segundos" **Respuesta 1** [chmod] [u+x] [delay.sh] **Respuesta 2** [ls][-l] 
[bash][][delay.sh]

**Respuesta 1**

#~/c/Users/Vanessa/genomicacomputacional/xconde_01/scripts

[chmod] [u+x] [delay.sh] 

**Respuesta 2** 

[ls][-l]
[bash][][delay.sh]

 **Respuesta 3**

[nano][][delay.sh]

#~/c/Users/Vanessa/genomicacomputacional/xconde_01/scripts/delay.sh
 
[echo] "despues de la parte I. necesito un descanso de 30 segundos" && 
sleep 30s && [echo] "ya puedo continuar"

#~/c/Users/Vanessa/genomicacomputacional/xconde_01/scripts

[bash] [] [delay.sh]

**Respuesta 4"
#~/c/Users/Vanessa/genomicacomputacional/xconde_01/scripts
[bash] [] [delay.sh &]
[kill] [-a] [PID]

#Parte III

#~/c/Users/Vanessa/genomicacomputacional/xconde_01/meta

**Respuesta 1**

[touch] [] [SarsCov-2.txt ~/genomicacomputacional/xconde_p01/meta] 

**Respuesta 2**

#~/c/Users/Vanessa/downloads

[mv] [] [sequence.fasta sarscov2_genome.fasta]

[mv] [] [sequence.gff3 sarscov2_genome.gff3]

[touch] [] [SarsCov-2_spike.txt]

#~/c/Users/Vanessa/downloads

[mv] [] [sequence.fasta splike_c.faa]

[mv] [] [sequence1.fasta splike_b.faa]

[mv] [] [sequence2.fasta splike_a.faa]

#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/meta

[touch][][SarsCov-2_Spike.txt]

[mv] sarscov2_genome.fasta sarscov2_genome.gff3 splike_c.faa 
splike_b.faa splike_a.faa SRR10971381_R1.fastq.gz 
SRR10971381_R2.fastq.gz sarscov2_assembly.fasta.gz 
[/c/Users/Vanessa/genomicacomputcional/xconde_p01/data/raw_data]

#Parte IV

**Respuesta 1**
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data

[ln] [-s] [/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/filtered splike_c.faa splike_b.faa splike_a.faa]

**Respuesta 2**
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data
[touch] [] [glycoproteins.faa]
 
**Respuesta 3**

 [head] [-3] [splike_c.faa splike_b.faa splike_a.faa] 
>> /c/Users/home/genomicacomptacional/xconde_p01/comandos_p01.md] 

==> splike_a.faa <==
>pdb|7JJJ|A Chain A, Spike glycoprotein
MFVFLVLLPLVSSQCVNLTTRTQLPPAYTNSFTRGVYYPDKVFRSSVLHSTQDLFLPFFSNVTWFHAIHV
SGTNGTKRFDNPVLPFNDGVYFASTEKSNIIRGWIFGTTLDSKTQSLLIVNNATNVVIKVCEFQFCNDPF

==> splike_b.faa <==
>pdb|7JJJ|B Chain B, Spike glycoprotein
MFVFLVLLPLVSSQCVNLTTRTQLPPAYTNSFTRGVYYPDKVFRSSVLHSTQDLFLPFFSNVTWFHAIHV
SGTNGTKRFDNPVLPFNDGVYFASTEKSNIIRGWIFGTTLDSKTQSLLIVNNATNVVIKVCEFQFCNDPF

==> splike_c.faa <==
>pdb|7JJJ|C Chain C, Spike glycoprotein
MFVFLVLLPLVSSQCVNLTTRTQLPPAYTNSFTRGVYYPDKVFRSSVLHSTQDLFLPFFSNVTWFHAIHV
SGTNGTKRFDNPVLPFNDGVYFASTEKSNIIRGWIFGTTLDSKTQSLLIVNNATNVVIKVCEFQFCNDPF



**Respuesa 4** 
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data

splike_a.faa splike_b.faa splike_c.faa >> 
/c/Users/home/genomicacomputacional/xconde_p01/data/filtered/glycoproteins.faa]

** Respuesta 5** 
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data

[mv] [] [splike_*.faa >> /c/Users/home/genomicacomputacional/xconde_p01/archive]
 
**Respuesta 6**
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data

[nano] [] [sarscov2_genome.fasta]
[zless] [sarscov2_assemly.fasta.gz]
[zless] [sarscov2_assembly.fasta.gz] | [head -3] [>> /c/Users/genomicacomptacional/xconde_p01/comandos_p01.md]
[head] [-3] [>/c/Users/genomicacomptacional/xconde_p01/comandos_p01.md]
 
>NODE_1_length_264_cov_161.042781
CACAAATCTTAACACTCTTCCCTACACGACGCTCTTCCGATCTACGCCGGGCCATTCGTA
CGAACCGATACCTGTGGTAAAGGGTCCTACTGTATGGTGGTACACGAGTAGTAGCAAATG

>gi|1798174254|ref|NC_045512.2| Severe acute respiratory syndrome coronavirus 2 isolate Wuhan-Hu-1, complete genome
ATTAAAGGTTTATACCTTCCCAGGTAACAAACCAACCAACTTTCGATCTCTTGTAGATCTGTTCTCTAAA
CGAACTTTAAAATCTGTGTGGCTGTCACTCGGCTGCATGCTTAGTGCACTCACGCAGTATAATTAATAAC
 
El número de lecturas en el archivo .gz es mayor debido a que se 
encuentra comprimido por lo que existe la posibiidad de guardar más 
y que tenga menos pesomientras que el archivo fasta está con el peso 
y la cantidad de lecturas que se pudieron guardar.

**Respuesta 7** 
#~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data
[zless] [sarscov2_assembly.fasta.gz | grep '>']

35 

[less] [sarscov2_genome.fasta | grep '>']

1

 **Respuesta 8**
 #~/c/Users/Vanessa/genomicacomputacional/xconde_p01/data/raw_data

[zless] [SRR10971381_R2.fastq.gz] 
 
[zless] [SRR10971381_R2.fastq.gz | grep '@'] 
son 130002 secuencias 

@SRR10971381.512_2 
CGTGGAGTATGGCTACATACTACTTATTTGATGAGTCTGGTGAGTTTAAAGTGGCTTCACATATGTATTGTTCTTTCTACCCTCCAGATGAGGATGAAGAAGAAGGTGATTGTGAAGAAGAAGAGTTTGAGCCATCAACTCAATATGAGT 
+ 
/FFFA/A/FFFF66FFFFFF/FF/FFFFFFFFFFFFF/AFFF6FFFA6FFFFF/FFFFFFFFFFFFFFFFFF/FF/FFFFFA/FFF/FFF/A/AFA/FFFFF/=F/F/F/AFAFF//A/AFF//FFAF/FFF=FFAFFFA/A/6=///== 
@SRR10971381.556_2 
TTTGTAAAAATAAAATAAAAAAAATAAAAATAATATATTAAAAAAAGATAAATAAAAAAATGAACAATTAATAAAAAAAAAAAAAAAAAAAAATTAAAAAAAAAAAAAAAAAAAATAAAAAAAAAAAAAAATAAAAAAAAAATTATAAAA 
+ 
6AFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF/FFFAFFFFFF/FFA/FF=F//=FF/FFFFFFFFFFFFFA/FFFF/FF/FA//F/FFFFFFA/=FFFFF/FFFF/F=FFFAFF///FFFFA/FF/6//////=/ 
@SRR10971381.1428_2 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA + 
FFFFFFFFFFFFAFFFAFFFFFF6A//F//FFF 
**Respuesta 9**
 
Nucleótidos se encuentran en la secuencia de formato .fasta. Aminoacidos se encuentran en el formato .faa El 
formato fastqc contiene secuencias tanto de aminoacidos como de nucleótidos , y de algunos codones que codifican para aminoacidos

**Respuesta 10** 


[less] [-S] [less -S sarscov2_genome.gff3]

[less] [sequence.gff3]

La diferencia de less y less -s es que en less se muestran los 
datos de forma justificada y con un orden en el que los datos no se aprecian de 
manera clara , mientras que en el otro al escribirse en una sola linea se aprecia 
más la correspondencia de cada dato.

**Respuesta 11**

[cut] [-f3] [sarscov2_genome.gff3 | grep -c gene]

El cds es una porcion codificante de ADN del gen, mientras que el gen se refiere a 
la secuencia completa de ADN perteneciente a ciierto gen.
 
