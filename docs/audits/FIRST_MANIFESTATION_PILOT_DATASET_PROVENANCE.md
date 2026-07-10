# First Manifestation Pilot Dataset Provenance

## Dataset Identity

Pilot name: First Manifestation Pilot - SPY Short-Horizon Momentum Validation.

Dataset artifact path: `data/pilot/spy_short_horizon_momentum/bounded/SPY_2015-01-01_2019-12-31_daily_adjusted_close.csv`.

Source artifact path: `data/pilot/spy_short_horizon_momentum/source/SPY_yahoo_chart_2015-01-01_2019-12-31_daily.json`.

Instrument: SPY.

Observation frequency: daily.

Field used: adjusted close, from Yahoo Finance `indicators.adjclose[0].adjclose`.

Registered date boundary: 2015-01-01 through 2019-12-31, inclusive where observations exist.

Research use: first Manifestation pilot only.

## Source Provenance

Provider: Yahoo Finance.

Retrieval mechanism: direct HTTP retrieval from the Yahoo Finance chart JSON endpoint.

Retrieval timestamp: 2026-07-09T19:45:19Z.

Source instrument identifier: `SPY`.

Requested date range: `period1=1420070400` and `period2=1577836800`, corresponding to 2015-01-01T00:00:00Z through 2020-01-01T00:00:00Z as an exclusive upper bound used to retrieve observations through 2019-12-31.

Source request URL:

```text
https://query1.finance.yahoo.com/v8/finance/chart/SPY?period1=1420070400&period2=1577836800&interval=1d&events=history&includeAdjustedClose=true
```

Source adjusted-close documentation: `https://help.yahoo.com/kb/SLN28256.html`.

Returned field names used or preserved:

- `timestamp`;
- `indicators.quote[0].open`;
- `indicators.quote[0].high`;
- `indicators.quote[0].low`;
- `indicators.quote[0].close`;
- `indicators.quote[0].volume`;
- `indicators.adjclose[0].adjclose`.

Returned metadata used for validation:

- `meta.symbol`: `SPY`;
- `meta.exchangeTimezoneName`: `America/New_York`;
- `meta.dataGranularity`: `1d`.

Source field semantics: Yahoo Finance documents adjusted close as the closing price after adjustments for applicable splits and dividend distributions. This pilot uses Yahoo's provided adjusted-close field and does not recompute adjustment factors.

Known source-specific limitations:

- Yahoo Finance historical data is a vendor-provided historical market-data source and may be revised by the provider.
- The chart endpoint is an implementation endpoint rather than a formal archival dataset release.
- Adjustment policy is accepted as Yahoo's vendor semantics; adjustment factors were not independently reconstructed.
- The source artifact includes additional OHLCV fields returned by the endpoint, but the bounded pilot artifact preserves only date and adjusted close.

## Transformation Provenance

Transformations from the source artifact to the bounded artifact:

1. Parsed the Yahoo Finance JSON source artifact.
2. Confirmed returned instrument metadata `SPY`.
3. Read observation timestamps and `adjclose` values from the returned arrays.
4. Converted each timestamp to an `America/New_York` market calendar date represented as `YYYY-MM-DD`.
5. Filtered rows to the frozen registered boundary, 2015-01-01 through 2019-12-31 inclusive where observations exist.
6. Selected only `date` and `adjusted_close`.
7. Serialized adjusted close as the base-10 decimal text representation of the Yahoo JSON numeric value.
8. Sorted rows by date ascending.
9. Rejected duplicate dates by validation; none were present.
10. Serialized the bounded artifact as UTF-8 CSV with LF line endings.

No analytical pilot transformations were performed. No 20-day returns, 5-day forward returns, group labels, comparison metrics, Hypothesis result, Evidence conclusion, or Decision recommendation were calculated.

## Integrity

Bounded artifact:

| Identifier | Value |
|---|---|
| File name | `SPY_2015-01-01_2019-12-31_daily_adjusted_close.csv` |
| Byte size | 37039 |
| Row count | 1258 |
| First observation | 2015-01-02 |
| Last observation | 2019-12-31 |
| SHA-256 | `591c3f8e654e611923ad46935f6c41724a24756b60dc3d6d2c3d9298c40406f7` |
| Schema | `date` as ISO-8601 `YYYY-MM-DD`; `adjusted_close` as decimal string |

Source artifact:

| Identifier | Value |
|---|---|
| File name | `SPY_yahoo_chart_2015-01-01_2019-12-31_daily.json` |
| Byte size | 139609 |
| Row count | 1258 timestamped source observations |
| First returned timestamp | 2015-01-02T14:30:00Z |
| Last returned timestamp | 2019-12-31T14:30:00Z |
| SHA-256 | `0e1b512a1b8fe19bcf3acdccc7d83ccff64a074d41569ce6721435883629dcd9` |
| Schema signature | Yahoo chart JSON with `timestamp`, `quote` OHLCV arrays, and `adjclose.adjclose` array |

## Quality Checks

| Check | Result |
|---|---|
| Registered contract matches preregistration | Pass: SPY daily adjusted close, 2015-01-01 through 2019-12-31, first pilot only |
| Source instrument identifier | Pass: source metadata returned `SPY` |
| Adjusted-close field present | Pass: `indicators.adjclose[0].adjclose` present |
| Schema | Pass: bounded CSV has exactly `date,adjusted_close` |
| Date parseability | Pass |
| Chronological ordering | Pass |
| Duplicate dates | Pass: none found |
| Missing adjusted-close values | Pass: none found |
| Non-finite adjusted-close values | Pass: none found |
| Observations outside registered boundary | Pass: none found |
| Unexpected empty dataset | Pass: 1258 rows |
| Basic observation count | 1258 rows |
| First available observation date | 2015-01-02 |
| Last available observation date | 2019-12-31 |
| NYSE expected session coverage | Pass: 1258 expected NYSE sessions, 1258 observed sessions |
| Missing expected sessions | Pass: none found |
| Unexpected observed sessions | Pass: none found |

Calendar gaps caused by weekends and market holidays were not treated as missing observations. No imputation, forward fill, or repair was applied.

## Known Limitations

- The dataset relies on Yahoo Finance as the chosen provider.
- The adjusted-close semantics rely on Yahoo's documented interpretation of adjusted close and Yahoo's returned `adjclose` field.
- No independent reconstruction of dividend or split adjustment factors was performed.
- No missing expected NYSE sessions were found for the registered boundary using `pandas_market_calendars` for a local integrity check.
- This exact bounded dataset artifact was not present in the repository at preregistration time. The preregistration records prior domain knowledge of the generic momentum idea and no inherited local VAKI Quant dataset context. External prior exposure to overlapping SPY historical data cannot be ruled out from repository evidence alone.
- The dataset is bounded to one instrument, one provider, one historical interval, and one adjusted-close field. It is not a general market-data archive.

## Observation Boundary Note

The stored price series is Data.

Dataset integrity checks do not make the dataset Evidence.

Measurements created during the registered investigation may become Observations under the pilot's Observation model only when preserved with sufficient provenance, context, scope, and limits.

Evidential meaning is assessed only later in relation to the frozen Hypothesis and context. This provenance record closes a data-materialization blocker; it does not execute the Experiment, create Evidence, assess the Hypothesis, or support a Decision recommendation.
