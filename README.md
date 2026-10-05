# datascience-project

Simple data pipeline design: **Weather API → Dashboard.**


[Assignment-1](https://docs.google.com/document/d/1ANH4dETwJcVe3SRfKSnpWw_wAIb8H6AjdevtbRL27-I/edit?usp=sharing)

## What is this?

I designed a simple pipeline that pulls weather data every 1 hour from OpenWeatherMap Public API, saves raw JSON, cleans it, and shows it on a dashboard for normal people.

No complex tools. Only what I can explain.

## Architecture

**Logical:**
```
Weather API → Ingestion → Raw Storage → Processing → Analytical Storage → Dashboard
```

**With Tools:**
```
OpenWeather API → Python (hourly) → Amazon S3 (raw) → Pandas (clean) → PostgreSQL → Power BI
```

## What's inside the doc?

1. Selected Source + data type
2. Diagram 1 — Logical Architecture
3. Diagram 2 — Technology Mapping
4. Why each component exists (1 line each)
5. Question Log — 6 real doubts
6. Why data moves forward (short story)

## Reference

Main guide: *What Data Pipeline Architecture should I use? — Google Cloud*

**Source → Processing → Target.** Logical first, tools later.
