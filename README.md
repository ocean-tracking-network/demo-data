# Project LATiTuDeS
***Library of Aquatic Tracking and Telemetry Data Samples***

## Library structure

```
latitudes/
  |-- Raw/
     |-- Vendor1/
          |-- InstrumentA/
               |-- software version 1.0/
                    |-- file123.ext
                    |-- metadata.yaml
          |-- ...
     |-- Vendor2/
     |-- ...
  |-- Derived/
     |-- Network1/
     |-- Network2/
     |-- ...
  |-- Network Schema/
  |-- Forms/
```

## File metadata schema
Files must be associated with a `metadata.yaml` file providing its context, attribution, and licensing. The current schema is found within [`schema-guide.md`](schema-guide.md) and validated against [`test/validation-schema.yaml`](test/validation-schema.yaml).

## Contributing and data needs
- Raw
   - Vemco/Innovasea (Current: VRL, VDAT; Legacy: binary, text)
   - Lotek
   - ThelmaBiotel
   - Sonotronics
- Derived
   - Vemco/Innovasea ("non-truth" VRL, CSV)
   - OTN matched/unmatched/qualified/unqualified/other networks
   - GLATOS and `glatos`
   - ETN and `etn`
   - IMOS
   - Actel
   - Deployment data, various forms
- Forms
   - OTN/FACT/MATOS/ETN/GLATOS metadata forms (multiple versions)
- Schema
   - OTN (multiple across Geoserver and exports)
   - GLATOS 
