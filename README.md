<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<!--1、强制让页面的宽度与设备的宽度保持1:1-->
	<meta name ="viewport" content ="width=device-width initial-scale=1, maximum-scale=1, minimum-scale=1, user-scalable=no">
	<!--2、iphone设备中的safari私有meta标签，它表示：允许全屏模式浏览-->
	<meta name="apple-mobile-web-app-capable" content="yes"/>
	<!--3、iphone的私有标签，它指定的iphone中safari顶端的状态条的样式-->
	<meta name="apple-mobile-web-app-status-bar-style" content="black"/>
	<!--4、禁止ios设备,识别电话号码-->
	<meta name="format-detection" content="telephone=no" />
	<title>投保资料上传</title>
	<link href="./css/mui.min.css" rel="stylesheet"/>
    <link rel="stylesheet" type="text/css" href="./css/mui.picker.min.css" />
	<link href="./css/mui.poppicker.css" rel="stylesheet" />
	<link rel="stylesheet" href="./css/common.css">
	<link rel="stylesheet" href="./css/dataUpload.css">
</head>
<body>
	<div class="header">
		<p id="company">永达理保险经纪有限公司 </p>
		<p id="fwzy">服务专员：小勇 1334567895</p>
	</div>
	<div class="prompt">
		<i class="iconfont">&#xe602;</i>投保资料上传
	</div>
	<div class="datum">
		<p>投保人身份证件正、背面上传（必传）</p>
		<ul class="cards clearfix">
			<li>
				<div>
					<img src="images/idcardz.jpg" alt=""><i class="iconfont">&#xe604;</i>
				</div>
			</li>
			<li>
				<div>
					<img src="images/idcardf.jpg" alt=""><i class="iconfont">&#xe604;</i>
				</div>
			</li>
		</ul>
	</div>
	<div class="datum">
		<p>被保险人身份证件正、背面上传（必传）</p>
		<div></div>
	</div>
	<div class="datum">
		<p>受益人身份证件正、背面上传（必传）</p>
		<div></div>
	</div>
	<div class="datum">
		<p>投保人银行卡正面上传（必传）</p>
		<div></div>
	</div>
	<div class="datum datum-last">
		<p>其他资料上传</p>
		<div></div>
	</div>
	<p class="warning">提示：依据公司《反洗钱管理办法》客户身份识别规定，如果以转账形式累计应交保险费超过20万元（或以现金形式累计应交保险费超过2万元），请提供投保人与被保人关系证明资料。</p>
	<div class="prompt">
		<i class="iconfont">&#xe613;</i>签名
	</div>
	<div class="datum">
		<p class="autograph">投保人签名</p>
		<div class="qianm-a">
			<div class="qianm-b">
				<img class="qianm" src="images/mou_03.png" alt="">
				<i class="iconfont">&#xe604;</i>
			</div>
		</div>
	</div>
	<div class="datum datum-last">
		<p>被保险人或其法定监护人签名</p>
		<div></div>
	</div>
	<p class="warning">提示：如果被保险人小于18周岁，须其法定监护人签字。</p>
	<div class="clause">
		<div class="clause-a">
		<div class="clause-xz">
			<div class="mui-input-row mui-checkbox mui-left demand">
			<label class="lables"></label>
			  	<input name="checkbox1" value="Item 1" type="checkbox">
			</div>
		</div>本人已阅读<a href="clauses.html">《保险条款》</a>、<a href="">《产品说明书》</a>、<a href="tipbook.html">《投保提示书》</a>并确认<a href="javascript:;">录入以下风险提示语</a>，已充分理解保险责任、责任免除、保障范围、退保等条款，且同意遵守。
		</div>
		<div class="reminder">
		<p class="reminder-a">本人已阅读保险条款、产品说明书和投保提示
书，了解本产品的特点和保单利益的不确定性</p>
<textarea name="" id="" class="reminder-b" placeholder="请正确录入以上风险提示语（包含标点符号）"></textarea>
		</div>
	</div>
	<p class="warning">提示：由于条款等内容较大，建议在WIFI环境下打开</p>
	<div class="btn-group">
	<button class="pre-btn btn-witer">上一步</button>
	<button class="next-btn btn-red">下一步</button></div>
	<div class="footer">
		<p>华夏保险 版权所有</p>
	</div>
	<iframe class="board" name="ifm" src ="./sign.html" width="100%" frameborder="0"></iframe>
</body>
<script src="./js/jquery-1.11.3.min.js"></script>
<script src="./js/flexible.js"></script>
<script src="./js/bootstrap.min.js"></script>
<script src="./js/mui.min.js"></script>
<script src="./js/mui.picker.min.js"></script>
<script src="./js/mui.poppicker.js"></script>
<script src="./js/city.data.js" type="text/javascript" charset="utf-8"></script>
<script src="./js/city.data-3.js" type="text/javascript" charset="utf-8"></script>
<script>
	$(function(){
		$(".autograph").click(function(){
			$(".board").css("height","100%");
			$("body").css("overflow-y","hidden");
		})
	})
</script>
</html>
