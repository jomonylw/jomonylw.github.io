---
title: ""
description: ""
---

{{< typeit 
  tag=h2
  speed=100
>}}
人生只需富有一次
{{< /typeit >}}

## 💰&nbsp;&nbsp;1000 美元的增长
{{< alert "circle-info">}}
如从 **2014 年 10月** 开始投资 **QQQ** **1000** 美元，持有 **10** 年，到 
**2024 年 9月** 将价值 **4813.31** 美元，总回报率为 **381.33%**（年化回报率为 **17.17%**）。
{{< /alert >}}
<br>
{{< chart >}}
    data: {'datasets': [{'type': 'line', 'label': '价格', 'data': [1018.2445759368835, 1103.1558185404338, 1168.4418145956606, 1536.0946745562128, 1521.3017751479288, 2096.7455621301774, 3094.082840236686, 3923.5700197238657, 2626.0355029585794, 4038.658777120315, 4813.313609467455], 'yAxisID': 'price-axis', 'borderColor': 'rgb(96, 165, 250)', 'fill': 'false', 'tension': 0.4}, {'type': 'bar', 'label': '收益率', 'data': [0.018244575936883507, 0.08338983050847454, 0.059181119256213166, 0.3146522619851451, -0.009630200308166414, 0.37825748735900444, 0.47565965852970216, 0.26808822591955134, -0.33070252607766754, 0.5379299984978219, 0.19180992381324474], 'yAxisID': 'return-axis', 'backgroundColor': ['rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderColor': ['rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderRadius': 5}], 'labels': [2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024]},
    options: {
        scales: {
            'price-axis': {
                type: 'linear',
                position: 'left',
                title: {
                    display: true,
                    text: '价格' 
                }
             },
            'return-axis': {
                type: 'linear',
                position: 'right',
                title: {
                    display: true,
                    text: '收益率'
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


## 📈&nbsp;&nbsp;市场及成分股
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
                                "locale": "zh_CN",
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
                                        "locale": "zh_CN",
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

## 🔗&nbsp;&nbsp;或许你想了解

| 网站 | 描述 |
|---|---|
| [Invesco QQQ](https://www.invesco.com/us/financial-products/etfs/product-detail?audienceType=Investor&productId=ETF-QQQ) | QQQ 官方网站 |
| [QQQ 持仓](https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Investor&ticker=QQQ) | QQQ 持仓列表 | 
| [QQQ 财务比率](https://marketchameleon.com/Overview/QQQ/ETF-Financial-Ratios/) | QQQ 各项财务比率数据汇总 | 
| [QQQ 历史回报](https://www.lazyportfolioetf.com/etf/invesco-qqq-trust-qqq/) | 从各维度展示QQQ历史表现 |
| [QQQ 金融图表](https://www.financecharts.com/etfs/QQQ/) | QQQ 金融图表资讯 |
| [如何投资纳斯达克 100](/posts/1728723295012-invest-qqq/) | 纳斯达克 100 投资资讯 |

