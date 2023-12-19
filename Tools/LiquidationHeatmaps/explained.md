# Liquidation heatmaps explained

A liquidation heatmap (figure 1) is a visual representation of the liquidation levels of traders in a market. It is calculated using market data and different leverage amounts. The liquidation levels are then added to price buckets on a chart. The more liquidation levels are added to a certain price, the brighter the color of the heatmap becomes, with bright yellow representing the highest amount of predicted liquidation levels. This allows traders to identify areas of high liquidity and potential price volatility.

In other words, a liquidation heatmap is a tool that helps traders identify where other traders are most likely to be liquidated. This can be useful for both long and short traders, as it can help them to avoid being liquidated themselves and to identify potential trading opportunities.

Price is likely to move towards a brighter zone of liquidations. If the liquidation zone is above the price as in figure 1 (see below) traders can expect the price to go towards that zone and could look for a long and take profit at that zone. Shorters could look at the liquidation zone and choose to take a short. In figure 2 it is visible that price immediately reversed after the liquidity was taken at the bright yellow zone.

<style>
	.modal {
		position: fixed;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		z-index: 1050;
		display: none;
		overflow: hidden;
		outline: 0;
	}
	.modal-dialog {
		position: relative;
		width: auto;
		margin: 10px;
		padding: 6% 10%;
	}
	.modal-content {
		position: relative;
		background-color: #fff;
		border: 1px solid #999;
		border: 1px solid rgba(0,0,0,.2);
		border-radius: 6px;
		outline: 0;
		box-shadow: 0 3px 9px rgba(0,0,0,.5);
	}
	.modal-header {
		padding: 15px;
		border-bottom: 1px solid #e5e5e5;
	}
	.modal-body {
		position: relative;
		padding: 15px;
	}
	.close {
		float: right;
		font-size: 1.5rem;
		font-weight: 700;
		line-height: 0;
		color: #000;
		text-shadow: 0 1px 0 #fff;
		opacity: .5;
	}
	.close:hover, .close:focus {
		color: #000;
		text-decoration: none;
		opacity: .75;
	}
</style>

<figure class="content-center">
	<img src="/static/TIA1.png" data-toggle="modal" data-target="#myModal1"/>
</figure>

<div class="modal" id="myModal1">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal">&times;</button>
			</div>
			<div class="modal-body">
				<img src="/static/TIA1.png" style="width:100%"/>
			</div>
		</div>
	</div>
</div>

![Figure 1: 7-Day heatmap of TIAUSD. There is a bright yellow liquidation zone above the latest spike. Price could move towards that price to liquidate shorters.]

<figure class="content-center">
	<img src="/static/TIA2.png" data-toggle="modal" data-target="#myModal2"/>
</figure>

<div class="modal" id="myModal2">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal">&times;</button>
			</div>
			<div class="modal-body">
				<img src="/static/TIA2.png" style="width:100%"/>
			</div>
		</div>
	</div>
</div>

![Figure 2: Price completely reversed after hitting the bright yellow liquidation zone thus presenting a perfect entry for a short trade or an exit for a previous long trade.]


<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>