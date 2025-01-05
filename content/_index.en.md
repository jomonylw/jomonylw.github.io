---
title: ""
description: ""
tags: ["Investment", "Financial Management", "Nasdaq Index", "Nasdaq-100", "Fund", "Stock", "ETF", "Portfolio", "Asset Allocation", "Financial Freedom", "Investment Strategy", "Investment & Financial Management for Beginners", "How to Invest in Funds", "Nasdaq Index Analysis", "Fund Recommendation", "Stock Investment Strategy", "ETF Investment Guide", "Asset Allocation Plan", "Personal Financial Planning", "Investment Book Recommendation", "Value Investing","Early Retirement","FIRE"]
---

{{< typeit 
  tag=h2
  speed=100
>}}
You Only Have to Get Rich Once
{{< /typeit >}}
## 💰&nbsp;&nbsp;Growth of $1000
{{< alert "circle-info">}}
If you invested **$1000** in **QQQ** starting from **2009/12**, and held it for **15** years, by 
**2024/12** it would be worth **$11174.43**, with a total return of **1017.44%** (annualized return of **17.46%**).
{{< /alert >}}
<br>
{{< chart >}}
    data: {'datasets': [{'type': 'line', 'label': 'Price', 'data': [1000.0, 1190.3825136612022, 1220.327868852459, 1423.606557377049, 1922.622950819672, 2256.830601092896, 2445.0273224043717, 2589.726775956284, 3404.590163934426, 3371.803278688524, 4647.213114754099, 6857.704918032787, 8696.174863387978, 5820.327868852458, 8951.256830601093, 11174.426229508197], 'yAxisID': 'price-axis', 'borderColor': 'rgb(96, 165, 250)', 'fill': 'false', 'tension': 0.4}, {'type': 'bar', 'label': 'Return', 'data': [0.0, 0.1903825136612022, 0.025156077855306616, 0.16657710908113907, 0.350529709811147, 0.17382901318781255, 0.08338983050847476, 0.05918111925621308, 0.31465226198514507, -0.009630200308166482, 0.3782574873590045, 0.47565965852970216, 0.2680882259195512, -0.3307025260776676, 0.5379299984978221, 0.24836393826919329], 'yAxisID': 'return-axis', 'backgroundColor': ['rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderColor': ['rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderRadius': 5}], 'labels': [2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024]},
    options: {
        scales: {
            'price-axis': {
                type: 'linear',
                position: 'left',
                title: {
                    display: true,
                    text: 'Price' 
                }
             },
            'return-axis': {
                type: 'linear',
                position: 'right',
                title: {
                    display: true,
                    text: 'Return'
                },
                ticks: {
                    callback: function(value, index, values) {
                        return (value * 100).toFixed(2) + '%';
                    }
                }
            }
        },
        plugins: {
            legend: {
                display: false
            },
            tooltip: {
                callbacks: {
                    label: function(context) {
                        if (context.dataset.type === 'bar') {
                            return context.dataset.label + ': ' + (context.parsed.y * 100).toFixed(2) + '%';
                        } else {
                            return context.dataset.label + ': $' + context.parsed.y.toFixed(2);
                        }
                    }
                }
            }
        }
    }
{{< /chart >}}


## 📈&nbsp;&nbsp;Market and Constituent Stocks
<div id="qqq-tradingview">
    <script>
        const container = document.getElementById('qqq-tradingview');
        const script = document.createElement('script');
        script.type = 'text/javascript';
        script.src = 'https://s3.tradingview.com/external-embedding/embed-widget-mini-symbol-overview.js';  // 加载TradingView库
        script.async = true; //  异步加载，不阻塞页面渲染
        script.textContent = `{"symbol": "NASDAQ:QQQ",
                                "width": "100%",
                                "height": "220",
                                "locale": "EN",
                                "dateRange": "60M",
                                "colorTheme": "dark",
                                "isTransparent": true,
                                "autosize": true}`;
        container.appendChild(script);  //  将 <script> 标签添加到容器中
    </script>
</div>

<br>
<div id="ndx-holdings">
    <script>
        const container_holdings = document.getElementById('ndx-holdings');
        const script_holdings = document.createElement('script');
        script_holdings.type = 'text/javascript';
        script_holdings.src = 'https://s3.tradingview.com/external-embedding/embed-widget-stock-heatmap.js';         
        script_holdings.async = true; //  异步加载，不阻塞页面渲染
        script_holdings.textContent = `{"exchanges": [],
                                        "dataSource": "NASDAQ100",
                                        "grouping": "no_group",
                                        "blockSize": "market_cap_basic",
                                        "blockColor": "change",
                                        "locale": "en",
                                        "symbolUrl": "",
                                        "colorTheme": "dark",
                                        "hasTopBar": false,
                                        "isDataSetEnabled": false,
                                        "isZoomEnabled": false,
                                        "hasSymbolTooltip": true,
                                        "isMonoSize": false,
                                        "width": "100%",
                                        "height": "350"}`;
        container_holdings.appendChild(script_holdings);  //  将 <script> 标签添加到容器中
    </script>
</div>

## 🔗&nbsp;&nbsp;Maybe you want to know more

| Website | Description |
|---|---|
| [Invesco QQQ](https://www.invesco.com/us/financial-products/etfs/product-detail?audienceType=Investor&productId=ETF-QQQ) | Official QQQ Website |
| [QQQ Holdings](https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Investor&ticker=QQQ) | QQQ Holdings List |
| [QQQ Financial Ratios](https://marketchameleon.com/Overview/QQQ/ETF-Financial-Ratios/) | Summary of QQQ Financial Ratios |
| [QQQ Historical Returns](https://www.lazyportfolioetf.com/etf/invesco-qqq-trust-qqq/) | QQQ Historical Performance from various perspectives |
| [QQQ Finance Charts](https://www.financecharts.com/etfs/QQQ/) | QQQ Finance Charts Information |
| [How to Invest in NASDAQ 100](/en/posts/1728723295012-invest-qqq/) |  NASDAQ 100 Investment Information  |

---
{{< article link="/en/posts/1736045402069/" >}}