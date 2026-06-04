Scenario 1: Metadata-Driven Smart Insights Generation

The Problem
As pipelines grow, metadata accumulates — table descriptions, column lineage, data types, refresh schedules, ownership — but it just sits there. No one queries it meaningfully. Teams waste time hunting for “what does this field mean?” or “is this table still active?”

How Cortex AI Fits
Cortex AI can read and reason over your existing metadata as context. Instead of static documentation, you can ask natural language questions directly against your metadata layer — and get intelligent, contextual answers.

What This Looks Like in Practice

	•	“Which tables haven’t been refreshed in 7 days and are used in active dashboards?”
	•	“Summarise what the outlet_code field represents across all pipelines”
	•	“Which upstream sources feed into this gold table?”

Cortex processes the metadata as semantic context — not keyword search — so it handles complex, multi-hop questions that a simple lookup cannot.

Scenario 2: Anomaly Detection Beyond Rule-Based DQ Checks

The Problem
Traditional DQ checks are brittle — they catch what you anticipated would break. They miss drift, subtle pattern shifts, or multi-column anomalies that no single threshold would flag.

How Cortex AI Fits
Cortex AI can learn the normal behaviour of your data over time and flag deviations that don’t match any explicit rule — including volume drops, statistical outliers, unexpected nulls clustering together, or distribution shifts across a dimension.

What This Looks Like in Practice

	•	A product code that always has a unit price in a certain range suddenly shows values 10x higher — flagged without a hardcoded threshold
	•	Outlet records that typically arrive daily go silent for a region — caught as a pattern break, not a null check
	•	A combination of fields that individually look fine but together are statistically anomalous — something rule-based DQ cannot detect

The key difference: rules tell you what you know is wrong. Cortex tells you what you didn’t know to look for.
