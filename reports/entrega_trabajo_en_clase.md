# Entrega trabajo en clase — 2025-10-29 11:37

## Avances realizados
- Estructura de experimentos creada (`experiments/` y notebook).
- Descarga de datasets enero y marzo 2025 (`data/green_tripdata_2025-01.parquet`, `...-03.parquet`).
- Entrenamiento con **RandomForest** y **GradientBoosting** con *child experiments* (Optuna).
- Métricas registradas en MLflow (train/validation RMSE).

## Comparación Champion vs Challenger (sobre marzo 2025)
- Challenger: **no disponible** (detalle: RestException: RESOURCE_DOES_NOT_EXIST: Routine or Model 'workspace.default.nyc_taxi_model' does not exist.)
- Champion: **no disponible** (detalle: RestException: RESOURCE_DOES_NOT_EXIST: Routine or Model 'workspace.default.nyc_taxi_model' does not exist.)

## Siguiente paso (mañana)
- Registrar el mejor run en **Unity Catalog** y asignar alias `challenger`.
- Si no existe `champion`, inicializarlo con el challenger actual.
- Re-evaluar y decidir promoción `challenger → champion` con criterio de mejora.

## Mejores runs por `validation_rmse` (top 10)
1. **run_id**: `b9999edbc0354eff84143de8b7b7ec3e` — **metrics**: {'validation_rmse': 5.971753001161576} — **tags**: {}
2. **run_id**: `002fc2ced57140be804a3786052cb913` — **metrics**: {'validation_rmse': 5.9854243429564065} — **tags**: {}
3. **run_id**: `19c06997b651476292ab651d0924281c` — **metrics**: {'validation_rmse': 6.000273746357954} — **tags**: {}
4. **run_id**: `f8d7fade52ca40db95dfc0e29c6a3687` — **metrics**: {'validation_rmse': 6.000684030772848} — **tags**: {}
5. **run_id**: `128911a442b74b518caec8ec450e0a6e` — **metrics**: {'validation_rmse': 6.016830998488338} — **tags**: {}
6. **run_id**: `d7141fbb3d1e4a4a89b2efa9ff81b68c` — **metrics**: {'validation_rmse': 6.0284808673533465} — **tags**: {}
7. **run_id**: `910cd9bf918b4c5ea814beffeeac1604` — **metrics**: {'validation_rmse': 6.03511996831642} — **tags**: {}
8. **run_id**: `b6a6195722364bd781c7c03ed43ec2db` — **metrics**: {'validation_rmse': 6.036067316351653} — **tags**: {}
9. **run_id**: `f0a9edb5280f4568baca40f241be8ec3` — **metrics**: {'validation_rmse': 6.042634473207194} — **tags**: {}
10. **run_id**: `8abe4f2c1944419596aa08e39a209eaa` — **metrics**: {'validation_rmse': 6.049592558740287} — **tags**: {}