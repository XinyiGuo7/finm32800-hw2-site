# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ)

One row per contract per trading day, with columns date, symbol, open, high, low, close, and volume. A contract settles at 100 minus the average effective fed funds rate over its month, so 100 minus the close is the market's forecast of that average. The data includes calendar spreads such as ZQU6-ZQZ6; filter them out with fedwatch.filter_outright_contracts. The pull covers the trailing 180 days by default and is free under the course subscription.


## DataFrame Glimpse

```
Rows: 11787
Columns: 7
$ date   <datetime[ns]> 2026-10-23 00:00:00
$ symbol          <str> 'ZQZ6'
$ open            <f64> 95.965
$ high            <f64> 95.965
$ low             <f64> 95.945
$ close           <f64> 95.965
$ volume          <u64> 12677


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ)                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Futures, Monetary Policy, Fed Funds                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Python client (GLBX.MDP3, ohlcv-1d, parent symbol ZQ.FUT)                                                   |
| Data available up to (min)     | 2026-10-23 00:00:00                                                             |
| Data available up to (max)     | 2026-10-23 00:00:00                                                             |
| Dataframe Path                 | C:\Users\yannee\OneDrive\Desktop\hw2-XinyiGuo7\_data\fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file://C:/Users/yannee/OneDrive/Desktop/hw2-XinyiGuo7/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-25 14:23:55           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

