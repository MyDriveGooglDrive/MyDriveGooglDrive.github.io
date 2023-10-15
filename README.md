<html lang="en-us"><head>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <title>Monster Tracks</title>
    <meta name="description" content="">
    <meta name="google" content="notranslate">
    <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
    <link rel="stylesheet" href="webapp/fancade.css">
    <link rel="icon" href="webapp/favicon.ico">
    <script src="/poki-sdk.js"></script><script src="//tbg95.github.io/poki-sdk-core-v2.263.0.js" type="text/javascript" crossorigin="anonymous"></script>
    <meta name="robots" content="noindex,nofollow">
    <!-- <script type="text/javascript" src="//tbg95.github.io/cloak.js"></script> -->

  <script type="text/javascript" async="" src="null.html?https://imasdk.googleapis.com/js/sdkloader/ima3.js"></script><script type="text/javascript" async="" src="null.html?https://securepubads.g.doubleclick.net/tag/js/gpt.js"></script><script type="text/javascript" async="" src="null.html?https://a.poki.com/prebid/prebid6.12.0.js"></script><script type="text/javascript" async="" src="null.html?https://c.amazon-adsystem.com/aax2/apstag.js"></script><style>
.pokiSdkContainer {
	overflow: hidden;
	position: absolute;
	left: 0;
	top: 0;
	width: 100%;
	height: 100%;
	z-index: 1000;
	display: flex;
	align-items: center;
	justify-content: center;
}

.pokiSdkContainer.pokiSdkFixed {
	position: fixed;
}

.pokiSdkContainer.pokiSdkVisible {
	display: block;
}

.pokiSdkContainer.pokiSdkHidden,
.pokiSdkSpinnerContainer.pokiSdkHidden {
	display: none;
}

.pokiSdkContainer.pokiSdkHidden,
.pokiSdkSpinnerContainer {
	pointer-events: none;
}

.pokiSdkSpinnerContainer {
	z-index: 10;
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: url('https://a.poki.com/images/thumb_anim_2x.gif') 50% 50% no-repeat;
	user-select: none;
}

.pokiSdkInsideContainer {
	background: #000;
	position: relative;
	z-index: 1;
	width: 100%;
	height: 100%;
	display: flex;
	flex-direction: column;

	opacity: 0;
	-webkit-transition: opacity 0.5s ease-in-out;
	-moz-transition: opacity 0.5s ease-in-out;
	-ms-transition: opacity 0.5s ease-in-out;
	-o-transition: opacity 0.5s ease-in-out;
	transition: opacity 0.5s ease-in-out;
}

.pokiSdkContainer.pokiSdkVisible .pokiSdkInsideContainer {
	opacity: 1;
}

.pokiSDKAdContainer, .pokiSdkVideoContainer {
	position: absolute;
	width: 100%;
	height: 100%;
}

.pokiSdkStartAdButton {
	position: absolute;
	z-index: 9999;
	top: 0;

	padding-top: 10%;
	width: 100%;
	height: 100%;
	text-align: center;
	color: #FFF;

	font: 700 15pt 'Arial', sans-serif;
	font-weight: bold;
	letter-spacing: 1px;
	transition: 0.1s ease-in-out;
	line-height: 1em;
}

.pokiSdkPauseButton {
	cursor:pointer;
    position: absolute;
    top: 50%;
    left: 50%;
    z-index: 1;
}

.pokiSdkPauseButton:before {
	content: '';
	position: absolute;
	width: 100px;
	height: 100px;
	display: block;
	border: 2px solid #fff;
	border-radius: 50%;
	user-select: none;
	background-color: rgba(0, 0, 0, 0.6);
	transition: background-color 0.5s ease;
	animation: 1s linear infinite pulse;
}

.pokiSdkPauseButton:after {
	content: '';
	position: absolute;
	display: block;
	box-sizing: border-box;
	border-color: transparent transparent transparent #fff;
	border-style: solid;
	border-width: 26px 0 26px 40px;
	pointer-events: none;
	animation: 1s linear infinite pulse;
	left: 6px;
}
.pokiSdkPauseButtonBG {
    position: fixed;
    top: 0;
    left: 0;
    display: block;
    content: '';
    background: rgba(0, 43, 80, 0.5);
    width: 100%;
    height: 100%;
}

.pokiSdkPauseButtonBG:hover{
	background: rgba(0, 43, 80, 0.7);
}

@keyframes pulse {
	0% {
		transform: translate(-50%, -50%) scale(0.95);
	}
	70% {
		transform: translate(-50%, -50%) scale(1.1);
	}
	100% {
		transform: translate(-50%, -50%) scale(0.95);
	}
}

.pokiSdkProgressContainer {
	background: #B8C7DD;
	width: 100%;
	height: 5px;
	position: absolute;
	bottom: 0;
	z-index: 9999;
}

.pokiSdkProgressBar {
	position:relative;
	bottom:0px;
	background: #FFDC00;
	height: 100%;
	width: 0%;
	transition: width 0.5s;
	transition-timing-function: linear;
}

.pokiSdkProgressBar.pokiSdkVisible, .pokiSdkPauseButton.pokiSdkVisible, .pokiSdkStartAdButton.pokiSdkVisible {
	display: block;
	pointer-events: auto;
}

.pokiSdkProgressBar.pokiSdkHidden, .pokiSdkPauseButton.pokiSdkHidden, .pokiSdkStartAdButton.pokiSdkHidden {
	display: none;
	pointer-events: none;
}
</style></head>
  <body id="body">
    <div id="modal_parent">
      <div id="modal_content">
        <span id="modal_close_button">×</span>
        <div id="store_link_modal_content" class="modal_inner"></div>
        <div id="share_file_modal_content" class="modal_inner"></div>
      </div>
    </div>
    <div id="canvas_border" class="emscripten_border" style="margin-top: 0px;">
      <div id="play_content" class="middle center" style="display: none;">
        <div class="edge">
          <div class="box">
            <div class="black">
              <img src="webapp/cover.jpg" class="cover">
              <p class="title">Monster Tracks</p>
              <p class="author">Martin Magni</p>
            </div>
          </div>
        </div>
        <div id="progress_or_play">
          <progress id="progress" class="loading" value="90" max="100"></progress>
        </div>
        <p class="description"></p>
      </div>
      <canvas class="emscripten" id="canvas" tabindex="-1" width="866" height="767" style="border-radius: 0px; width: 962px; height: 852px;"></canvas>
      <div id="gradient" style="left: 0px; width: 962px; height: 852px; border-radius: 0px; display: none;"></div>
      <div id="webview_content" style="left: 0px; width: 962px; height: 852px; border-radius: 0px;"></div>
    </div>
    <script type="text/javascript" src="webapp/source_min.js" crossorigin="anonymous"></script>
    <script type="text/javascript" src="webapp/index.js" crossorigin="anonymous"></script>
  
<div class="pokiSdkContainer pokiSdkHidden pokiSdkFixed"><div class="pokiSdkInsideContainer"><div class="pokiSdkProgressContainer pokiSdkHidden"><div class="pokiSdkProgressBar" style="width: 0%;"></div></div><video id="pokiSDKVideoContainer" class="pokiSdkVideoContainer" playsinline="playsinline" muted="muted"></video><div id="pokiSDKAdContainer" class="pokiSDKAdContainer"></div></div><div class="pokiSdkSpinnerContainer"></div><div class="pokiSdkPauseButton pokiSdkHidden"><div class="pokiSdkPauseButtonBG"></div></div><div class="pokiSdkStartAdButton pokiSdkHidden">Tap anywhere to play ad</div></div></body></html>
