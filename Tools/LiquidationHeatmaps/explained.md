# Liquidation heatmaps explained

A liquidation heatmap (figure 1) is a visual representation of the liquidation levels of traders in a market. It is calculated using market data and different leverage amounts. The liquidation levels are then added to price buckets on a chart. The more liquidation levels are added to a certain price, the brighter the color of the heatmap becomes, with bright yellow representing the highest amount of predicted liquidation levels. This allows traders to identify areas of high liquidity and potential price volatility.

In other words, a liquidation heatmap is a tool that helps traders identify where other traders are most likely to be liquidated. This can be useful for both long and short traders, as it can help them to avoid being liquidated themselves and to identify potential trading opportunities.

Price is likely to move towards a brighter zone of liquidations. If the liquidation zone is above the price as in figure 1 (see below) traders can expect the price to go towards that zone and could look for a long and take profit at that zone. Shorters could look at the liquidation zone and choose to take a short. In figure 2 it is visible that price immediately reversed after the liquidity was taken at the bright yellow zone.

![Figure 1: 7-Day heatmap of TIAUSD. There is a bright yellow liquidation zone above the latest spike. Price could move towards that price to liquidate shorters.](/static/TIA1.png)

![Figure 2: Price completely reversed after hitting the bright yellow liquidation zone thus presenting a perfect entry for a short trade or an exit for a previous long trade.](/static/TIA2.png)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Popup Test</title>
    <style>
        #myModal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.9);
        }

        #myModal img {
            margin: 20px;
            width: 80%;
            max-width: 800px;
        }
    </style>
</head>
<body>

    <!-- Image Popup/Modal -->
    <div id="myModal">
        <img src="" alt="Enlarged Image" id="modalImage">
    </div>

    <img src="../test/static/TIA1.png" alt="Figure 1" onclick="showModal(this.src)">
    <img src="../test/static/TIA2.png" alt="Figure 2" onclick="showModal(this.src)">

    <script>
        function showModal(imagePath) {
            var modal = document.getElementById('myModal');
            var modalImage = document.getElementById('modalImage');

            modalImage.src = imagePath;
            modal.style.display = 'block';

            modal.onclick = function () {
                modal.style.display = 'none';
            };
        }
    </script>

</body>
</html>