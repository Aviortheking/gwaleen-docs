# gwaleen-docs

### Commandes

| émetteur | trame                     | description                                                           |
| -------- | ------------------------- | --------------------------------------------------------------------- |
| tablette | `a#`                      | requête de ping a la règle                                            |
| règle    | `%a:e#`                   | réponse du ping de la règle                                           |
| tablette | `b#`                      | requête des information de la règle                                   |
| règle    | `%b:[NAME],[VERSION],#`   | réponse du nom et de la version de la règle                           |
| tablette | `&q#`                     | requête sur le pourcentage de batterie                                |
| règle    | `%q:[PERCENT_OF_BATT],0#` | réponse du pourcentage de batterie                                    |
| tablette | `&t#`                     | requête pour l'humidité et la température du boitier                  |
| règle    | `$t,[TEMP] °C,[HUM] %#`   | réponse pour l'humidité et la température du boitier                  |
| règle    | `%l,[VAL]#`               | prise de mesure de la règle en millimètre                             |
| règle    | `%t:0#`                   | envoyé quand l'aimant est déposé sur la règle (avant prise de mesure) |
| règle    | `%t:1#`                   | envoyé quand l'aimant est enlevé de la règle (après prise de mesure)  |

- *Toutes les commandes sont optionnel*
- *Toutes les commandes sont des Strings.*
- *Les commandes envoyées par la règle ne contienne pas de retours a la ligne.

### Usage Bluetooth

1. Activer le bluetooth sur la règle
2. Connectez-vous à la règle en Serial
3. Enjoy!

### Usage Filaire

Pré-requis Windows: https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers

1. Branchez la règle au PC
2. Il devrait il y avoir un port en plus de rajouté dans les périphériques
3. connectez vous en Serial RS-232
4. Enjoy!
