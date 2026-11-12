# Thuisscherm

Wandscherm voor de tablet en bureaubladachtergrond voor de pc: energiestroom (SolarEdge + accu), kachel (SHPI), 3D-printer (Creality K2 Pro), weer en agenda.

Zonder Home Assistant-koppeling draait het scherm op voorbeelddata; het weer (Open-Meteo) is altijd live.

## Instellen via het adres

| Toevoeging | Wat het doet |
| --- | --- |
| `?breedte=55` | Gebruik 55% van de schermbreedte |
| `?positie=rechts` | `links`, `midden` of `rechts` |
| `?hoogte=70` | Gebruik 70% van de schermhoogte |
| `?verticaal=boven` | `boven`, `midden` of `onder` |
| `?schaal=75` | Tekst en onderdelen kleiner (75%) of groter (bijv. 120) |
| `?indeling=ultra` | `auto`, `ultra` (4 kolommen) of `normaal` |
| `?reset=1` | Alles terug naar standaard |
| `?token=...` | Home Assistant-token, wordt alleen op dit apparaat bewaard |

Combineer met `&`, bijvoorbeeld `?breedte=55&positie=rechts`.

## Bestanden

- `index.html`: het hele scherm in één bestand. Instellingen staan bovenin het script (`CONFIG`).
- `homeassistant/shpi.yaml`: koppeling van de SHPI-thermostaat aan Home Assistant.
