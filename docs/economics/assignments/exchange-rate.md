# Exchange Rate

```vegalite
{
  "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
  "title": "Currency Exchange Rates Over Time",
  "description": "A line graph showing the exchange rates of various currencies to USD over time",
  "data": {
    "values": [
      {
        "Date": "2023-01-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0776
      },
      {
        "Date": "2023-01-11",
        "Currency": "EURUSD",
        "ExchangeRate": 1.057
      },
      {
        "Date": "2023-02-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0477
      },
      {
        "Date": "2023-02-11",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0621
      },
      {
        "Date": "2023-03-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0466
      },
      {
        "Date": "2023-03-11",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0732
      },
      {
        "Date": "2023-04-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0796
      },
      {
        "Date": "2023-04-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0505
      },
      {
        "Date": "2023-05-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0721
      },
      {
        "Date": "2023-05-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0551
      },
      {
        "Date": "2023-06-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0725
      },
      {
        "Date": "2023-06-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.059
      },
      {
        "Date": "2023-06-11",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0719
      },
      {
        "Date": "2023-07-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0696
      },
      {
        "Date": "2023-08-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0702
      },
      {
        "Date": "2023-08-14",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0906
      },
      {
        "Date": "2023-08-15",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0906
      },
      {
        "Date": "2023-08-16",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0879
      },
      {
        "Date": "2023-08-17",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0873
      },
      {
        "Date": "2023-08-18",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0873
      },
      {
        "Date": "2023-08-21",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0896
      },
      {
        "Date": "2023-08-22",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0845
      },
      {
        "Date": "2023-08-23",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0863
      },
      {
        "Date": "2023-08-24",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0811
      },
      {
        "Date": "2023-08-25",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0796
      },
      {
        "Date": "2023-08-28",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0821
      },
      {
        "Date": "2023-08-29",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0881
      },
      {
        "Date": "2023-08-30",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0924
      },
      {
        "Date": "2023-08-31",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0843
      },
      {
        "Date": "2023-09-08",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0974
      },
      {
        "Date": "2023-09-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0569
      },
      {
        "Date": "2023-09-13",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0732
      },
      {
        "Date": "2023-09-14",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0642
      },
      {
        "Date": "2023-09-15",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0659
      },
      {
        "Date": "2023-09-18",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0692
      },
      {
        "Date": "2023-09-19",
        "Currency": "EURUSD",
        "ExchangeRate": 1.068
      },
      {
        "Date": "2023-09-20",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0661
      },
      {
        "Date": "2023-09-21",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0662
      },
      {
        "Date": "2023-09-22",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0646
      },
      {
        "Date": "2023-09-25",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0593
      },
      {
        "Date": "2023-09-26",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0573
      },
      {
        "Date": "2023-09-27",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0505
      },
      {
        "Date": "2023-09-28",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0568
      },
      {
        "Date": "2023-09-29",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0573
      },
      {
        "Date": "2023-10-08",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0982
      },
      {
        "Date": "2023-10-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0608
      },
      {
        "Date": "2023-10-13",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0511
      },
      {
        "Date": "2023-10-16",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0561
      },
      {
        "Date": "2023-10-17",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0576
      },
      {
        "Date": "2023-10-18",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0538
      },
      {
        "Date": "2023-10-19",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0584
      },
      {
        "Date": "2023-10-20",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0595
      },
      {
        "Date": "2023-10-23",
        "Currency": "EURUSD",
        "ExchangeRate": 1.067
      },
      {
        "Date": "2023-10-24",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0591
      },
      {
        "Date": "2023-10-25",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0567
      },
      {
        "Date": "2023-10-26",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0563
      },
      {
        "Date": "2023-10-27",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0563
      },
      {
        "Date": "2023-10-30",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0616
      },
      {
        "Date": "2023-10-31",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0577
      },
      {
        "Date": "2023-11-08",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0947
      },
      {
        "Date": "2023-11-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.075
      },
      {
        "Date": "2023-11-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0618
      },
      {
        "Date": "2023-12-09",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0756
      },
      {
        "Date": "2023-12-10",
        "Currency": "EURUSD",
        "ExchangeRate": 1.0531
      },
      {
        "Date": "2023-01-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1377
      },
      {
        "Date": "2023-01-11",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-02-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-02-11",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-03-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1389
      },
      {
        "Date": "2023-03-11",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-04-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1375
      },
      {
        "Date": "2023-04-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1389
      },
      {
        "Date": "2023-05-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1369
      },
      {
        "Date": "2023-05-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1389
      },
      {
        "Date": "2023-06-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-06-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.139
      },
      {
        "Date": "2023-06-11",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1376
      },
      {
        "Date": "2023-07-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1365
      },
      {
        "Date": "2023-08-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1362
      },
      {
        "Date": "2023-08-14",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1378
      },
      {
        "Date": "2023-08-15",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1373
      },
      {
        "Date": "2023-08-16",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-08-17",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1373
      },
      {
        "Date": "2023-08-18",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1373
      },
      {
        "Date": "2023-08-21",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1381
      },
      {
        "Date": "2023-08-22",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-08-23",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1374
      },
      {
        "Date": "2023-08-24",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1374
      },
      {
        "Date": "2023-08-25",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1372
      },
      {
        "Date": "2023-08-28",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1372
      },
      {
        "Date": "2023-08-29",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1373
      },
      {
        "Date": "2023-08-30",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1373
      },
      {
        "Date": "2023-08-31",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1378
      },
      {
        "Date": "2023-09-08",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1387
      },
      {
        "Date": "2023-09-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-09-13",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1375
      },
      {
        "Date": "2023-09-14",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1374
      },
      {
        "Date": "2023-09-15",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1375
      },
      {
        "Date": "2023-09-18",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-09-19",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-09-20",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1372
      },
      {
        "Date": "2023-09-21",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-09-22",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-09-25",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-09-26",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-09-27",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-09-28",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-09-29",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-10-08",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1386
      },
      {
        "Date": "2023-10-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-10-13",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1369
      },
      {
        "Date": "2023-10-16",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-10-17",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-18",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-19",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-20",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-23",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-24",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1368
      },
      {
        "Date": "2023-10-25",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-26",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-27",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-30",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-10-31",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1367
      },
      {
        "Date": "2023-11-08",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1382
      },
      {
        "Date": "2023-11-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1372
      },
      {
        "Date": "2023-11-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.137
      },
      {
        "Date": "2023-12-09",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1371
      },
      {
        "Date": "2023-12-10",
        "Currency": "CNYUSD",
        "ExchangeRate": 0.1369
      },
      {
        "Date": "2023-01-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6453
      },
      {
        "Date": "2023-01-11",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6393
      },
      {
        "Date": "2023-02-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6362
      },
      {
        "Date": "2023-02-11",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6433
      },
      {
        "Date": "2023-03-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6302
      },
      {
        "Date": "2023-03-11",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6513
      },
      {
        "Date": "2023-04-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6462
      },
      {
        "Date": "2023-04-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6326
      },
      {
        "Date": "2023-05-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.638
      },
      {
        "Date": "2023-05-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6372
      },
      {
        "Date": "2023-06-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6382
      },
      {
        "Date": "2023-06-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6386
      },
      {
        "Date": "2023-06-11",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6491
      },
      {
        "Date": "2023-07-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6375
      },
      {
        "Date": "2023-08-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6379
      },
      {
        "Date": "2023-08-14",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6487
      },
      {
        "Date": "2023-08-15",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6454
      },
      {
        "Date": "2023-08-16",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6423
      },
      {
        "Date": "2023-08-17",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6405
      },
      {
        "Date": "2023-08-18",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6404
      },
      {
        "Date": "2023-08-21",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6414
      },
      {
        "Date": "2023-08-22",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6422
      },
      {
        "Date": "2023-08-23",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.648
      },
      {
        "Date": "2023-08-24",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6417
      },
      {
        "Date": "2023-08-25",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6403
      },
      {
        "Date": "2023-08-28",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6431
      },
      {
        "Date": "2023-08-29",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.648
      },
      {
        "Date": "2023-08-30",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6476
      },
      {
        "Date": "2023-08-31",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6483
      },
      {
        "Date": "2023-09-08",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6529
      },
      {
        "Date": "2023-09-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6412
      },
      {
        "Date": "2023-09-13",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6424
      },
      {
        "Date": "2023-09-14",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6441
      },
      {
        "Date": "2023-09-15",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6435
      },
      {
        "Date": "2023-09-18",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6438
      },
      {
        "Date": "2023-09-19",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6454
      },
      {
        "Date": "2023-09-20",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6448
      },
      {
        "Date": "2023-09-21",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6414
      },
      {
        "Date": "2023-09-22",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6444
      },
      {
        "Date": "2023-09-25",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6425
      },
      {
        "Date": "2023-09-26",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6397
      },
      {
        "Date": "2023-09-27",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6352
      },
      {
        "Date": "2023-09-28",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6426
      },
      {
        "Date": "2023-09-29",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6433
      },
      {
        "Date": "2023-10-08",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6516
      },
      {
        "Date": "2023-10-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6431
      },
      {
        "Date": "2023-10-13",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6297
      },
      {
        "Date": "2023-10-16",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6342
      },
      {
        "Date": "2023-10-17",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6365
      },
      {
        "Date": "2023-10-18",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6338
      },
      {
        "Date": "2023-10-19",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6329
      },
      {
        "Date": "2023-10-20",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6315
      },
      {
        "Date": "2023-10-23",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6337
      },
      {
        "Date": "2023-10-24",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6354
      },
      {
        "Date": "2023-10-25",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6307
      },
      {
        "Date": "2023-10-26",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6323
      },
      {
        "Date": "2023-10-27",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6333
      },
      {
        "Date": "2023-10-30",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6375
      },
      {
        "Date": "2023-10-31",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6338
      },
      {
        "Date": "2023-11-08",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6497
      },
      {
        "Date": "2023-11-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6433
      },
      {
        "Date": "2023-11-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6414
      },
      {
        "Date": "2023-12-09",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6425
      },
      {
        "Date": "2023-12-10",
        "Currency": "AUDUSD",
        "ExchangeRate": 0.6315
      },
      {
        "Date": "2023-01-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2591
      },
      {
        "Date": "2023-01-11",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.215
      },
      {
        "Date": "2023-02-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2086
      },
      {
        "Date": "2023-02-11",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2203
      },
      {
        "Date": "2023-03-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2077
      },
      {
        "Date": "2023-03-11",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2381
      },
      {
        "Date": "2023-04-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2628
      },
      {
        "Date": "2023-04-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2135
      },
      {
        "Date": "2023-05-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2565
      },
      {
        "Date": "2023-05-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2193
      },
      {
        "Date": "2023-06-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2507
      },
      {
        "Date": "2023-06-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2239
      },
      {
        "Date": "2023-06-11",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2342
      },
      {
        "Date": "2023-07-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2471
      },
      {
        "Date": "2023-08-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2467
      },
      {
        "Date": "2023-08-14",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2687
      },
      {
        "Date": "2023-08-15",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2706
      },
      {
        "Date": "2023-08-16",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2732
      },
      {
        "Date": "2023-08-17",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2746
      },
      {
        "Date": "2023-08-18",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2735
      },
      {
        "Date": "2023-08-21",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2756
      },
      {
        "Date": "2023-08-22",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2732
      },
      {
        "Date": "2023-08-23",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2724
      },
      {
        "Date": "2023-08-24",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2601
      },
      {
        "Date": "2023-08-25",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2579
      },
      {
        "Date": "2023-08-28",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2602
      },
      {
        "Date": "2023-08-29",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2643
      },
      {
        "Date": "2023-08-30",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2721
      },
      {
        "Date": "2023-08-31",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2673
      },
      {
        "Date": "2023-09-08",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2717
      },
      {
        "Date": "2023-09-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2239
      },
      {
        "Date": "2023-09-13",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2489
      },
      {
        "Date": "2023-09-14",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2408
      },
      {
        "Date": "2023-09-15",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2383
      },
      {
        "Date": "2023-09-18",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2385
      },
      {
        "Date": "2023-09-19",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2393
      },
      {
        "Date": "2023-09-20",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2344
      },
      {
        "Date": "2023-09-21",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2296
      },
      {
        "Date": "2023-09-22",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2241
      },
      {
        "Date": "2023-09-25",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.221
      },
      {
        "Date": "2023-09-26",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2159
      },
      {
        "Date": "2023-09-27",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2135
      },
      {
        "Date": "2023-09-28",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2205
      },
      {
        "Date": "2023-09-29",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2199
      },
      {
        "Date": "2023-10-08",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2675
      },
      {
        "Date": "2023-10-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2287
      },
      {
        "Date": "2023-10-13",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2145
      },
      {
        "Date": "2023-10-16",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2217
      },
      {
        "Date": "2023-10-17",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2184
      },
      {
        "Date": "2023-10-18",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.214
      },
      {
        "Date": "2023-10-19",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2144
      },
      {
        "Date": "2023-10-20",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2165
      },
      {
        "Date": "2023-10-23",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2247
      },
      {
        "Date": "2023-10-24",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2159
      },
      {
        "Date": "2023-10-25",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2113
      },
      {
        "Date": "2023-10-26",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2129
      },
      {
        "Date": "2023-10-27",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.212
      },
      {
        "Date": "2023-10-30",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2169
      },
      {
        "Date": "2023-10-31",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2153
      },
      {
        "Date": "2023-11-08",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2696
      },
      {
        "Date": "2023-11-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2508
      },
      {
        "Date": "2023-11-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2314
      },
      {
        "Date": "2023-12-09",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2494
      },
      {
        "Date": "2023-12-10",
        "Currency": "GBPUSD",
        "ExchangeRate": 1.2174
      }
    ]
  },
  "mark": "line",
  "encoding": {
    "x": {
      "field": "Date",
      "type": "temporal",
      "axis": {
        "title": "Date"
      }
    },
    "y": {
      "field": "ExchangeRate",
      "type": "quantitative",
      "axis": {
        "title": "Exchange Rate"
      }
    },
    "color": {
      "field": "Currency",
      "type": "nominal",
      "legend": {
        "title": "Currency Pair"
      }
    },
    "tooltip": [
      {
        "field": "Date",
        "type": "temporal"
      },
      {
        "field": "Currency",
        "type": "nominal"
      },
      {
        "field": "ExchangeRate",
        "type": "quantitative"
      }
    ]
  },
  "height": 600
}
```