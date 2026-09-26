# Data required to rerun the notebooks

The original source CSV files are not included in this public-facing portfolio package. The first three notebooks expect these filenames in their working directory:

- `CO2Emis.csv`: five-minute Energinet DK1 emissions observations (semicolon-separated, comma decimals).
- `ProductionConsumptionSettlement.csv`: hourly Energinet DK1 settlement data (semicolon-separated, comma decimals).
- `dmi_station06072_2022_2024_temp_wind_solar_clean.csv`: ten-minute DMI station observations.

They produce these processed CSV files for the fourth notebook:

- `co2_dk1_hourly_2022_2024.csv`: hourly DK1 CO₂ intensity, with `datetime_utc` and `co2_intensity`.
- `pcs_processed_dk1_utc.csv`: processed hourly DK1 production and consumption settlement data, with `datetime_utc` and `GrossConsumptionMWh` among its columns.
- `weather_dk1_hourly_2022_2024.csv`: hourly weather observations, with `datetime_utc`, `temperature`, `wind_speed` and `solar_radiation`.

The fourth notebook produces `final_dataset_model_ready.csv` for the fifth. Consult the notebooks and thesis for column definitions and transformations. Obtain source data from Energinet and DMI subject to their current terms. The PDF and saved notebook outputs allow review of the original analysis without these files.
