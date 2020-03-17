# RS3D config Cheetah V1.1x
## Procedure pour modifier et faire ca prope compilation
    - Copier/coller les fichier Configuration_adv.h et Configuration.h du dossier  config et les placer dans le dossier Marlin
    - Modifier dans le fichier platformio.ini le "default_envs = mega2560" par default_envs = STM32F103RC_fysetc

## Procedure flash firmaware
    https://wiki.fysetc.com/Cheetah_Board/
    section Upload the firmware(windows)
    une fois le flash effectuer fait une initialisation eeprom
        -configuration
            config_avance
                en bas du menu initialise eeprom
                    clic INIT attendre 2/3s couper l'imprimante puis la relancer.
#### 14/03/2020
    Mise a jour avec la version 2.0.5

#### 04/03/2020
    configuration marlin 2.0.x pour Cheetah V1.1x 
    changement:
        - langue mis en francais
        - configuration BLTouch_V3.x(en cours)
        - creation du .hex