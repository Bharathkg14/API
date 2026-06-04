Need admin to create CORTEX_POC DB (request sent)


Isolation. We’re running AI functions that generate new tables, views, and ML models. Doing this in a dedicated CORTEX_POC database means:

Zero risk to production — no accidental writes to COMM_DEV.GOLD
Easy cleanup — drop one database when POC ends, no orphan objects
Clear ownership — my role owns it, no permission conflicts with shared schemas
