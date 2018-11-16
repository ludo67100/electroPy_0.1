# electroPy_0.1
Updated version of ElectroPy with scalogram 
<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<title>Scalogram</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>

<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.2.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.2.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.2.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.2.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.2.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.2.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2);
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1);
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1);
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
@media (max-width: 991px) {
  #ipython_notebook {
    margin-left: 10px;
  }
}
[dir="rtl"] #ipython_notebook {
  float: right !important;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#login_widget {
  float: right;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  text-align: center;
  vertical-align: middle;
  display: inline;
  opacity: 0;
  z-index: 2;
  width: 12ex;
  margin-right: -12ex;
}
.alternate_upload .btn-upload {
  height: 22px;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
[dir="rtl"] #tabs li {
  float: right;
}
ul#tabs {
  margin-bottom: 4px;
}
[dir="rtl"] ul#tabs {
  margin-right: 0px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons {
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-right {
  padding-top: 1px;
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-left {
  float: right !important;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: baseline;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
#tree-selector {
  padding-right: 0px;
}
[dir="rtl"] #tree-selector a {
  float: right;
}
#button-select-all {
  min-width: 50px;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
[dir="rtl"] #new-menu {
  text-align: right;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
[dir="rtl"] #running .col-sm-8 {
  float: right !important;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI colors. */
.ansibold {
  font-weight: bold;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  border-left-width: 1px;
  padding-left: 5px;
  background: linear-gradient(to right, transparent -40px, transparent 1px, transparent 1px, transparent 100%);
}
div.cell.jupyter-soft-selected {
  border-left-color: #90CAF9;
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected {
  border-color: #ababab;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 5px, transparent 5px, transparent 100%);
}
@media print {
  div.cell.selected {
    border-color: transparent;
  }
}
div.cell.selected.jupyter-soft-selected {
  border-left-width: 0;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 7px, #E3F2FD 7px, #E3F2FD 100%);
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #66BB6A -40px, #66BB6A 5px, transparent 5px, transparent 100%);
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  padding: 0.4em;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. We need the 0 value because of how we size */
  /* .CodeMirror-lines */
  padding: 0;
  border: 0;
  border-radius: 0;
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul {
  list-style: disc;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ul ul {
  list-style: square;
  margin: 0em 2em;
}
.rendered_html ul ul ul {
  list-style: circle;
  margin: 0em 2em;
}
.rendered_html ol {
  list-style: decimal;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
  margin: 0em 2em;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  background-color: #fff;
  color: #000;
  font-size: 100%;
  padding: 0px;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: 1px solid black;
  border-collapse: collapse;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  border: 1px solid black;
  border-collapse: collapse;
  margin: 1em 2em;
}
.rendered_html td,
.rendered_html th {
  text-align: left;
  vertical-align: middle;
  padding: 4px;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget {
  float: right !important;
  float: right;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  margin-top: 6px;
}
span.save_widget span.filename {
  height: 1em;
  line-height: 1em;
  padding: 3px;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  display: none;
}
.command-shortcut:before {
  content: "(command)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    
/* Temporary definitions which will become obsolete with Notebook release 5.0 */
.ansi-black-fg { color: #3E424D; }
.ansi-black-bg { background-color: #3E424D; }
.ansi-black-intense-fg { color: #282C36; }
.ansi-black-intense-bg { background-color: #282C36; }
.ansi-red-fg { color: #E75C58; }
.ansi-red-bg { background-color: #E75C58; }
.ansi-red-intense-fg { color: #B22B31; }
.ansi-red-intense-bg { background-color: #B22B31; }
.ansi-green-fg { color: #00A250; }
.ansi-green-bg { background-color: #00A250; }
.ansi-green-intense-fg { color: #007427; }
.ansi-green-intense-bg { background-color: #007427; }
.ansi-yellow-fg { color: #DDB62B; }
.ansi-yellow-bg { background-color: #DDB62B; }
.ansi-yellow-intense-fg { color: #B27D12; }
.ansi-yellow-intense-bg { background-color: #B27D12; }
.ansi-blue-fg { color: #208FFB; }
.ansi-blue-bg { background-color: #208FFB; }
.ansi-blue-intense-fg { color: #0065CA; }
.ansi-blue-intense-bg { background-color: #0065CA; }
.ansi-magenta-fg { color: #D160C4; }
.ansi-magenta-bg { background-color: #D160C4; }
.ansi-magenta-intense-fg { color: #A03196; }
.ansi-magenta-intense-bg { background-color: #A03196; }
.ansi-cyan-fg { color: #60C6C8; }
.ansi-cyan-bg { background-color: #60C6C8; }
.ansi-cyan-intense-fg { color: #258F8F; }
.ansi-cyan-intense-bg { background-color: #258F8F; }
.ansi-white-fg { color: #C5C1B4; }
.ansi-white-bg { background-color: #C5C1B4; }
.ansi-white-intense-fg { color: #A1A6B2; }
.ansi-white-intense-bg { background-color: #A1A6B2; }

.ansi-bold { font-weight: bold; }

    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#First import all what we need from electroPy</span>
<span class="kn">from</span> <span class="nn">electroPy</span> <span class="k">import</span> <span class="n">HdF5IO</span><span class="p">,</span> <span class="n">AnalogSignal</span><span class="p">,</span> <span class="n">TimeFreq</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[&nbsp;]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">path</span> <span class="o">=</span> <span class="s1">&#39;C:/Users/ludov/Documents/2018-08-10T13-54-41McsRecording.h5&#39;</span>

<span class="c1">#Open the .h5 file</span>
<span class="n">my_file</span> <span class="o">=</span> <span class="n">HdF5IO</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>

<span class="c1">#Get the data for computation, i.e. on the first channel</span>
<span class="n">ch_0</span> <span class="o">=</span> <span class="n">my_file</span><span class="o">.</span><span class="n">raw_record</span><span class="p">()[</span><span class="mi">0</span><span class="p">]</span>

<span class="c1">#We also need the the time vector</span>
<span class="n">time_vector</span> <span class="o">=</span> <span class="n">my_file</span><span class="o">.</span><span class="n">raw_time</span><span class="p">()</span>

<span class="c1">#And the sampling rate</span>
<span class="n">sampling_rate</span> <span class="o">=</span> <span class="n">my_file</span><span class="o">.</span><span class="n">raw_sampling_rate</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Let&#39;s plot the data just for fun </span>
<span class="kn">from</span> <span class="nn">matplotlib</span> <span class="k">import</span> <span class="n">pyplot</span> <span class="k">as</span> <span class="n">plt</span>

<span class="n">fig1</span> <span class="o">=</span><span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">()</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">time_vector</span><span class="p">,</span><span class="n">ch_0</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Time (s)&#39;</span><span class="p">);</span> <span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Amplitude (V)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Now we need to convert our .h5 data in AnalogSignal</span>
<span class="c1">#&#39;Cause the morlet/fft/scalo method can only hanlde this kind of object</span>
<span class="c1">#The minimum to fill are the signal, the time vector and the sampling rate</span>

<span class="n">anasig</span> <span class="o">=</span> <span class="n">AnalogSignal</span><span class="p">(</span><span class="n">signal</span><span class="o">=</span><span class="n">ch_0</span><span class="p">,</span><span class="n">time_vector</span><span class="o">=</span><span class="n">time_vector</span><span class="p">,</span>
                      <span class="n">sampling_rate</span><span class="o">=</span><span class="n">sampling_rate</span><span class="p">)</span>

<span class="c1">#Let&#39;s plot it to see, it should look exactly like above</span>
<span class="n">fig2</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">()</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">anasig</span><span class="o">.</span><span class="n">t</span><span class="p">(),</span><span class="n">anasig</span><span class="o">.</span><span class="n">signal</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Time (s)&#39;</span><span class="p">);</span> <span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Amplitude (V)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Now we can go the the scalogram </span>
<span class="c1">#Here u should fill the following parameters, f_start &amp; f_stop delimit the freq range for computation </span>
<span class="c1">#Deltafreq has a binning effect, a high delta implies low spectral resolution but faster computation...</span>
<span class="n">scalo</span> <span class="o">=</span> <span class="n">TimeFreq</span><span class="p">(</span><span class="n">anasig</span><span class="p">,</span>
                 <span class="n">f_start</span><span class="o">=</span><span class="mi">5</span><span class="p">,</span>
                 <span class="n">f_stop</span><span class="o">=</span><span class="mi">20</span><span class="p">,</span>
                 <span class="n">deltafreq</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span>
                 <span class="n">sampling_rate</span><span class="o">=</span><span class="n">sampling_rate</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Then we should plot it ! </span>
<span class="kn">from</span> <span class="nn">matplotlib</span> <span class="k">import</span> <span class="n">pyplot</span> <span class="k">as</span> <span class="n">plt</span>

<span class="n">fig3</span><span class="p">,</span> <span class="n">ax</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span><span class="mi">1</span><span class="p">)</span>

<span class="n">scalo</span><span class="o">.</span><span class="n">plotMap</span><span class="p">(</span><span class="n">ax</span><span class="p">)</span>

<span class="n">ax</span><span class="o">.</span><span class="n">set_xlabel</span><span class="p">(</span><span class="s1">&#39;Time (s)&#39;</span><span class="p">)</span>
<span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="s1">&#39;Frequency (Hz)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>

<span class="c1">#Tadaaaaaaaaaaaaaaaaaaaaaaaaaaaaa</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>
