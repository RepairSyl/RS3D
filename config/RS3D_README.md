# RS3D config SKR Mini E3 1.2

## Les configs

   
 Option                         |Base      |Touchmi_10|Touchmi_20|Bltouch
 -------------------------------|----------|----------|----------|----------
 PID_EDIT_MENU                  |   OUI    |   OUI    |   OUI    |   OUI
 PIDTEMP                        |   OUI    |   OUI    |   OUI    |   OUI
 PID_AUTOTUNE_MENU              |   OUI    |   OUI    |   OUI    |   OUI
 CLASSIC_JERK                   |   OUI    |   OUI    |   OUI    |   OUI    
 S_CURVE_ACCELERATION           |   OUI    |   OUI    |   OUI    |   OUI
 MESH_BED_LEVELING              |   OUI    |   NON    |   NON    |   NON
 AUTO_BED_LEVELING_BILINEAR     |   NON    |   OUI    |   OUI    |   OUI
 RESTORE_LEVELING_AFTER_G28     |   OUI    |   OUI    |   OUI    |   OUI
 LCD_BED_LEVELING               |   OUI    |   OUI    |   OUI    |   OUI
 LEVEL_BED_CORNERS Z=0.1        |   OUI    |   OUI    |   OUI    |   OUI
 NOZZLE_PARK_FEATURE            |   OUI    |   OUI    |   OUI    |   OUI
 LCD_LANGUAGE fr                |   OUI    |   OUI    |   OUI    |   OUI
 INDIVIDUAL_AXIS_HOMING_MENU    |   OUI    |   OUI    |   OUI    |   OUI
 ADAPTIVE_STEP_SMOOTHING        |   OUI    |   OUI    |   OUI    |   OUI
 DOGM_SD_PERCENT                |   OUI    |   OUI    |   OUI    |   OUI
 BABYSTEPPING                   |   OUI    |   OUI    |   OUI    |   OUI
 LIN_ADVANCE k=0.0              |   OUI    |   OUI    |   OUI    |   OUI
 ADVANCED_PAUSE_FEATURE         |   OUI    |   OUI    |   OUI    |   OUI
 MONITOR_DRIVER_STATUS          |   OUI    |   OUI    |   OUI    |   OUI
 TMC_DEBUG                      |   OUI    |   OUI    |   OUI    |   OUI
 CUSTOM_USER_MENUS              |   OUI    |   OUI    |   OUI    |   OUI
### Procedure 
    - dans le dossier marlin ce trouve la version de base
    Si vous souhaiter changer de config il suffit de remplacer les fichier par la config que vous souhitez modifier. 
    - Copier/coller les fichier Configuration_adv.h et Configuration.h du dossier  config et les placer dans le dossier Marlin
    
#### CUSTOM_USER_MENU
    Home
    Home/Preheat PLA : fait une home XYZ(G28) + prechaufe le BED 
    Home/Preheat ABS : fait une home XYZ(G28) + prechaufe le BED 
    Home/Level Bed : fait une home XYZ(G28) + leveling bed (G29)
    Extrude 100mm   


#### 20/03/2020
    -mise a jours marlin 2.0.5.1
    -creation config touchmi et bltouch
        MIN_PROBE_EDGE 10 pour ender3pro
        MIN_PROBE_EDGE 20 pour ender3 
    - regle pour machine d'origine NOZZLE_TO_PROBE_OFFSET x-44 y-6  les modifier si vous etes sur un system de fang

explication MIN_PROBE_EDGE         
<img align="center" width=500 src="https://github.com/RepairSyl/Marlin_Partage/blob/master/MIN_PROBE_EDGE.PNG" />

#### 14/03/2020
    Mise a jour avec la version 2.0.5

#### 04/03/2020
    configuration marlin Version 2.0.4.4 pour SKR mini E3 V1.2 
    changement:
        - langue mis en francais
        - creation du .bin