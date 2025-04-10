___
EXPLAIN ANALYZE
SELECT * FROM tipg.tipg_catalog(
    schemas := ARRAY['public'],  -- Replace with your desired schema(s)
    tables := NULL,              -- NULL means include all tables
    exclude_tables := NULL,      -- Exclude specific tables if needed
    exclude_table_schemas := NULL,
    functions := NULL,           -- NULL means include all functions
    exclude_functions := NULL,
    exclude_function_schemas := NULL,
    spatial := FALSE,            -- Set to TRUE if only spatial tables/functions are needed
    spatial_extent := FALSE,
    datetime_extent := TRUE
);
