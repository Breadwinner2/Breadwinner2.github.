# Breadwinner2.github.
	text-decoration: none;
}

#gameOver h2{
#gameOver h3{
	color:orange;
}

 3  dist/tetris.js 
@@ -178,8 +178,11 @@ var gridLineColor = 'rgba(255,255,255,0.2)';
var boxBorderColor = 'rgba(255,255,255,0.5)';


// Game speed
var defaultInterval = 600;


// Level update interval 
var levelInterval = 120 * 1000; 


 4  index.html 
@@ -14,8 +14,8 @@
	<canvas id="scene"></canvas>
	<div id="gameOver">
		<h1>Game Over !</h1>
		<h2>Score: <span id="finalScore">0</span></h2>
		<h3><a href="#" id="restart">Restart</a></h2>
		<h3>Score: <span id="finalScore">0</span></h3>
		<h2><a href="#" id="restart">Restart</a></h2>

	</div>
	<div id="side">
 3  src/consts.js 
@@ -26,8 +26,11 @@ var gridLineColor = 'rgba(255,255,255,0.2)';
var boxBorderColor = 'rgba(255,255,255,0.5)';


// Game speed
var defaultInterval = 600;


// Level update interval 
var levelInterval = 120 * 1000; 


var exports = module.exports = {};
exports.COLORS =  colors;
exports.SIDE_WIDTH = sideWidth;
exports.ROW_COUNT = rowCount;
exports.COLUMN_COUNT = columnCount;
exports.SCENE_BG_START = sceneBgStart;
exports.SCENE_BG_END = sceneBgEnd;
exports.PREVIEW_BG = previewBg;
exports.PREVIEW_COUNT = previewCount;
exports.GRID_LINE_COLOR = gridLineColor;
