# Task 1 — Operational Downtime Analysis

## Objective

Analyze Daikibo machine telemetry data to identify factories with the highest potential downtime and determine which device types contribute to downtime within the selected factory.

## Methodology

### 1. Downtime metric

The telemetry data contains a machine `Status` field.

For this simulation, each `unhealthy` status represents **10 minutes of potential downtime**.

The Tableau calculated field used was:

```text
IF [Status] = 'unhealthy' THEN 10
ELSE 0
END
```

The resulting measure was aggregated using `SUM(Unhealthy)`.

### 2. Factory analysis

Potential downtime was aggregated by `Factory` to compare operational impact across locations.

### 3. Device analysis

Potential downtime was aggregated by `Device Type`.

### 4. Interactive filtering

The factory chart was configured as a dashboard filter. Selecting a factory dynamically filters the device-type chart to that factory.

## Key Finding

The highest potential downtime was recorded at:

**daikibo-factory-seiko — 480 minutes**

With Seiko selected, the device-level analysis shows:

**LaserWelder — 480 minutes**

This identifies the location and device type that warrant further operational investigation.

> The analysis identifies an association in the telemetry data. It does not by itself establish the root cause of the downtime.

## Dashboard

Add the final Tableau dashboard screenshot below:

`../screenshots/operational-analysis.png`

## Tools

- Tableau
- JSON telemetry data
- Calculated fields
- Interactive dashboard filtering
