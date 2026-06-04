SELECT column_name, data_type, is_nullable
FROM COMM_DEV.INFORMATION_SCHEMA.COLUMNS
WHERE table_schema = 'GOLD'
  AND table_name   = 'FIELD_ACTIVITY_METRIC'
ORDER BY ordinal_position;
