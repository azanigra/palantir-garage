# Normativa Municipal Bonaerense

Open source tool for searching municipal regulations and public spending across Buenos Aires province, Argentina.

Data sourced from [SIBOM](https://sibom.slyt.gba.gob.ar) (Sistema de Boletines Oficiales Municipales) — official provincial platform. No editorial bias. Just public data.

## What it does

- Shows spending and regulations across four pillars: health, education, security, infrastructure
- Searchable by keyword, municipality, and regulation type
- Data in plain JSON — easy to update and extend

## Structure

```
index.html        main app
data/
  lamatanza.json  municipal data (extend with more municipalities)
LICENSE
README.md
```

## Adding more municipalities

Each entry in the JSON follows this schema:

```json
{
  "num": "24265",
  "fecha": "2016-01-01",
  "tipo": "presupuesto",
  "titulo": "Description of the regulation",
  "monto": 4219801121,
  "expediente": "HCD 502/16",
  "municipio": "La Matanza"
}
```

## License

BSD 2-Clause — see LICENSE file.

Part of the [Palantir Garage](https://github.com/azanigra/palantir-garage) project.
