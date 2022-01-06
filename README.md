# Rapport

### Mon ordinateur
    Architecture:                    x86_64
    CPU op-mode(s):                  32-bit, 64-bit
    Byte Order:                      Little Endian
    Address sizes:                   39 bits physical, 48 bits virtual
    CPU(s):                          8
    On-line CPU(s) list:             0-7
    Thread(s) per core:              2
    Core(s) per socket:              4
    Socket(s):                       1
    NUMA node(s):                    1
    Vendor ID:                       GenuineIntel
    CPU family:                      6
    Model:                           158
    Model name:                      Intel(R) Core(TM) i5-8300H CPU @ 2.30GHz
    Stepping:                        10
    CPU MHz:                         2300.000
    CPU max MHz:                     4000,0000
    CPU min MHz:                     800,0000
    BogoMIPS:                        4599.93
    Virtualization:                  VT-x
    L1d cache:                       128 KiB
    L1i cache:                       128 KiB
    L2 cache:                        1 MiB
    L3 cache:                        8 MiB
    NUMA node0 CPU(s):               0-7


## First part - Point 2.1 (Simulation V1)
        
    Début boucle épidémie
        Temps de calcul de la simulation par jour : 0.0181674s
        Temps de calcul de l'affichage par jour : 0.0138341s
        Temps de calcul global par jour : 0.0321879s

Le temps global que nous pouvons observer est simplement la somme des temps de calcul de la simulation et de l'affichage.

##  Second part - Point 2.2 (Simulation V2)

    Début boucle épidémie

	Temps de calcul de la simulation par jour : 0.0335138s
	Temps de calcul global par jour : 0.0335151s
	Temps de calcul de l'affichage par jour : 0.0331582s

nous ne pouvons pas voir un changement significatif ou une amélioration sur le speed up parce que les conditions sont de type bloquant, l'envoi et la réception de messages de la grille définie doivent toujours attendre que l'autre processus lève la main, afin de continuer avec le jour suivant. 
