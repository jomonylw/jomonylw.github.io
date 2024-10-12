---
title: ""
description: ""
---

{{< typeit 
  tag=h2
  speed=100
>}}
You Only Have to Get Rich Once
{{< /typeit >}}
## 💰&nbsp;&nbsp;Growth of $1
{{< alert "circle-info">}}
An investment of **$1** in **QQQ** starting in **October 2004** would be worth **$13.68** by **October 2024**, representing a total return of **1268.00%** (annualized return of **13.94%**).

{{< /alert >}}
<br>
{{< chart >}}
type: 'line',
data: {
    labels: ['2004/10', '2005/04', '2005/10', '2006/04', '2006/10', '2007/04', '2007/10', '2008/04', '2008/10', '2009/04', '2009/10', '2010/04', '2010/10', '2011/04', '2011/10', '2012/04', '2012/10', '2013/04', '2013/10', '2014/04', '2014/10', '2015/04', '2015/10', '2016/04', '2016/10', '2017/04', '2017/10', '2018/04', '2018/10', '2019/04', '2019/10', '2020/04', '2020/10', '2021/04', '2021/10', '2022/04', '2022/10', '2023/04', '2023/10', '2024/04', '2024/10'],
    datasets: [{
        label: '$',
        data: [1.04, 0.98, 1.08, 1.17, 1.18, 1.31, 1.51, 1.32, 0.92, 0.95, 1.15, 1.38, 1.46, 1.66, 1.65, 1.89, 1.83, 1.95, 2.33, 2.42, 2.85, 3.10, 3.18, 2.97, 3.29, 3.82, 4.24, 4.55, 4.68, 5.35, 5.49, 6.00, 7.56, 9.49, 10.84, 8.79, 7.89, 9.05, 9.69, 12.10, 13.68],
        borderColor: 'rgb(75, 192, 192)',
        tension: 0.1,
    }],
},
options: {
    plugins: {
        legend: {
            display: false
        }
    }
}
{{< /chart >}}

---
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

## 🔗&nbsp;&nbsp;Maybe you want to know more

| Website | Description |
|---|---|
| [Invesco QQQ](https://www.invesco.com/us/financial-products/etfs/product-detail?audienceType=Investor&productId=ETF-QQQ) | Official QQQ Website |
| [QQQ Holdings](https://www.invesco.com/us/financial-products/etfs/holdings?audienceType=Investor&ticker=QQQ) | QQQ Holdings List |
| [QQQ Financial Ratios](https://marketchameleon.com/Overview/QQQ/ETF-Financial-Ratios/) | Summary of QQQ Financial Ratios |
| [QQQ Historical Returns](https://www.lazyportfolioetf.com/etf/invesco-qqq-trust-qqq/) | QQQ Historical Performance from various perspectives |
| [QQQ Finance Charts](https://www.financecharts.com/etfs/QQQ/) | QQQ Finance Charts Information |
| [How to Invest in QQQ](/en/posts/1728723295012-invest-qqq/) | QQQ Investment Information  |

