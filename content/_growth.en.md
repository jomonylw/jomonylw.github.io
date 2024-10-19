## 💰&nbsp;&nbsp;Growth of $1000
{{< alert "circle-info">}}
If you invested **$1000** in **QQQ** starting from **2009/09**, and held it for **15** years, by 
**2024/09** it would be worth **$11551.95**, with a total return of **1055.20%** (annualized return of **17.72%**).
{{< /alert >}}
<br>
{{< chart >}}
    data: {'datasets': [{'type': 'line', 'label': 'Price', 'data': [1082.8402366863904, 1288.9940828402366, 1321.4201183431953, 1541.5384615384614, 2081.8934911242604, 2443.786982248521, 2647.5739644970413, 2804.2603550295858, 3686.627218934911, 3651.1242603550295, 5032.1893491124265, 7425.798816568047, 9416.56804733728, 6302.485207100591, 9692.781065088757, 11551.952662721893], 'yAxisID': 'price-axis', 'borderColor': 'rgb(96, 165, 250)', 'fill': 'false', 'tension': 0.4}, {'type': 'bar', 'label': 'Return', 'data': [0.08284023668639043, 0.19038251366120224, 0.02515607785530675, 0.16657710908113904, 0.35052970981114706, 0.1738290131878127, 0.08338983050847446, 0.05918111925621316, 0.3146522619851451, -0.009630200308166388, 0.37825748735900444, 0.4756596585297021, 0.26808822591955145, -0.33070252607766765, 0.537929998497822, 0.1918099238132448], 'yAxisID': 'return-axis', 'backgroundColor': ['rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderColor': ['rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(255, 99, 132, 0.5)'], 'borderRadius': 5}], 'labels': [2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024]},
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
