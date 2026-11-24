# Tennis BI — ATP 1991–2026

Projet de Business Intelligence (ECE) : ETL Talend + tableau de bord Power BI sur les matchs ATP.

## Source des données

- **Jeu de données** : [JeffSackmann/tennis_atp](https://github.com/JeffSackmann/tennis_atp) (Jeff Sackmann / Tennis Abstract)
- **Licence** : [CC BY-NC-SA 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/). Il faut citer la source, l'usage commercial est interdit et les œuvres dérivées doivent être partagées sous la même licence.
- Le README original est conservé dans `data/raw/UPSTREAM_README.md`, et le dictionnaire des colonnes dans `data/raw/matches_data_dictionary.txt`.

## Arborescence

```
.
├── data/
│   ├── raw/        ← atp_matches_1991..2026.csv (36 fichiers) + atp_players.csv + documentation source
│   ├── clean/      ← sorties Talend (CSV finaux)
│   └── archive/    ← fichiers source hors périmètre (matchs 1968–1990, futures, qual/chall, doubles, rankings, amateur)
├── talend/         ← exports .zip des jobs
├── powerbi/        ← le .pbix
├── report/         ← rapport + captures/
└── README.md
```

## Chemins

| Élément | Chemin |
|---|---|
| Entrées Talend | `data/raw/atp_matches_*.csv`, `data/raw/atp_players.csv` |
| Sorties Talend | `data/clean/` |
| Source Power BI | `data/clean/` |
| Jobs Talend exportés | `talend/*.zip` |
| Rapport | `report/` |
