SELECT column_name, data_type, is_nullable
FROM COMM_DEV.INFORMATION_SCHEMA.COLUMNS
WHERE table_schema = 'GOLD'
  AND table_name   = 'FIELD_ACTIVITY_METRIC'
ORDER BY ordinal_position;


Use Case	Technique	Output
UC1: Smart Metadata Insights	Cortex LLM (COMPLETE)	Daily AI-generated insights on freshness, growth, usage, quality
UC2: Anomaly Detection	Cortex ML (ANOMALY_DETECTION)	Daily anomaly flags on row count, avg metric value + AI explanations
