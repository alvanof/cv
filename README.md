<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html b:version='2' class='v2' expr:dir='data:blog.languageDirection' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <meta content='width=device-width, initial-scale=1, maximum-scale=1' name='viewport'/>
    <b:include data='blog' name='all-head-content'/>

    <title>
      <b:if cond='data:blog.pageType == &quot;index&quot;'>
        <data:blog.pageTitle/>
        <b:else/>
        <b:if cond='data:blog.pageType != &quot;error_page&quot;'>
          <data:blog.pageName/> - <data:blog.title/>
          <b:else/>
          ERROR 404 - <data:blog.title/> 
        </b:if>
      </b:if>
    </title>

    <!-- Description and Keywords -->
    <b:if cond='data:blog.pageType == &quot;index&quot;'>
      <meta content='YOUR DESCRIPTION HERE' name='description'/>
    </b:if>
    <meta content='YOUR KEYWORDS HERE' name='keywords'/>
    <b:if cond='data:blog.pageType == &quot;item&quot;'>
      <meta expr:content='data:blog.pageName' property='og:title'/>
      <meta expr:content='data:blog.canonicalUrl' property='og:url'/>
      <meta content='article' property='og:type'/>
    </b:if>
    <b:if cond='data:blog.postImageUrl'>
      <meta expr:content='data:blog.postImageUrl' property='og:image'/>
      <b:else/>
      <b:if cond='data:blog.postImageThumbnailUrl'>
        <meta expr:content='data:blog.postImageThumbnailUrl' property='og:image'/>
      </b:if></b:if>
    <b:if cond='data:blog.metaDescription != &quot;&quot;'>
      <meta expr:content='data:blog.metaDescription' name='og:description'/>
    </b:if>
    <meta expr:content='data:blog.title' property='og:site_name'/>
    <meta expr:content='data:blog.homepageUrl' name='twitter:domain'/>
    <meta expr:content='data:blog.pageName' name='twitter:title'/>
    <b:if cond='data:blog.postImageUrl'>
      <meta content='summary_large_image' name='twitter:card'/>
      <meta expr:content='data:blog.postImageUrl' name='twitter:image'/>
      <b:else/>
      <meta content='summary' name='twitter:card'/>
      <b:if cond='data:blog.postImageThumbnailUrl'>
        <meta expr:content='data:blog.postImageThumbnailUrl' name='twitter:image'/> 
      </b:if>
    </b:if>
    <meta expr:content='data:blog.pageName' name='twitter:title'/>
    <b:if cond='data:blog.metaDescription'>
      <meta expr:content='data:blog.metaDescription' name='twitter:description'/>
    </b:if>

    <!-- Links -->
    <link href='https://maxcdn.bootstrapcdn.com/font-awesome/4.6.1/css/font-awesome.min.css' rel='stylesheet'/>
    <link href='https://cdn.linearicons.com/free/1.0.0/icon-font.min.css' rel='stylesheet'/>
    <link href='//fonts.googleapis.com/css?family=Open+Sans:300,300i,400,400i,600,600i,700,700i,800,800i' rel='stylesheet'/>
    <link href='http://fonts.googleapis.com/css?family=Raleway:400,600' rel='stylesheet' type='text/css'/>
    <script src='http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js' type='text/javascript'/>
    <!-- Links END-->

&lt;style type=&quot;text/css&quot;&gt;&lt;!-- /* 
    <b:skin><![CDATA[/*
//////////////////////////////////////////////////////////////
//                                                         //
//  Theme Name : Storm                                    //
//  Author : Themeswear								     //
//  Site :www.Themeswear.com                            //
//  License : Creative Commons Attribution License	   //
//  Share and Use This With Proper Credit.            //
//                                                   //
//////////////////////////////////////////////////////
*/
/*-------------------------------------------*/
/*  1. Bootstrap
/*-------------------------------------------*/
html{font-family:sans-serif;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{margin:.67em 0;font-size:2em}mark{color:#000;background:#ff0}small{font-size:80%}sub,sup{position:relative;font-size:75%;line-height:0;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{height:0;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{margin:0;font:inherit;color:inherit}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{padding:0;border:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;-webkit-appearance:textfield}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{padding:.35em .625em .75em;margin:0 2px;border:1px solid silver}legend{padding:0;border:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-spacing:0;border-collapse:collapse}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="javascript:"]:after,a[href^="#"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:'Glyphicons Halflings';src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format('embedded-opentype'),url(../fonts/glyphicons-halflings-regular.woff2) format('woff2'),url(../fonts/glyphicons-halflings-regular.woff) format('woff'),url(../fonts/glyphicons-halflings-regular.ttf) format('truetype'),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format('svg')}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{display:inline-block;max-width:100%;height:auto;padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;margin-left:-5px;list-style:none}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;overflow:hidden;clear:left;text-align:right;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help;border-bottom:1px dotted #777}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:'\2014 \00A0'}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:''}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:'\00A0 \2014'}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=file]:focus,input[type=checkbox]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}input[type=search]{-webkit-appearance:none}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=time].form-control,input[type=datetime-local].form-control,input[type=month].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=time],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],input[type=date].input-sm,input[type=time].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=time],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],input[type=date].input-lg,input[type=time].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;padding:6px 12px;margin-bottom:0;font-size:14px;font-weight:400;line-height:1.42857143;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-image:none;border:1px solid transparent;border-radius:4px}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);-webkit-box-shadow:none;box-shadow:none;opacity:.65}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{background-image:none}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{background-image:none}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{background-image:none}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{background-image:none}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{background-image:none}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{background-image:none}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;-webkit-overflow-scrolling:touch;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1)}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-top:8px;margin-right:15px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-top:8px;margin-right:-15px;margin-bottom:8px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1)}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{-webkit-appearance:none;padding:0;cursor:pointer;background:0 0;border:0}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out;-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%)}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;outline:0;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5)}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:12px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;filter:alpha(opacity=0);opacity:0;line-break:auto}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2);line-break:auto}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow{border-width:11px}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{left:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{left:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{left:0;-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;filter:alpha(opacity=90);outline:0;opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:'\2039'}.carousel-control .icon-next:before{content:'\203a'}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
/*# sourceMappingURL=bootstrap.min.css.map */
/*-------------------------------------------*/
/*  2. Animation
/*-------------------------------------------*/
.animated{-webkit-animation-duration:1s;animation-duration:1s;-webkit-animation-fill-mode:both;animation-fill-mode:both}.animated.infinite{-webkit-animation-iteration-count:infinite;animation-iteration-count:infinite}.animated.hinge{-webkit-animation-duration:2s;animation-duration:2s}.animated.flipOutX,.animated.flipOutY,.animated.bounceIn,.animated.bounceOut{-webkit-animation-duration:.75s;animation-duration:.75s}@-webkit-keyframes bounce{from,20%,53%,80%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}40%,43%{-webkit-animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);-webkit-transform:translate3d(0,-30px,0);transform:translate3d(0,-30px,0)}70%{-webkit-animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);-webkit-transform:translate3d(0,-15px,0);transform:translate3d(0,-15px,0)}90%{-webkit-transform:translate3d(0,-4px,0);transform:translate3d(0,-4px,0)}}@keyframes bounce{from,20%,53%,80%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}40%,43%{-webkit-animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);-webkit-transform:translate3d(0,-30px,0);transform:translate3d(0,-30px,0)}70%{-webkit-animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);animation-timing-function:cubic-bezier(0.755,0.050,0.855,0.060);-webkit-transform:translate3d(0,-15px,0);transform:translate3d(0,-15px,0)}90%{-webkit-transform:translate3d(0,-4px,0);transform:translate3d(0,-4px,0)}}.bounce{-webkit-animation-name:bounce;animation-name:bounce;-webkit-transform-origin:center bottom;transform-origin:center bottom}@-webkit-keyframes flash{from,50%,to{opacity:1}25%,75%{opacity:0}}@keyframes flash{from,50%,to{opacity:1}25%,75%{opacity:0}}.flash{-webkit-animation-name:flash;animation-name:flash}@-webkit-keyframes pulse{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}50%{-webkit-transform:scale3d(1.05,1.05,1.05);transform:scale3d(1.05,1.05,1.05)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}@keyframes pulse{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}50%{-webkit-transform:scale3d(1.05,1.05,1.05);transform:scale3d(1.05,1.05,1.05)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}.pulse{-webkit-animation-name:pulse;animation-name:pulse}@-webkit-keyframes rubberBand{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}30%{-webkit-transform:scale3d(1.25,0.75,1);transform:scale3d(1.25,0.75,1)}40%{-webkit-transform:scale3d(0.75,1.25,1);transform:scale3d(0.75,1.25,1)}50%{-webkit-transform:scale3d(1.15,0.85,1);transform:scale3d(1.15,0.85,1)}65%{-webkit-transform:scale3d(.95,1.05,1);transform:scale3d(.95,1.05,1)}75%{-webkit-transform:scale3d(1.05,.95,1);transform:scale3d(1.05,.95,1)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}@keyframes rubberBand{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}30%{-webkit-transform:scale3d(1.25,0.75,1);transform:scale3d(1.25,0.75,1)}40%{-webkit-transform:scale3d(0.75,1.25,1);transform:scale3d(0.75,1.25,1)}50%{-webkit-transform:scale3d(1.15,0.85,1);transform:scale3d(1.15,0.85,1)}65%{-webkit-transform:scale3d(.95,1.05,1);transform:scale3d(.95,1.05,1)}75%{-webkit-transform:scale3d(1.05,.95,1);transform:scale3d(1.05,.95,1)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}.rubberBand{-webkit-animation-name:rubberBand;animation-name:rubberBand}@-webkit-keyframes shake{from,to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}10%,30%,50%,70%,90%{-webkit-transform:translate3d(-10px,0,0);transform:translate3d(-10px,0,0)}20%,40%,60%,80%{-webkit-transform:translate3d(10px,0,0);transform:translate3d(10px,0,0)}}@keyframes shake{from,to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}10%,30%,50%,70%,90%{-webkit-transform:translate3d(-10px,0,0);transform:translate3d(-10px,0,0)}20%,40%,60%,80%{-webkit-transform:translate3d(10px,0,0);transform:translate3d(10px,0,0)}}.shake{-webkit-animation-name:shake;animation-name:shake}@-webkit-keyframes headShake{0%{-webkit-transform:translateX(0);transform:translateX(0)}6.5%{-webkit-transform:translateX(-6px) rotateY(-9deg);transform:translateX(-6px) rotateY(-9deg)}18.5%{-webkit-transform:translateX(5px) rotateY(7deg);transform:translateX(5px) rotateY(7deg)}31.5%{-webkit-transform:translateX(-3px) rotateY(-5deg);transform:translateX(-3px) rotateY(-5deg)}43.5%{-webkit-transform:translateX(2px) rotateY(3deg);transform:translateX(2px) rotateY(3deg)}50%{-webkit-transform:translateX(0);transform:translateX(0)}}@keyframes headShake{0%{-webkit-transform:translateX(0);transform:translateX(0)}6.5%{-webkit-transform:translateX(-6px) rotateY(-9deg);transform:translateX(-6px) rotateY(-9deg)}18.5%{-webkit-transform:translateX(5px) rotateY(7deg);transform:translateX(5px) rotateY(7deg)}31.5%{-webkit-transform:translateX(-3px) rotateY(-5deg);transform:translateX(-3px) rotateY(-5deg)}43.5%{-webkit-transform:translateX(2px) rotateY(3deg);transform:translateX(2px) rotateY(3deg)}50%{-webkit-transform:translateX(0);transform:translateX(0)}}.headShake{-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out;-webkit-animation-name:headShake;animation-name:headShake}@-webkit-keyframes swing{20%{-webkit-transform:rotate3d(0,0,1,15deg);transform:rotate3d(0,0,1,15deg)}40%{-webkit-transform:rotate3d(0,0,1,-10deg);transform:rotate3d(0,0,1,-10deg)}60%{-webkit-transform:rotate3d(0,0,1,5deg);transform:rotate3d(0,0,1,5deg)}80%{-webkit-transform:rotate3d(0,0,1,-5deg);transform:rotate3d(0,0,1,-5deg)}to{-webkit-transform:rotate3d(0,0,1,0deg);transform:rotate3d(0,0,1,0deg)}}@keyframes swing{20%{-webkit-transform:rotate3d(0,0,1,15deg);transform:rotate3d(0,0,1,15deg)}40%{-webkit-transform:rotate3d(0,0,1,-10deg);transform:rotate3d(0,0,1,-10deg)}60%{-webkit-transform:rotate3d(0,0,1,5deg);transform:rotate3d(0,0,1,5deg)}80%{-webkit-transform:rotate3d(0,0,1,-5deg);transform:rotate3d(0,0,1,-5deg)}to{-webkit-transform:rotate3d(0,0,1,0deg);transform:rotate3d(0,0,1,0deg)}}.swing{-webkit-transform-origin:top center;transform-origin:top center;-webkit-animation-name:swing;animation-name:swing}@-webkit-keyframes tada{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}10%,20%{-webkit-transform:scale3d(.9,.9,.9) rotate3d(0,0,1,-3deg);transform:scale3d(.9,.9,.9) rotate3d(0,0,1,-3deg)}30%,50%,70%,90%{-webkit-transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,3deg);transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,3deg)}40%,60%,80%{-webkit-transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,-3deg);transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,-3deg)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}@keyframes tada{from{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}10%,20%{-webkit-transform:scale3d(.9,.9,.9) rotate3d(0,0,1,-3deg);transform:scale3d(.9,.9,.9) rotate3d(0,0,1,-3deg)}30%,50%,70%,90%{-webkit-transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,3deg);transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,3deg)}40%,60%,80%{-webkit-transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,-3deg);transform:scale3d(1.1,1.1,1.1) rotate3d(0,0,1,-3deg)}to{-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}.tada{-webkit-animation-name:tada;animation-name:tada}@-webkit-keyframes wobble{from{-webkit-transform:none;transform:none}15%{-webkit-transform:translate3d(-25%,0,0) rotate3d(0,0,1,-5deg);transform:translate3d(-25%,0,0) rotate3d(0,0,1,-5deg)}30%{-webkit-transform:translate3d(20%,0,0) rotate3d(0,0,1,3deg);transform:translate3d(20%,0,0) rotate3d(0,0,1,3deg)}45%{-webkit-transform:translate3d(-15%,0,0) rotate3d(0,0,1,-3deg);transform:translate3d(-15%,0,0) rotate3d(0,0,1,-3deg)}60%{-webkit-transform:translate3d(10%,0,0) rotate3d(0,0,1,2deg);transform:translate3d(10%,0,0) rotate3d(0,0,1,2deg)}75%{-webkit-transform:translate3d(-5%,0,0) rotate3d(0,0,1,-1deg);transform:translate3d(-5%,0,0) rotate3d(0,0,1,-1deg)}to{-webkit-transform:none;transform:none}}@keyframes wobble{from{-webkit-transform:none;transform:none}15%{-webkit-transform:translate3d(-25%,0,0) rotate3d(0,0,1,-5deg);transform:translate3d(-25%,0,0) rotate3d(0,0,1,-5deg)}30%{-webkit-transform:translate3d(20%,0,0) rotate3d(0,0,1,3deg);transform:translate3d(20%,0,0) rotate3d(0,0,1,3deg)}45%{-webkit-transform:translate3d(-15%,0,0) rotate3d(0,0,1,-3deg);transform:translate3d(-15%,0,0) rotate3d(0,0,1,-3deg)}60%{-webkit-transform:translate3d(10%,0,0) rotate3d(0,0,1,2deg);transform:translate3d(10%,0,0) rotate3d(0,0,1,2deg)}75%{-webkit-transform:translate3d(-5%,0,0) rotate3d(0,0,1,-1deg);transform:translate3d(-5%,0,0) rotate3d(0,0,1,-1deg)}to{-webkit-transform:none;transform:none}}.wobble{-webkit-animation-name:wobble;animation-name:wobble}@-webkit-keyframes jello{from,11.1%,to{-webkit-transform:none;transform:none}22.2%{-webkit-transform:skewX(-12.5deg) skewY(-12.5deg);transform:skewX(-12.5deg) skewY(-12.5deg)}33.3%{-webkit-transform:skewX(6.25deg) skewY(6.25deg);transform:skewX(6.25deg) skewY(6.25deg)}44.4%{-webkit-transform:skewX(-3.125deg) skewY(-3.125deg);transform:skewX(-3.125deg) skewY(-3.125deg)}55.5%{-webkit-transform:skewX(1.5625deg) skewY(1.5625deg);transform:skewX(1.5625deg) skewY(1.5625deg)}66.6%{-webkit-transform:skewX(-0.78125deg) skewY(-0.78125deg);transform:skewX(-0.78125deg) skewY(-0.78125deg)}77.7%{-webkit-transform:skewX(0.390625deg) skewY(0.390625deg);transform:skewX(0.390625deg) skewY(0.390625deg)}88.8%{-webkit-transform:skewX(-0.1953125deg) skewY(-0.1953125deg);transform:skewX(-0.1953125deg) skewY(-0.1953125deg)}}@keyframes jello{from,11.1%,to{-webkit-transform:none;transform:none}22.2%{-webkit-transform:skewX(-12.5deg) skewY(-12.5deg);transform:skewX(-12.5deg) skewY(-12.5deg)}33.3%{-webkit-transform:skewX(6.25deg) skewY(6.25deg);transform:skewX(6.25deg) skewY(6.25deg)}44.4%{-webkit-transform:skewX(-3.125deg) skewY(-3.125deg);transform:skewX(-3.125deg) skewY(-3.125deg)}55.5%{-webkit-transform:skewX(1.5625deg) skewY(1.5625deg);transform:skewX(1.5625deg) skewY(1.5625deg)}66.6%{-webkit-transform:skewX(-0.78125deg) skewY(-0.78125deg);transform:skewX(-0.78125deg) skewY(-0.78125deg)}77.7%{-webkit-transform:skewX(0.390625deg) skewY(0.390625deg);transform:skewX(0.390625deg) skewY(0.390625deg)}88.8%{-webkit-transform:skewX(-0.1953125deg) skewY(-0.1953125deg);transform:skewX(-0.1953125deg) skewY(-0.1953125deg)}}.jello{-webkit-animation-name:jello;animation-name:jello;-webkit-transform-origin:center;transform-origin:center}@-webkit-keyframes bounceIn{from,20%,40%,60%,80%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}20%{-webkit-transform:scale3d(1.1,1.1,1.1);transform:scale3d(1.1,1.1,1.1)}40%{-webkit-transform:scale3d(.9,.9,.9);transform:scale3d(.9,.9,.9)}60%{opacity:1;-webkit-transform:scale3d(1.03,1.03,1.03);transform:scale3d(1.03,1.03,1.03)}80%{-webkit-transform:scale3d(.97,.97,.97);transform:scale3d(.97,.97,.97)}to{opacity:1;-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}@keyframes bounceIn{from,20%,40%,60%,80%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}20%{-webkit-transform:scale3d(1.1,1.1,1.1);transform:scale3d(1.1,1.1,1.1)}40%{-webkit-transform:scale3d(.9,.9,.9);transform:scale3d(.9,.9,.9)}60%{opacity:1;-webkit-transform:scale3d(1.03,1.03,1.03);transform:scale3d(1.03,1.03,1.03)}80%{-webkit-transform:scale3d(.97,.97,.97);transform:scale3d(.97,.97,.97)}to{opacity:1;-webkit-transform:scale3d(1,1,1);transform:scale3d(1,1,1)}}.bounceIn{-webkit-animation-name:bounceIn;animation-name:bounceIn}@-webkit-keyframes bounceInDown{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:translate3d(0,-3000px,0);transform:translate3d(0,-3000px,0)}60%{opacity:1;-webkit-transform:translate3d(0,25px,0);transform:translate3d(0,25px,0)}75%{-webkit-transform:translate3d(0,-10px,0);transform:translate3d(0,-10px,0)}90%{-webkit-transform:translate3d(0,5px,0);transform:translate3d(0,5px,0)}to{-webkit-transform:none;transform:none}}@keyframes bounceInDown{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:translate3d(0,-3000px,0);transform:translate3d(0,-3000px,0)}60%{opacity:1;-webkit-transform:translate3d(0,25px,0);transform:translate3d(0,25px,0)}75%{-webkit-transform:translate3d(0,-10px,0);transform:translate3d(0,-10px,0)}90%{-webkit-transform:translate3d(0,5px,0);transform:translate3d(0,5px,0)}to{-webkit-transform:none;transform:none}}.bounceInDown{-webkit-animation-name:bounceInDown;animation-name:bounceInDown}@-webkit-keyframes bounceInLeft{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:translate3d(-3000px,0,0);transform:translate3d(-3000px,0,0)}60%{opacity:1;-webkit-transform:translate3d(25px,0,0);transform:translate3d(25px,0,0)}75%{-webkit-transform:translate3d(-10px,0,0);transform:translate3d(-10px,0,0)}90%{-webkit-transform:translate3d(5px,0,0);transform:translate3d(5px,0,0)}to{-webkit-transform:none;transform:none}}@keyframes bounceInLeft{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}0%{opacity:0;-webkit-transform:translate3d(-3000px,0,0);transform:translate3d(-3000px,0,0)}60%{opacity:1;-webkit-transform:translate3d(25px,0,0);transform:translate3d(25px,0,0)}75%{-webkit-transform:translate3d(-10px,0,0);transform:translate3d(-10px,0,0)}90%{-webkit-transform:translate3d(5px,0,0);transform:translate3d(5px,0,0)}to{-webkit-transform:none;transform:none}}.bounceInLeft{-webkit-animation-name:bounceInLeft;animation-name:bounceInLeft}@-webkit-keyframes bounceInRight{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}from{opacity:0;-webkit-transform:translate3d(3000px,0,0);transform:translate3d(3000px,0,0)}60%{opacity:1;-webkit-transform:translate3d(-25px,0,0);transform:translate3d(-25px,0,0)}75%{-webkit-transform:translate3d(10px,0,0);transform:translate3d(10px,0,0)}90%{-webkit-transform:translate3d(-5px,0,0);transform:translate3d(-5px,0,0)}to{-webkit-transform:none;transform:none}}@keyframes bounceInRight{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}from{opacity:0;-webkit-transform:translate3d(3000px,0,0);transform:translate3d(3000px,0,0)}60%{opacity:1;-webkit-transform:translate3d(-25px,0,0);transform:translate3d(-25px,0,0)}75%{-webkit-transform:translate3d(10px,0,0);transform:translate3d(10px,0,0)}90%{-webkit-transform:translate3d(-5px,0,0);transform:translate3d(-5px,0,0)}to{-webkit-transform:none;transform:none}}.bounceInRight{-webkit-animation-name:bounceInRight;animation-name:bounceInRight}@-webkit-keyframes bounceInUp{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}from{opacity:0;-webkit-transform:translate3d(0,3000px,0);transform:translate3d(0,3000px,0)}60%{opacity:1;-webkit-transform:translate3d(0,-20px,0);transform:translate3d(0,-20px,0)}75%{-webkit-transform:translate3d(0,10px,0);transform:translate3d(0,10px,0)}90%{-webkit-transform:translate3d(0,-5px,0);transform:translate3d(0,-5px,0)}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}@keyframes bounceInUp{from,60%,75%,90%,to{-webkit-animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000);animation-timing-function:cubic-bezier(0.215,0.610,0.355,1.000)}from{opacity:0;-webkit-transform:translate3d(0,3000px,0);transform:translate3d(0,3000px,0)}60%{opacity:1;-webkit-transform:translate3d(0,-20px,0);transform:translate3d(0,-20px,0)}75%{-webkit-transform:translate3d(0,10px,0);transform:translate3d(0,10px,0)}90%{-webkit-transform:translate3d(0,-5px,0);transform:translate3d(0,-5px,0)}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.bounceInUp{-webkit-animation-name:bounceInUp;animation-name:bounceInUp}@-webkit-keyframes bounceOut{20%{-webkit-transform:scale3d(.9,.9,.9);transform:scale3d(.9,.9,.9)}50%,55%{opacity:1;-webkit-transform:scale3d(1.1,1.1,1.1);transform:scale3d(1.1,1.1,1.1)}to{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}}@keyframes bounceOut{20%{-webkit-transform:scale3d(.9,.9,.9);transform:scale3d(.9,.9,.9)}50%,55%{opacity:1;-webkit-transform:scale3d(1.1,1.1,1.1);transform:scale3d(1.1,1.1,1.1)}to{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}}.bounceOut{-webkit-animation-name:bounceOut;animation-name:bounceOut}@-webkit-keyframes bounceOutDown{20%{-webkit-transform:translate3d(0,10px,0);transform:translate3d(0,10px,0)}40%,45%{opacity:1;-webkit-transform:translate3d(0,-20px,0);transform:translate3d(0,-20px,0)}to{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}}@keyframes bounceOutDown{20%{-webkit-transform:translate3d(0,10px,0);transform:translate3d(0,10px,0)}40%,45%{opacity:1;-webkit-transform:translate3d(0,-20px,0);transform:translate3d(0,-20px,0)}to{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}}.bounceOutDown{-webkit-animation-name:bounceOutDown;animation-name:bounceOutDown}@-webkit-keyframes bounceOutLeft{20%{opacity:1;-webkit-transform:translate3d(20px,0,0);transform:translate3d(20px,0,0)}to{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}}@keyframes bounceOutLeft{20%{opacity:1;-webkit-transform:translate3d(20px,0,0);transform:translate3d(20px,0,0)}to{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}}.bounceOutLeft{-webkit-animation-name:bounceOutLeft;animation-name:bounceOutLeft}@-webkit-keyframes bounceOutRight{20%{opacity:1;-webkit-transform:translate3d(-20px,0,0);transform:translate3d(-20px,0,0)}to{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}}@keyframes bounceOutRight{20%{opacity:1;-webkit-transform:translate3d(-20px,0,0);transform:translate3d(-20px,0,0)}to{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}}.bounceOutRight{-webkit-animation-name:bounceOutRight;animation-name:bounceOutRight}@-webkit-keyframes bounceOutUp{20%{-webkit-transform:translate3d(0,-10px,0);transform:translate3d(0,-10px,0)}40%,45%{opacity:1;-webkit-transform:translate3d(0,20px,0);transform:translate3d(0,20px,0)}to{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}}@keyframes bounceOutUp{20%{-webkit-transform:translate3d(0,-10px,0);transform:translate3d(0,-10px,0)}40%,45%{opacity:1;-webkit-transform:translate3d(0,20px,0);transform:translate3d(0,20px,0)}to{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}}.bounceOutUp{-webkit-animation-name:bounceOutUp;animation-name:bounceOutUp}@-webkit-keyframes fadeIn{from{opacity:0}to{opacity:1}}@keyframes fadeIn{from{opacity:0}to{opacity:1}}.fadeIn{-webkit-animation-name:fadeIn;animation-name:fadeIn}@-webkit-keyframes fadeInDown{from{opacity:0;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInDown{from{opacity:0;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInDown{-webkit-animation-name:fadeInDown;animation-name:fadeInDown}@-webkit-keyframes fadeInDownBig{from{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInDownBig{from{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInDownBig{-webkit-animation-name:fadeInDownBig;animation-name:fadeInDownBig}@-webkit-keyframes fadeInLeft{from{opacity:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInLeft{from{opacity:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInLeft{-webkit-animation-name:fadeInLeft;animation-name:fadeInLeft}@-webkit-keyframes fadeInLeftBig{from{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInLeftBig{from{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInLeftBig{-webkit-animation-name:fadeInLeftBig;animation-name:fadeInLeftBig}@-webkit-keyframes fadeInRight{from{opacity:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInRight{from{opacity:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInRight{-webkit-animation-name:fadeInRight;animation-name:fadeInRight}@-webkit-keyframes fadeInRightBig{from{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInRightBig{from{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInRightBig{-webkit-animation-name:fadeInRightBig;animation-name:fadeInRightBig}@-webkit-keyframes fadeInUp{from{opacity:0;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInUp{from{opacity:0;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInUp{-webkit-animation-name:fadeInUp;animation-name:fadeInUp}@-webkit-keyframes fadeInUpBig{from{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes fadeInUpBig{from{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}to{opacity:1;-webkit-transform:none;transform:none}}.fadeInUpBig{-webkit-animation-name:fadeInUpBig;animation-name:fadeInUpBig}@-webkit-keyframes fadeOut{from{opacity:1}to{opacity:0}}@keyframes fadeOut{from{opacity:1}to{opacity:0}}.fadeOut{-webkit-animation-name:fadeOut;animation-name:fadeOut}@-webkit-keyframes fadeOutDown{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}}@keyframes fadeOutDown{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}}.fadeOutDown{-webkit-animation-name:fadeOutDown;animation-name:fadeOutDown}@-webkit-keyframes fadeOutDownBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}}@keyframes fadeOutDownBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,2000px,0);transform:translate3d(0,2000px,0)}}.fadeOutDownBig{-webkit-animation-name:fadeOutDownBig;animation-name:fadeOutDownBig}@-webkit-keyframes fadeOutLeft{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}}@keyframes fadeOutLeft{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}}.fadeOutLeft{-webkit-animation-name:fadeOutLeft;animation-name:fadeOutLeft}@-webkit-keyframes fadeOutLeftBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}}@keyframes fadeOutLeftBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(-2000px,0,0);transform:translate3d(-2000px,0,0)}}.fadeOutLeftBig{-webkit-animation-name:fadeOutLeftBig;animation-name:fadeOutLeftBig}@-webkit-keyframes fadeOutRight{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}}@keyframes fadeOutRight{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}}.fadeOutRight{-webkit-animation-name:fadeOutRight;animation-name:fadeOutRight}@-webkit-keyframes fadeOutRightBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}}@keyframes fadeOutRightBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(2000px,0,0);transform:translate3d(2000px,0,0)}}.fadeOutRightBig{-webkit-animation-name:fadeOutRightBig;animation-name:fadeOutRightBig}@-webkit-keyframes fadeOutUp{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}}@keyframes fadeOutUp{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}}.fadeOutUp{-webkit-animation-name:fadeOutUp;animation-name:fadeOutUp}@-webkit-keyframes fadeOutUpBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}}@keyframes fadeOutUpBig{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(0,-2000px,0);transform:translate3d(0,-2000px,0)}}.fadeOutUpBig{-webkit-animation-name:fadeOutUpBig;animation-name:fadeOutUpBig}@-webkit-keyframes flip{from{-webkit-transform:perspective(400px) rotate3d(0,1,0,-360deg);transform:perspective(400px) rotate3d(0,1,0,-360deg);-webkit-animation-timing-function:ease-out;animation-timing-function:ease-out}40%{-webkit-transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-190deg);transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-190deg);-webkit-animation-timing-function:ease-out;animation-timing-function:ease-out}50%{-webkit-transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-170deg);transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-170deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}80%{-webkit-transform:perspective(400px) scale3d(.95,.95,.95);transform:perspective(400px) scale3d(.95,.95,.95);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}to{-webkit-transform:perspective(400px);transform:perspective(400px);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}}@keyframes flip{from{-webkit-transform:perspective(400px) rotate3d(0,1,0,-360deg);transform:perspective(400px) rotate3d(0,1,0,-360deg);-webkit-animation-timing-function:ease-out;animation-timing-function:ease-out}40%{-webkit-transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-190deg);transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-190deg);-webkit-animation-timing-function:ease-out;animation-timing-function:ease-out}50%{-webkit-transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-170deg);transform:perspective(400px) translate3d(0,0,150px) rotate3d(0,1,0,-170deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}80%{-webkit-transform:perspective(400px) scale3d(.95,.95,.95);transform:perspective(400px) scale3d(.95,.95,.95);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}to{-webkit-transform:perspective(400px);transform:perspective(400px);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}}.animated.flip{-webkit-backface-visibility:visible;backface-visibility:visible;-webkit-animation-name:flip;animation-name:flip}@-webkit-keyframes flipInX{from{-webkit-transform:perspective(400px) rotate3d(1,0,0,90deg);transform:perspective(400px) rotate3d(1,0,0,90deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in;opacity:0}40%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-20deg);transform:perspective(400px) rotate3d(1,0,0,-20deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}60%{-webkit-transform:perspective(400px) rotate3d(1,0,0,10deg);transform:perspective(400px) rotate3d(1,0,0,10deg);opacity:1}80%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-5deg);transform:perspective(400px) rotate3d(1,0,0,-5deg)}to{-webkit-transform:perspective(400px);transform:perspective(400px)}}@keyframes flipInX{from{-webkit-transform:perspective(400px) rotate3d(1,0,0,90deg);transform:perspective(400px) rotate3d(1,0,0,90deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in;opacity:0}40%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-20deg);transform:perspective(400px) rotate3d(1,0,0,-20deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}60%{-webkit-transform:perspective(400px) rotate3d(1,0,0,10deg);transform:perspective(400px) rotate3d(1,0,0,10deg);opacity:1}80%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-5deg);transform:perspective(400px) rotate3d(1,0,0,-5deg)}to{-webkit-transform:perspective(400px);transform:perspective(400px)}}.flipInX{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;-webkit-animation-name:flipInX;animation-name:flipInX}@-webkit-keyframes flipInY{from{-webkit-transform:perspective(400px) rotate3d(0,1,0,90deg);transform:perspective(400px) rotate3d(0,1,0,90deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in;opacity:0}40%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-20deg);transform:perspective(400px) rotate3d(0,1,0,-20deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}60%{-webkit-transform:perspective(400px) rotate3d(0,1,0,10deg);transform:perspective(400px) rotate3d(0,1,0,10deg);opacity:1}80%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-5deg);transform:perspective(400px) rotate3d(0,1,0,-5deg)}to{-webkit-transform:perspective(400px);transform:perspective(400px)}}@keyframes flipInY{from{-webkit-transform:perspective(400px) rotate3d(0,1,0,90deg);transform:perspective(400px) rotate3d(0,1,0,90deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in;opacity:0}40%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-20deg);transform:perspective(400px) rotate3d(0,1,0,-20deg);-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}60%{-webkit-transform:perspective(400px) rotate3d(0,1,0,10deg);transform:perspective(400px) rotate3d(0,1,0,10deg);opacity:1}80%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-5deg);transform:perspective(400px) rotate3d(0,1,0,-5deg)}to{-webkit-transform:perspective(400px);transform:perspective(400px)}}.flipInY{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;-webkit-animation-name:flipInY;animation-name:flipInY}@-webkit-keyframes flipOutX{from{-webkit-transform:perspective(400px);transform:perspective(400px)}30%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-20deg);transform:perspective(400px) rotate3d(1,0,0,-20deg);opacity:1}to{-webkit-transform:perspective(400px) rotate3d(1,0,0,90deg);transform:perspective(400px) rotate3d(1,0,0,90deg);opacity:0}}@keyframes flipOutX{from{-webkit-transform:perspective(400px);transform:perspective(400px)}30%{-webkit-transform:perspective(400px) rotate3d(1,0,0,-20deg);transform:perspective(400px) rotate3d(1,0,0,-20deg);opacity:1}to{-webkit-transform:perspective(400px) rotate3d(1,0,0,90deg);transform:perspective(400px) rotate3d(1,0,0,90deg);opacity:0}}.flipOutX{-webkit-animation-name:flipOutX;animation-name:flipOutX;-webkit-backface-visibility:visible!important;backface-visibility:visible!important}@-webkit-keyframes flipOutY{from{-webkit-transform:perspective(400px);transform:perspective(400px)}30%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-15deg);transform:perspective(400px) rotate3d(0,1,0,-15deg);opacity:1}to{-webkit-transform:perspective(400px) rotate3d(0,1,0,90deg);transform:perspective(400px) rotate3d(0,1,0,90deg);opacity:0}}@keyframes flipOutY{from{-webkit-transform:perspective(400px);transform:perspective(400px)}30%{-webkit-transform:perspective(400px) rotate3d(0,1,0,-15deg);transform:perspective(400px) rotate3d(0,1,0,-15deg);opacity:1}to{-webkit-transform:perspective(400px) rotate3d(0,1,0,90deg);transform:perspective(400px) rotate3d(0,1,0,90deg);opacity:0}}.flipOutY{-webkit-backface-visibility:visible!important;backface-visibility:visible!important;-webkit-animation-name:flipOutY;animation-name:flipOutY}@-webkit-keyframes lightSpeedIn{from{-webkit-transform:translate3d(100%,0,0) skewX(-30deg);transform:translate3d(100%,0,0) skewX(-30deg);opacity:0}60%{-webkit-transform:skewX(20deg);transform:skewX(20deg);opacity:1}80%{-webkit-transform:skewX(-5deg);transform:skewX(-5deg);opacity:1}to{-webkit-transform:none;transform:none;opacity:1}}@keyframes lightSpeedIn{from{-webkit-transform:translate3d(100%,0,0) skewX(-30deg);transform:translate3d(100%,0,0) skewX(-30deg);opacity:0}60%{-webkit-transform:skewX(20deg);transform:skewX(20deg);opacity:1}80%{-webkit-transform:skewX(-5deg);transform:skewX(-5deg);opacity:1}to{-webkit-transform:none;transform:none;opacity:1}}.lightSpeedIn{-webkit-animation-name:lightSpeedIn;animation-name:lightSpeedIn;-webkit-animation-timing-function:ease-out;animation-timing-function:ease-out}@-webkit-keyframes lightSpeedOut{from{opacity:1}to{-webkit-transform:translate3d(100%,0,0) skewX(30deg);transform:translate3d(100%,0,0) skewX(30deg);opacity:0}}@keyframes lightSpeedOut{from{opacity:1}to{-webkit-transform:translate3d(100%,0,0) skewX(30deg);transform:translate3d(100%,0,0) skewX(30deg);opacity:0}}.lightSpeedOut{-webkit-animation-name:lightSpeedOut;animation-name:lightSpeedOut;-webkit-animation-timing-function:ease-in;animation-timing-function:ease-in}@-webkit-keyframes rotateIn{from{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:rotate3d(0,0,1,-200deg);transform:rotate3d(0,0,1,-200deg);opacity:0}to{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:none;transform:none;opacity:1}}@keyframes rotateIn{from{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:rotate3d(0,0,1,-200deg);transform:rotate3d(0,0,1,-200deg);opacity:0}to{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:none;transform:none;opacity:1}}.rotateIn{-webkit-animation-name:rotateIn;animation-name:rotateIn}@-webkit-keyframes rotateInDownLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:none;transform:none;opacity:1}}@keyframes rotateInDownLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:none;transform:none;opacity:1}}.rotateInDownLeft{-webkit-animation-name:rotateInDownLeft;animation-name:rotateInDownLeft}@-webkit-keyframes rotateInDownRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:none;transform:none;opacity:1}}@keyframes rotateInDownRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:none;transform:none;opacity:1}}.rotateInDownRight{-webkit-animation-name:rotateInDownRight;animation-name:rotateInDownRight}@-webkit-keyframes rotateInUpLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:none;transform:none;opacity:1}}@keyframes rotateInUpLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:none;transform:none;opacity:1}}.rotateInUpLeft{-webkit-animation-name:rotateInUpLeft;animation-name:rotateInUpLeft}@-webkit-keyframes rotateInUpRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,-90deg);transform:rotate3d(0,0,1,-90deg);opacity:0}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:none;transform:none;opacity:1}}@keyframes rotateInUpRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,-90deg);transform:rotate3d(0,0,1,-90deg);opacity:0}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:none;transform:none;opacity:1}}.rotateInUpRight{-webkit-animation-name:rotateInUpRight;animation-name:rotateInUpRight}@-webkit-keyframes rotateOut{from{-webkit-transform-origin:center;transform-origin:center;opacity:1}to{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:rotate3d(0,0,1,200deg);transform:rotate3d(0,0,1,200deg);opacity:0}}@keyframes rotateOut{from{-webkit-transform-origin:center;transform-origin:center;opacity:1}to{-webkit-transform-origin:center;transform-origin:center;-webkit-transform:rotate3d(0,0,1,200deg);transform:rotate3d(0,0,1,200deg);opacity:0}}.rotateOut{-webkit-animation-name:rotateOut;animation-name:rotateOut}@-webkit-keyframes rotateOutDownLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;opacity:1}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}}@keyframes rotateOutDownLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;opacity:1}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,45deg);transform:rotate3d(0,0,1,45deg);opacity:0}}.rotateOutDownLeft{-webkit-animation-name:rotateOutDownLeft;animation-name:rotateOutDownLeft}@-webkit-keyframes rotateOutDownRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;opacity:1}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}}@keyframes rotateOutDownRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;opacity:1}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}}.rotateOutDownRight{-webkit-animation-name:rotateOutDownRight;animation-name:rotateOutDownRight}@-webkit-keyframes rotateOutUpLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;opacity:1}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}}@keyframes rotateOutUpLeft{from{-webkit-transform-origin:left bottom;transform-origin:left bottom;opacity:1}to{-webkit-transform-origin:left bottom;transform-origin:left bottom;-webkit-transform:rotate3d(0,0,1,-45deg);transform:rotate3d(0,0,1,-45deg);opacity:0}}.rotateOutUpLeft{-webkit-animation-name:rotateOutUpLeft;animation-name:rotateOutUpLeft}@-webkit-keyframes rotateOutUpRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;opacity:1}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,90deg);transform:rotate3d(0,0,1,90deg);opacity:0}}@keyframes rotateOutUpRight{from{-webkit-transform-origin:right bottom;transform-origin:right bottom;opacity:1}to{-webkit-transform-origin:right bottom;transform-origin:right bottom;-webkit-transform:rotate3d(0,0,1,90deg);transform:rotate3d(0,0,1,90deg);opacity:0}}.rotateOutUpRight{-webkit-animation-name:rotateOutUpRight;animation-name:rotateOutUpRight}@-webkit-keyframes hinge{0%{-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out}20%,60%{-webkit-transform:rotate3d(0,0,1,80deg);transform:rotate3d(0,0,1,80deg);-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out}40%,80%{-webkit-transform:rotate3d(0,0,1,60deg);transform:rotate3d(0,0,1,60deg);-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out;opacity:1}to{-webkit-transform:translate3d(0,700px,0);transform:translate3d(0,700px,0);opacity:0}}@keyframes hinge{0%{-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out}20%,60%{-webkit-transform:rotate3d(0,0,1,80deg);transform:rotate3d(0,0,1,80deg);-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out}40%,80%{-webkit-transform:rotate3d(0,0,1,60deg);transform:rotate3d(0,0,1,60deg);-webkit-transform-origin:top left;transform-origin:top left;-webkit-animation-timing-function:ease-in-out;animation-timing-function:ease-in-out;opacity:1}to{-webkit-transform:translate3d(0,700px,0);transform:translate3d(0,700px,0);opacity:0}}.hinge{-webkit-animation-name:hinge;animation-name:hinge}@-webkit-keyframes rollIn{from{opacity:0;-webkit-transform:translate3d(-100%,0,0) rotate3d(0,0,1,-120deg);transform:translate3d(-100%,0,0) rotate3d(0,0,1,-120deg)}to{opacity:1;-webkit-transform:none;transform:none}}@keyframes rollIn{from{opacity:0;-webkit-transform:translate3d(-100%,0,0) rotate3d(0,0,1,-120deg);transform:translate3d(-100%,0,0) rotate3d(0,0,1,-120deg)}to{opacity:1;-webkit-transform:none;transform:none}}.rollIn{-webkit-animation-name:rollIn;animation-name:rollIn}@-webkit-keyframes rollOut{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(100%,0,0) rotate3d(0,0,1,120deg);transform:translate3d(100%,0,0) rotate3d(0,0,1,120deg)}}@keyframes rollOut{from{opacity:1}to{opacity:0;-webkit-transform:translate3d(100%,0,0) rotate3d(0,0,1,120deg);transform:translate3d(100%,0,0) rotate3d(0,0,1,120deg)}}.rollOut{-webkit-animation-name:rollOut;animation-name:rollOut}@-webkit-keyframes zoomIn{from{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}50%{opacity:1}}@keyframes zoomIn{from{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}50%{opacity:1}}.zoomIn{-webkit-animation-name:zoomIn;animation-name:zoomIn}@-webkit-keyframes zoomInDown{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,-1000px,0);transform:scale3d(.1,.1,.1) translate3d(0,-1000px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,60px,0);transform:scale3d(.475,.475,.475) translate3d(0,60px,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomInDown{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,-1000px,0);transform:scale3d(.1,.1,.1) translate3d(0,-1000px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,60px,0);transform:scale3d(.475,.475,.475) translate3d(0,60px,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomInDown{-webkit-animation-name:zoomInDown;animation-name:zoomInDown}@-webkit-keyframes zoomInLeft{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(-1000px,0,0);transform:scale3d(.1,.1,.1) translate3d(-1000px,0,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(10px,0,0);transform:scale3d(.475,.475,.475) translate3d(10px,0,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomInLeft{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(-1000px,0,0);transform:scale3d(.1,.1,.1) translate3d(-1000px,0,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(10px,0,0);transform:scale3d(.475,.475,.475) translate3d(10px,0,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomInLeft{-webkit-animation-name:zoomInLeft;animation-name:zoomInLeft}@-webkit-keyframes zoomInRight{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(1000px,0,0);transform:scale3d(.1,.1,.1) translate3d(1000px,0,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(-10px,0,0);transform:scale3d(.475,.475,.475) translate3d(-10px,0,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomInRight{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(1000px,0,0);transform:scale3d(.1,.1,.1) translate3d(1000px,0,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(-10px,0,0);transform:scale3d(.475,.475,.475) translate3d(-10px,0,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomInRight{-webkit-animation-name:zoomInRight;animation-name:zoomInRight}@-webkit-keyframes zoomInUp{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,1000px,0);transform:scale3d(.1,.1,.1) translate3d(0,1000px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomInUp{from{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,1000px,0);transform:scale3d(.1,.1,.1) translate3d(0,1000px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}60%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomInUp{-webkit-animation-name:zoomInUp;animation-name:zoomInUp}@-webkit-keyframes zoomOut{from{opacity:1}50%{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}to{opacity:0}}@keyframes zoomOut{from{opacity:1}50%{opacity:0;-webkit-transform:scale3d(.3,.3,.3);transform:scale3d(.3,.3,.3)}to{opacity:0}}.zoomOut{-webkit-animation-name:zoomOut;animation-name:zoomOut}@-webkit-keyframes zoomOutDown{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}to{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,2000px,0);transform:scale3d(.1,.1,.1) translate3d(0,2000px,0);-webkit-transform-origin:center bottom;transform-origin:center bottom;-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomOutDown{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);transform:scale3d(.475,.475,.475) translate3d(0,-60px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}to{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,2000px,0);transform:scale3d(.1,.1,.1) translate3d(0,2000px,0);-webkit-transform-origin:center bottom;transform-origin:center bottom;-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomOutDown{-webkit-animation-name:zoomOutDown;animation-name:zoomOutDown}@-webkit-keyframes zoomOutLeft{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(42px,0,0);transform:scale3d(.475,.475,.475) translate3d(42px,0,0)}to{opacity:0;-webkit-transform:scale(.1) translate3d(-2000px,0,0);transform:scale(.1) translate3d(-2000px,0,0);-webkit-transform-origin:left center;transform-origin:left center}}@keyframes zoomOutLeft{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(42px,0,0);transform:scale3d(.475,.475,.475) translate3d(42px,0,0)}to{opacity:0;-webkit-transform:scale(.1) translate3d(-2000px,0,0);transform:scale(.1) translate3d(-2000px,0,0);-webkit-transform-origin:left center;transform-origin:left center}}.zoomOutLeft{-webkit-animation-name:zoomOutLeft;animation-name:zoomOutLeft}@-webkit-keyframes zoomOutRight{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(-42px,0,0);transform:scale3d(.475,.475,.475) translate3d(-42px,0,0)}to{opacity:0;-webkit-transform:scale(.1) translate3d(2000px,0,0);transform:scale(.1) translate3d(2000px,0,0);-webkit-transform-origin:right center;transform-origin:right center}}@keyframes zoomOutRight{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(-42px,0,0);transform:scale3d(.475,.475,.475) translate3d(-42px,0,0)}to{opacity:0;-webkit-transform:scale(.1) translate3d(2000px,0,0);transform:scale(.1) translate3d(2000px,0,0);-webkit-transform-origin:right center;transform-origin:right center}}.zoomOutRight{-webkit-animation-name:zoomOutRight;animation-name:zoomOutRight}@-webkit-keyframes zoomOutUp{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,60px,0);transform:scale3d(.475,.475,.475) translate3d(0,60px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}to{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,-2000px,0);transform:scale3d(.1,.1,.1) translate3d(0,-2000px,0);-webkit-transform-origin:center bottom;transform-origin:center bottom;-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}@keyframes zoomOutUp{40%{opacity:1;-webkit-transform:scale3d(.475,.475,.475) translate3d(0,60px,0);transform:scale3d(.475,.475,.475) translate3d(0,60px,0);-webkit-animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190);animation-timing-function:cubic-bezier(0.550,0.055,0.675,0.190)}to{opacity:0;-webkit-transform:scale3d(.1,.1,.1) translate3d(0,-2000px,0);transform:scale3d(.1,.1,.1) translate3d(0,-2000px,0);-webkit-transform-origin:center bottom;transform-origin:center bottom;-webkit-animation-timing-function:cubic-bezier(0.175,0.885,0.320,1);animation-timing-function:cubic-bezier(0.175,0.885,0.320,1)}}.zoomOutUp{-webkit-animation-name:zoomOutUp;animation-name:zoomOutUp}@-webkit-keyframes slideInDown{from{-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}@keyframes slideInDown{from{-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.slideInDown{-webkit-animation-name:slideInDown;animation-name:slideInDown}@-webkit-keyframes slideInLeft{from{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}@keyframes slideInLeft{from{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.slideInLeft{-webkit-animation-name:slideInLeft;animation-name:slideInLeft}@-webkit-keyframes slideInRight{from{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}@keyframes slideInRight{from{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.slideInRight{-webkit-animation-name:slideInRight;animation-name:slideInRight}@-webkit-keyframes slideInUp{from{-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}@keyframes slideInUp{from{-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0);visibility:visible}to{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.slideInUp{-webkit-animation-name:slideInUp;animation-name:slideInUp}@-webkit-keyframes slideOutDown{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}}@keyframes slideOutDown{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(0,100%,0);transform:translate3d(0,100%,0)}}.slideOutDown{-webkit-animation-name:slideOutDown;animation-name:slideOutDown}@-webkit-keyframes slideOutLeft{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}}@keyframes slideOutLeft{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}}.slideOutLeft{-webkit-animation-name:slideOutLeft;animation-name:slideOutLeft}@-webkit-keyframes slideOutRight{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}}@keyframes slideOutRight{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}}.slideOutRight{-webkit-animation-name:slideOutRight;animation-name:slideOutRight}@-webkit-keyframes slideOutUp{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}}@keyframes slideOutUp{from{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}to{visibility:hidden;-webkit-transform:translate3d(0,-100%,0);transform:translate3d(0,-100%,0)}}.slideOutUp{-webkit-animation-name:slideOutUp;animation-name:slideOutUp}
/*-------------------------------------------*/
/*  3. Global CSS
/*-------------------------------------------*/
body{font-family:'Open Sans',sans-serif;font-size:14px;font-weight:400;line-height:1.5;overflow-x:hidden;-webkit-font-smoothing:antialiased;-moz-font-smoothing:antialiased;text-rendering:optimizeLegibility}
a,button{-webkit-transition:all .3s;transition:all .3s}
a button:hover,a:focus,a:hover,button button:hover,button:focus,button:hover{-webkit-transition:all .3s;transition:all .3s;text-decoration:none}
.btn{border-radius:0}
.section-title{display:block;margin-bottom:100px}
.section-title .title{font-weight:800;display:inline-block;margin-top:0;margin-bottom:10px}
.section-title .sub-title{font-size:16px;line-height:30px;color:gray}
.section-title.text-left h1{margin-left:20px}
.section-title.text-right h1{margin-right:20px}
.light-txt h1,.light-txt h5,.light-txt p{margin-top:0}
.light-txt .sub-title,.light-txt div{margin-top:0;color:#fff}
.light-txt h1,.light-txt h2,.light-txt h3,.light-txt h4,.light-txt h5,.light-txt p,.light-txt span{color:#fff}
.quote .quote-img img{width:40px;height:auto;margin-bottom:15px;padding:10px;opacity:.7}
.quote p{margin-bottom:0}
#preloader{position:fixed;z-index:1800;top:0;right:0;bottom:0;left:0;width:100%;height:100%;background:#000}
.no-js #preloader,.oldie #preloader{display:none}
#loader{position:absolute;top:50%;left:50%;width:60px;height:60px;margin:-30px 0 0 -30px;padding:0}
#loader:before{display:block;width:60px;height:60px;content:'';-webkit-animation:load 1.1s infinite linear;animation:load 1.1s infinite linear;border-top:2px solid rgba(255,255,255,.1);border-right:2px solid rgba(255,255,255,.1);border-bottom:2px solid rgba(255,255,255,.1);border-left:2px solid #2196f3;border-radius:50%}
@-webkit-keyframes load {
0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}
to{-webkit-transform:rotate(360deg);transform:rotate(360deg)}
}
@keyframes load {
0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}
to{-webkit-transform:rotate(360deg);transform:rotate(360deg)}
}
.white-highlight{color:#fff}
.section-padding{padding-top:60px;padding-bottom:60px}
.page-header{margin:0;padding:0;border:0;text-align:center;position:relative}
.page-header h1{font-weight:700;color:#282528;text-transform:uppercase}
.page-header .border-bottom{width:12px;height:12px;border-radius:50%;-moz-border-radius:50%;-webkit-border-radius:50%;margin:0 auto;position:relative}
.page-header .border-bottom:before,.page-header .border-bottom:after{content:"";position:absolute;height:1px;width:60px}
.page-header .border-bottom:before{left:-70px;bottom:5px}
.page-header .border-bottom:after{right:-70px;bottom:5px}
.color-highlight{color:#2196f3}
.page-header .border-bottom{border:1px solid #2196f3}
.page-header .border-bottom:before,.page-header .border-bottom:after{background:#2196f3}
.ct-wrapper{padding:0 20px;position:relative;max-width:1230px;margin:0 auto}
.main-wrapper{width:auto;margin-right:365px}
#content{position:relative;width:100%;float:left}
.sidebar-wrapper{width:330px!important;float:right;margin:0 0 40px}
body#layout .header-wrapper{margin-top:40px}
body#layout #header,body#layout .header-right{width:50%}
body#layout .outer-wrapper,body#layout .sidebar-wrapper,body#layout .ct-wrapper{margin:0;padding:0}
body#layout .footer.section{float:left;width:33%}
.Header h1{margin:0;color:#000;font-size:30px;text-transform:uppercase;letter-spacing:-1px}
h1.title a{color:#000}
.titlewrapper{margin-top:7px}
.navbar-inverse{border-color:transparent;background:#222}
.navbar-inverse .navbar-nav>li>a{font-size:13px;margin:10px;padding:5px 1px 5px 0;text-transform:uppercase;color:#e4e4e4}
.navbar-inverse .navbar-nav>li>a:before{position:absolute;top:23px;bottom:0;left:0;width:0;height:1px;content:'';-webkit-transition:all ease .3s;transition:all ease .3s;opacity:0;background:#222}
.navbar-inverse .navbar-nav>li.current>a,.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#2196f3}
.navbar-inverse .navbar-nav>li.current>a:before,.navbar-inverse .navbar-nav>li>a:focus:before,.navbar-inverse .navbar-nav>li>a:hover:before{width:100%;opacity:1}
.navbar-inverse .navbar-nav.navbar-link-dark li a{color:#333}
.blog-post .post-meta h3 a:hover,.blog-post .post-meta h4 a:hover,.blog-post .post-meta h5 a:hover,.navbar-inverse .navbar-nav.navbar-link-dark li a:hover,.navbar.navbar-white li.current a,.portfolio-filter ul li .active,.portfolio-filter ul li a:hover{color:#2196f3}
.navbar-inverse.navbar-white{background:#fff;box-shadow:0 -2px 19px rgba(0,0,0,.1)}
.navbar-default .navbar-brand img,.navbar-inverse .navbar-brand img{height:40px;margin-top:0}
.navbar-brand{padding:5px 15px}
.navbar-fixed-top,.navbar-fixed-top.navbar-expanded{padding:15px 0;-webkit-transition:all .3s;transition:all .3s}
.navbar-fixed-top.navbar-expanded{padding:0}
.navbar-toggle{border-radius:0}
.navbar-default .navbar-toggle,.navbar-inverse .navbar-toggle{font-size:14px;padding:6px 10px;color:#fff}
.blog-post .post-meta h3 a,.blog-post .post-meta h4 a,.blog-post .post-meta h5 a,.navbar-white.navbar-inverse .navbar-toggle,.widget .widget-category li a{color:#222}
.navbar-white.navbar-inverse .navbar-toggle:focus,.navbar-white.navbar-inverse .navbar-toggle:hover{color:#fff}
@media (min-width: 768px) {
.navbar-default.navbar-expanded,.navbar-inverse.navbar-expanded{border:none;background:0 0}
.navbar-fixed-top.navbar-expanded{padding:30px 0;opacity:0;visibility:hidden}
.navbar-fixed-top.navbar-expanded.navbar-visible{padding:10px 0;opacity:1;background:#fff}
}
.hero{position:relative;display:table;width:100%;height:100%;padding:0;background:url(https://2.bp.blogspot.com/-cB43heSn8MM/WE1me6Wu5zI/AAAAAAAAA9A/Rjv5pvzuG2AYzawnUpIS_pt7tLgWGClugCLcB/s1600/9o1oq9szqzq-ben-white.jpg) no-repeat center bottom;background-attachment:fixed;background-size:cover}
.hero .hero-content.light-txt .hero-subtitle,.hero .hero-content.light-txt h1,.hero .hero-content.light-txt h2,.hero .hero-content.light-txt i{color:#fff}
.hero .hero-content.light-txt .button-bg{border-color:#2196f3!important;background:#2196f3}
.hero .hero-content.light-txt .button-bg:hover{color:#333!important;border-color:#fff!important;background:#fff}
.hero .hero-content.light-txt .button{color:#fff;border:1px solid #fff}
.hero .hero-content.light-txt .button:focus,.hero .hero-content.light-txt .button:hover{border-color:#2196f3}
.hero .hero-content{display:table-cell;-webkit-transform:translateY(-2.1rem);-ms-transform:translateY(-2.1rem);transform:translateY(-2.1rem);vertical-align:middle}
.hero .hero-content h1,.hero .hero-content h2,.video-banner h1,.video-banner h2{line-height:1.071;display:inline-block;margin-top:1rem;margin-bottom:2rem;text-shadow:none}
.hero .hero-content h1,.video-banner h1{font-weight:800;font-size:6.4rem}
@media (max-width: 480px) {
.hero .hero-content h1{font-size:4.4rem}
}
@media (max-width: 767px) {
.navbar-inverse .navbar-nav>li>a:before{display:none}
.Header h1{padding:0 15px}
.aisa-copyright,.aisa-right{text-align:center!important}
.contact-detail{padding:40px!important;padding-bottom:0!important}
}
@media screen and (max-width: 960px) {
.worksItem{width:100%!important}
.ct-wrapper{padding:0 15px}
.main-wrapper{margin-right:0;width:100%}
.sidebar-wrapper{float:none;width:auto!important}
}
.hero .hero-content h2,.video-banner h2{font-size:4.4rem}
.hero .hero-content h5{font-family:Raleway;font-size:2.3rem;line-height:1.565;margin-bottom:0}
.hero .hero-content .hero-subtitle{font-size:2.5rem;line-height:2.4rem;margin-bottom:3rem;font-family:Raleway;text-shadow:none}
.hero .hero-content .group-button{display:inline-block;margin-top:30px}
.hero .hero-content .group-button a{margin:0 10px}
@media (max-width: 380px) {
.hero .hero-content .group-button a{display:block;margin:10px}
}
.hero .hero-content .button-bg{color:#fff!important;border-color:#2196f3!important;background:#2196f3}
.hero .hero-content .button-bg:hover{color:#fff;border-color:#000!important;background:#000}
.hero .hero-content .button{font-size:1.3rem;line-height:5.4rem;height:6rem;margin-top:.6rem;padding:10px 30px;letter-spacing:.25rem;text-transform:uppercase;color:#000;border:1px solid #000;border-radius:40px}
@media (max-width: 480px) {
.hero .hero-content .button{line-height:3rem;height:5rem}
}
.hero .hero-content .button:focus,.hero .hero-content .button:hover{border-color:#2196f3}
.hero-short-banner{height:500px}
.hero-overlay{position:absolute;top:0;left:0;width:100%;height:100%;opacity:.3;background:#111}
.light-border-top-bottom{padding:10px 0;border-top:1px solid #fff;border-bottom:1px solid #fff}
.dark-border-top-bottom{padding:10px 0;border-top:1px solid #222;border-bottom:1px solid #222}
.go-down{font-size:3.3rem;position:absolute;bottom:7.2rem;left:0;display:block;width:100%;margin:0;padding:0}
.go-down .vertical-txt{font-size:1.8rem;position:absolute;z-index:2;right:1rem;bottom:50px;-webkit-transform:translate(50px,0) rotateZ(90deg);-ms-transform:translate(50px,0) rotate(90deg);transform:translate(50px,0) rotateZ(90deg);-webkit-transform-origin:0 0;-ms-transform-origin:0 0;transform-origin:0 0}
.go-down .vertical-txt:after{position:absolute;right:-35px;bottom:11px;width:27px;height:1px;content:'';background:#fff}
.go-down .vertical-txt.light-txt,.social-link li a:hover{color:#fff}
.go-down .vertical-txt.dark-txt{color:#000}
.go-down .vertical-txt.dark-txt:after{background:#000}
.go-down .mouse{position:absolute;top:50%;left:50%;width:26px;height:42px;-webkit-transform:translate(-50%,-50%);-ms-transform:translate(-50%,-50%);transform:translate(-50%,-50%);border:2px solid #fff;border-radius:26px;-webkit-backface-visibility:hidden}
.go-down .mouse:after{position:absolute;top:5px;left:50%;width:4px;height:4px;margin-left:-2px;content:'';-webkit-transform:translateY(0) scaleY(1) scaleX(1) translateZ(0);transform:translateY(0) scaleY(1) scaleX(1) translateZ(0);-webkit-animation:scroll 1.5s -1s cubic-bezier(.68,-.55,.265,1.55) infinite;animation:scroll 1.5s -1s cubic-bezier(.68,-.55,.265,1.55) infinite;opacity:1;border-radius:100%;background-color:#fff}
@-webkit-keyframes scroll {
0%,20%{-webkit-transform:translateY(0) scaleY(1) scaleX(1) translateZ(0);transform:translateY(0) scaleY(1) scaleX(1) translateZ(0)}
10%{-webkit-transform:translateY(0) scaleY(1.2) scaleX(1.2) translateZ(0);transform:translateY(0) scaleY(1.2) scaleX(1.2) translateZ(0);opacity:1}
to{-webkit-transform:translateY(20px) scaleY(2.5) scaleX(.5) translateZ(0);transform:translateY(20px) scaleY(2.5) scaleX(.5) translateZ(0);opacity:.01}
}
@keyframes scroll {
0%,20%{-webkit-transform:translateY(0) scaleY(1) scaleX(1) translateZ(0);transform:translateY(0) scaleY(1) scaleX(1) translateZ(0)}
10%{-webkit-transform:translateY(0) scaleY(1.2) scaleX(1.2) translateZ(0);transform:translateY(0) scaleY(1.2) scaleX(1.2) translateZ(0);opacity:1}
to{-webkit-transform:translateY(20px) scaleY(2.5) scaleX(.5) translateZ(0);transform:translateY(20px) scaleY(2.5) scaleX(.5) translateZ(0);opacity:.01}
}
@-webkit-keyframes blink {
0%,to{opacity:1}
50%{opacity:0}
}
@keyframes blink {
0%,to{opacity:1}
50%{opacity:0}
}
.typist-blink{font-weight:700;font-family:Open Sans}
.typist-blink:after{position:relative;top:6px;display:inline-block;height:30px;margin-right:7px;margin-left:3px;content:' ';-webkit-animation:blink 1s step-start 0 infinite;animation:blink 1s step-start 0 infinite;border-right:2px solid}
.typist-blink>.selectedText{display:none}
.typist-mark>.selectedText{font-style:normal;color:#fff;background-color:#222}
.social-link{margin:20px 0}
@media (max-width: 768px) {
.social-link{margin-bottom:30px}
}
.social-link a{line-height:33px;display:inline-block;width:35px;height:35px;margin:0 2px;text-align:center;color:#737373;border:1px solid #e4e4e4;border-radius:50%}
.social-link a:hover{color:#fff;border-color:#000;background:#000}
.dark-txt .social-link a{color:#333;border:1px solid #333}
.dark-txt .social-link a:hover{color:#fff;border-color:#000;background:#000}
[ripple]{z-index:1;position:relative;overflow:hidden}
[ripple] .ripple{position:absolute;background:#fff;width:15px;height:12px;border-radius:100%;-webkit-animation:ripple 1.6s;animation:ripple 1.6s}
@-webkit-keyframes ripple {
0%{-webkit-transform:scale(1);transform:scale(1);opacity:.2}
100%{-webkit-transform:scale(40);transform:scale(40);opacity:0}
}
@keyframes ripple {
0%{-webkit-transform:scale(1);transform:scale(1);opacity:.2}
100%{-webkit-transform:scale(40);transform:scale(40);opacity:0}
}
@-webkit-keyframes at-ripple {
0%{box-shadow:0 8px 10px rgba(102,102,102,0.1),0 0 0 0 rgba(102,102,102,0.1),0 0 0 5px rgba(102,102,102,0.1),0 0 0 10px rgba(102,102,102,0.1)}
100%{box-shadow:0 8px 10px rgba(102,102,102,0.1),0 0 0 5px rgba(102,102,102,0.1),0 0 0 10px rgba(102,102,102,0.1),0 0 0 20px rgba(102,102,102,0)}
}
@keyframes at-ripple {
0%{box-shadow:0 8px 10px rgba(102,102,102,0.1),0 0 0 0 rgba(102,102,102,0.1),0 0 0 5px rgba(102,102,102,0.1),0 0 0 10px rgba(102,102,102,0.1)}
100%{box-shadow:0 8px 10px rgba(102,102,102,0.1),0 0 0 5px rgba(102,102,102,0.1),0 0 0 10px rgba(102,102,102,0.1),0 0 0 20px rgba(102,102,102,0)}
}
.about-content .basic-info{padding-top:70px}
.about-content .basic-info .person-title{font-family:Raleway;font-weight:700;letter-spacing:-1px;line-height:48px;color:#282528;margin:0}
.about-content .basic-info .bio-text{font-weight:100;line-height:24px;color:#646464}
.about-content .basic-info .info-list{list-style-type:none;padding:0}
.about-content .basic-info .info-list li{color:#282528;font-weight:600;text-transform:capitalize}
.about-content .basic-info .info-list li i{font-size:24px;position:relative;top:5px;margin-right:7px;line-height:37px}
.profile-photo{padding-top:90px;text-align:center}
.profile-photo img{border-radius:70%;-webkit-border-radius:70%;width:310px;height:310px;object-fit:cover;-webkit-animation:at-ripple .6s linear infinite;animation:at-ripple .6s linear infinite}
.about-content .skills-info{padding-top:70px}
.about-content .skills-info .title{font-family:Raleway;font-weight:700;letter-spacing:-1px;line-height:48px;color:#282528;margin:0}
.about-content .skills-info .skill-text{margin-bottom:0;font-weight:100;line-height:24px;color:#646464}
.about-content .skills-info .single-bar{margin-bottom:20px}
.about-content .skills-info .single-bar span{color:#282528}
.about-content .skills-info .single-bar .skill-info{overflow:hidden;margin-bottom:10px}
.about-content .skills-info .single-bar .skill-title{float:left}
.about-content .skills-info .single-bar .skill-percent{float:right}
.about-content .skills-info .single-bar .progress{height:10px;margin-bottom:0;border-radius:0;box-shadow:0 0 0}
.about-content .skills-info .single-bar .progress .progress-bar{border-radius:0;box-shadow:0 0 0}
.about-content .basic-info .info-list li i{color:#2196f3}
.about-content .skills-info .single-bar .progress{border:0 solid #2196f3}
.about-content .skills-info .single-bar .progress .progress-bar{background:#2196f3}
#service{background:#f8f8f8;padding-top:40px;padding-bottom:20px}
.vc_row.wpb_row.vc_row-fluid.vc_custom_1460751314260.row{margin-top:40px}
.vc_custom_1460751314260{margin-bottom:0!important}
.vc_column_container{padding-left:0!important;padding-right:0!important}
@media (min-width: 768px) {
.vc_col-sm-4{width:33.33333333%}
.vc_col-sm-1,.vc_col-sm-10,.vc_col-sm-11,.vc_col-sm-12,.vc_col-sm-2,.vc_col-sm-3,.vc_col-sm-4,.vc_col-sm-5,.vc_col-sm-6,.vc_col-sm-7,.vc_col-sm-8,.vc_col-sm-9{float:left}
.vc_col-sm-12{width:100%}
}
.vc_col-lg-1,.vc_col-lg-10,.vc_col-lg-11,.vc_col-lg-12,.vc_col-lg-2,.vc_col-lg-3,.vc_col-lg-4,.vc_col-lg-5,.vc_col-lg-6,.vc_col-lg-7,.vc_col-lg-8,.vc_col-lg-9,.vc_col-md-1,.vc_col-md-10,.vc_col-md-11,.vc_col-md-12,.vc_col-md-2,.vc_col-md-3,.vc_col-md-4,.vc_col-md-5,.vc_col-md-6,.vc_col-md-7,.vc_col-md-8,.vc_col-md-9,.vc_col-sm-1,.vc_col-sm-10,.vc_col-sm-11,.vc_col-sm-12,.vc_col-sm-2,.vc_col-sm-3,.vc_col-sm-4,.vc_col-sm-5,.vc_col-sm-6,.vc_col-sm-7,.vc_col-sm-8,.vc_col-sm-9,.vc_col-xs-1,.vc_col-xs-10,.vc_col-xs-11,.vc_col-xs-12,.vc_col-xs-2,.vc_col-xs-3,.vc_col-xs-4,.vc_col-xs-5,.vc_col-xs-6,.vc_col-xs-7,.vc_col-xs-8,.vc_col-xs-9{position:relative;min-height:1px;padding-left:15px;padding-right:15px;-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}
.vc_column_container>.vc_column-inner{box-sizing:border-box;padding-left:15px;padding-right:15px;width:100%}
.service-box.style-2:last-child{border-bottom:0}
.service-box.style-2{padding-bottom:30px;border-bottom:1px solid #f6f6f6;margin-bottom:30px}
.service-box.style-2>i{display:inline-block;float:left;color:#22272c;font-size:38px;line-height:38px;-webkit-transition:all .3s;transition:all .3s;position:absolute}
.service-box.style-2 .service-box-content{margin-left:65px;font-family:Open Sans;font-weight:300;color:#7a7e82}
#service .row.vc_row-fluid{margin-bottom:0!important}
.service-box.style-2 .service-box-content h4{text-transform:uppercase;font-size:18px;line-height:30px;color:#22272c;font-weight:700;padding:0;margin:0!important}
.service-box.style-2 .service-box-content h4 b{color:#22272c}
.service-box.style-2 .service-box-content>:last-child{margin-bottom:0}
.vc_custom_1460841507827{margin-bottom:80px!important}
.headline{margin-bottom:30px;text-transform:uppercase}
.headline.text-center:after{margin:0 auto}
.headline h3{color:#3d464d;font-family:'Roboto Slab'!important;font-weight:300;margin:0;font-size:60px}
.text-center{text-align:center}
.service-box.style-2:hover > i,.service-box.style-2:hover .service-box-content h4 b{color:#2196f3;cursor:pointer}
.service-box-content h4 b{-webkit-transition:all .3s;transition:all .3s}
.parallax-funfactor{padding:100px 0;background-image:url(http://2.bp.blogspot.com/-KEtTHF6ylRI/VmcReg8JeCI/AAAAAAAAAmk/IoYID5sVz1c/s1600/parallax2.jpg)!important}
.parallax{position:relative;background:no-repeat center center scroll;background-attachment:fixed;background-size:cover}
.parallax:before{position:absolute;top:0;left:0;width:100%;height:100%;content:'';background:rgba(0,0,0,0.4)}
.parallax.light-overlay:before{position:absolute;top:0;left:0;width:100%;height:100%;content:'';background:rgba(255,255,255,.3)}
.fun-box i{font-size:40px;margin-bottom:20px}
.fun-box .value{font-size:50px;font-weight:700}
.fun-box .title{font-size:16px;text-transform:uppercase;font-weight:100}
@media (max-width: 991px) {
.fun-box{margin-bottom:30px}
}
.first_post_img{width:100%}
.big_post_image{margin:0}
.theme-img a{margin:0!important}
.post{margin:20px 0 0;padding:0 3% 20px}
.post-title{text-decoration:none;font-size:30px;line-height:normal;padding:0 0 10px}
.post-title a{text-decoration:none;color:#000}
.post-body{font-size:15px;padding:0;margin:0;line-height:29px;word-wrap:break-word;font-weight:100}
.post-header{color:#999;font-family:Verdana,Arial,Tahoma,sans-serif;font-size:12px}
.itemCaption:before{position:absolute;top:0;left:0;width:100%;height:100%;background:-webkit-linear-gradient(top,rgba(72,76,97,0) 0%,rgba(72,76,97,0.8) 75%);background:linear-gradient(to bottom,rgba(72,76,97,0) 0%,rgba(0,0,0,0.8) 75%);content:'';opacity:0;-webkit-transform:translate3d(0,50%,0);transform:translate3d(0,50%,0);-webkit-transition:opacity 0.35s,-webkit-transform .35s;transition:opacity 0.35s,transform .35s}
.itemCaption:hover h3{color:#fff;-webkit-transform:translate3d(0,-50%,0) translate3d(0,-40px,0);transform:translate3d(0,-50%,0) translate3d(0,-40px,0)}
.itemCaption:hover:before{opacity:1;-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}
.itemCaption:hover .capPreview{opacity:1;-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}
#single-header{position:relative;padding:30px 0;text-align:center;background:#191818}
h2#title2,#title3{font-weight:900;color:#fff;float:left;padding:15px;font-family:Raleway;text-transform:capitalize}
nav.navigation.post-navigation.hidden-xs{float:right}
.theme-img img{height:auto;max-width:100%}
.pagination{position:relative;width:100%}
.pagination>li:first-child>a,.pagination>li:first-child>span{border:0}
.pagination>li>a,.pagination>li>span{display:block;border:0;float:left;margin:4px 4px 4px 0;padding:2px 25px;text-decoration:none;width:auto;color:#fff;background:#0e0e0e;min-width:55px;min-height:35px;text-align:center;line-height:32px;border-radius:40px!important}
.single .pagination > li > a,.single .pagination > li > span,.mfp-content .pagination > li > a,.mfp-content .pagination>li>span{margin:0;color:#BCC2C9;background:none;line-height:normal;min-height:inherit}
.pagination span.page-of{float:right}
.pagination>li>a:hover,.pagination>li>a:focus,.pagination>.active>a,.pagination>.active>span{color:#000;background:#fff}
.single .pagination > li > a:hover,.single .pagination > li > a:focus,.single .pagination > .active > a,.single .pagination>.active>span{color:#F36639;background:none}
.pagination .current,.pagination span.page-of{background:#F36639;color:#fff}
.single .pagination .current,.single .pagination span.page-of{color:#F36639;background:none}
a.scrollup{bottom:20px;height:42px;position:fixed;right:20px;width:42px;background:#F36639;line-height:47px;text-align:center;z-index:999}
.quoute{background:#2196f3}
.quoute-content .quoute-link:hover{color:#2196f3}
.quoute-content h1{color:#fff;font-weight:600}
.quoute-content p{color:#fff;font-weight:400;margin-top:10px}
.quoute-content .quoute-link{float:right;color:#fff;border:3px solid #fff;padding:10px 25px;font-weight:600;border-radius:50px;margin-top:35px;transition:.4s}
.quoute-content .quoute-link:hover{background:#fff}
#blog-pager{padding:1em 0 0;margin:0;line-height:normal;display:inline-block;width:100%;text-align:center}
.home-link{display:none}
#blog-pager-newer-link{float:right;text-decoration:none;background:#000;font-size:16px;font-family:sans-serif;padding:10px;font-weight:700;position:relative;left:-20px;top:8px}
#blog-pager-older-link{text-decoration:none;font-size:16px;font-family:sans-serif;font-weight:700;float:left;background:#000;padding:10px;margin-left:20px;margin-top:8px}
#blog-pager-newer-link a{text-decoration:none;color:#FFF}
#blog-pager-older-link a{text-decoration:none;color:#FFF}
.showpageOf{display:none}
.showpageNum a,.showpage a{margin:0 4px}
.showpagePoint{margin:0 2px 0 0}
.PopularPosts h2{padding-right:.4em;padding-left:0}
.popular-posts ul{padding:10px 0 0;margin:0}
.popular-posts ul li{list-style:none outside none!important;margin-left:0!important;overflow:hidden;padding:7px 0!important;-webkit-transition:all .25s linear 0;-moz-transition:all .25s linear 0;-o-transition:all .25s linear 0;transition:all .25s linear 0}
.PopularPosts .item-title a{font-size:15px;line-height:24px;display:block;margin-bottom:10px;font-weight:700;color:#252525;margin-left:110px;margin-top:5px}
.PopularPosts a{color:#666;font-size:.9rem;line-height:normal;text-decoration:none}
.PopularPosts a:hover{color:#3FA9F5!important}
.PopularPosts img{padding-right:0;height:95px;width:100px;object-fit:cover;-moz-border-radius:3px;-webkit-border-radius:3px;border-radius:3px}
.PopularPosts .item-thumbnail{width:100px;float:left}
.list-label-widget-content li{margin:0!important}
.cloud-label-widget-content .label-size{background-color:#F1F1F1;color:#a7a7a7!important;margin:0 7px 7px 0;display:block;float:left;padding:2px 11px;font-size:12px!important;-moz-border-radius:3px;-webkit-border-radius:3px;border-radius:3px;line-height:25px}
.cloud-label-widget-content{text-align:initial;margin-top:10px}
.cloud-label-widget-content .label-size a{color:#a7a7a7!important}
.cloud-label-widget-content .label-size:hover{background-color:#2196f3!important;color:#fff!important}
.label-size:hover.label-size a{color:#fff!important}
.list-label-widget-content li{display:block;padding:5px 0!important;border-bottom:1px solid #f3f3f3;position:relative;text-align:left}
.list-label-widget-content li:last-child{border:0;margin:0;padding-bottom:0!important}
.list-label-widget-content li a:before{content:'\203a';position:absolute;left:0;top:-3px;font-size:22px;margin-left:7px;color:rgba(1,1,1,0.7)}
.list-label-widget-content li a{color:#010101;font-size:12px;padding-left:20px;font-weight:400;text-transform:uppercase}
.list-label-widget-content li a:hover{color:#2196f3}
.list-label-widget-content li span:last-child{color:rgba(0,0,0,0.31);font-size:28px;font-weight:700;position:absolute;top:5px;right:0;opacity:.3}
.Profile img{border:1px solid #cecece;background:#fff;float:left;margin:5px 10px 5px 0;padding:5px;-webkit-border-radius:50px;-moz-border-radius:50px;border-radius:50px}
.profile-data{color:#999;font:bold 20px/1.6em Arial,Helvetica,Tahoma,sans-serif;font-variant:small-caps;margin:0;text-transform:capitalize}
.profile-datablock{margin:.5em 0}
.profile-textblock{line-height:1.6em;margin:.5em 0}
a.profile-link{clear:both;display:block;font:80% monospace;padding:10px 0;text-align:center;text-transform:capitalize}
.showpageArea a{text-decoration:underline}
.showpageNum a{background-color:#333;color:#fff;display:inline-block;position:relative;cursor:pointer;outline:none;white-space:nowrap;margin:2px;color:#FFF;font-size:14px;font-family:Open Sans;padding:0 12px;font-weight:700;line-height:36px;background:#333;border:none;text-shadow:1px 1px 1px rgba(0,0,0,0.3);border-radius:3px;-moz-border-radius:3px;-webkit-border-radius:3px;transition:background-color .2s linear;-moz-transition:background-color .2s linear;-webkit-transition:background-color .2s linear;-ms-transition:background-color .2s linear;-o-transition:background-color .2s linear}
.showpagePoint:hover,.showpageNum a:hover,.showpage a:hover{background-color:#2196f3;color:#fff}
.showpagePoint{background-color:#333;color:#fff;display:inline-block;position:relative;cursor:pointer;outline:none;white-space:nowrap;margin:2px;color:#FFF;font-size:14px;font-family:Open Sans;padding:0 12px;font-weight:700;line-height:36px;background:#333;border:none;text-shadow:1px 1px 1px rgba(0,0,0,0.3);border-radius:3px;-moz-border-radius:3px;-webkit-border-radius:3px;transition:background-color .2s linear;-moz-transition:background-color .2s linear;-webkit-transition:background-color .2s linear;-ms-transition:background-color .2s linear;-o-transition:background-color .2s linear}
.showpageOf{text-decoration:none;padding:3px;margin:0 3px 0 0;font-size:15px margin: 0 3px}
.showpage a{background-color:#333;color:#fff;display:inline-block;position:relative;cursor:pointer;outline:none;white-space:nowrap;margin:2px;color:#FFF;font-size:14px;font-family:Open Sans;padding:0 12px;font-weight:700;line-height:36px;background:#333;border:none;text-shadow:1px 1px 1px rgba(0,0,0,0.3);border-radius:3px;-moz-border-radius:3px;-webkit-border-radius:3px;transition:background-color .2s linear;-moz-transition:background-color .2s linear;-webkit-transition:background-color .2s linear;-ms-transition:background-color .2s linear;-o-transition:background-color .2s linear}
.showpage a:hover{text-decoration:none}
.showpageNum a:link,.showpage a:link{text-decoration:none}
.showpageOf{display:none}
.showpageArea{padding-bottom:20px}
.status-msg-wrap{text-align:center;padding:17px;color:#6F6B6B;margin-bottom:25px;text-transform:capitalize;border:1px solid #ddd}
.status-msg-border{display:none}
.sidebar{margin:0;padding:0;display:block}
.sidebar h2{padding:0 0 13px;margin:0;line-height:1;font-size:16px;text-transform:capitalize;color:#191818;border-bottom:1px solid #f4f4f4;position:relative;text-align:left;letter-spacing:-.5px}
.sidebar h2:before{position:absolute;content:" ";z-index:1;bottom:-1px;left:0;width:80px;height:1px;background-color:#3FA9F5!important}
.sidebar .widget{color:#BCC2C9;margin-bottom:30px;float:left;width:100%;background:#fff;padding:20px;-webkit-border-radius:3px;-moz-border-radius:3px;border-radius:3px}
.sidebar ul{margin:0;padding:0;list-style:none}
.sidebar li{margin:0 0 0 15px;padding:0 0 5px;text-transform:capitalize}
#comments{padding:0 20px;display:inline-block;width:100%;background:#fff}
#comments > h4{padding:0 0 15px;margin:0;line-height:1;font-size:14px;text-transform:uppercase;color:#50514f;border-bottom:1px solid #f4f4f4;position:relative;text-align:left;padding-top:20px}
#comments > h4:before{position:absolute;content:" ";z-index:1;bottom:-1px;left:0;width:80px;height:1px;background-color:#3FA9F5!important}
.c_msg_p{font-size:12px;padding:5px}
#comments #comment-post-message{color:#FFF;background:#3FA9F5!important;margin:0;padding:10px;line-height:normal;border-radius:2px;font-size:15px}
#comments .user a{color:#555;font-style:normal;font-size:16px;line-height:26px;font-weight:400;letter-spacing:1px}
#comments .datetime,#comments .datetime a{color:#999;text-decoration:none;margin:0;font-size:14px;display:inline-block;float:right}
.comments .comments-content .comment-content{margin:0 0 20px;color:#7B7B7B}
#comments .datetime a{margin:auto}
#comments .comment-actions a{background-color:#3FA9F5!important;border:1px solid #3FA9F5!important;border-radius:2px;color:#FFF;font-size:11px;padding:5px 15px;text-transform:uppercase;text-decoration:none;margin-right:10px}
#comments .comment-actions a:hover{color:#fff;background-color:#555;border:1px solid #555}
#comments .comment{border-bottom:1px solid #eee;padding:0 0 5px}
#comments .loadmore{margin-top:0}
#comment-editor{height:235px}
.comments .comments-content .avatar-image-container{max-height:76px;width:76px}
#comments .comments-content .avatar-image-container img{max-width:70px;width:100%;border-radius:205px}
.comments .comment-block{margin-left:90px!important}
span.icon.user.blog-author:after{background-color:#3FA9F5!important;color:#FFF;padding:2px 5px;font-weight:400;font-size:13px;content:"Admin";display:inline-block}
.thread-toggle{display:block!important}
.thread-toggle.thread-expanded{border-bottom:1px solid #ddd;width:100%;padding:0 0 10px;margin-bottom:10px}
#comments .thread-chrome .comment{border-bottom-color:#ddd!important}
#comments .comment-author{padding-left:25px}
.comment-body{margin:.5em 25px}
.comment-footer{margin:.5em 25px 1.5em}
.comment-body p{margin:0}
#comments .avatar-comment-indent .comment-author{margin-left:-45px;padding-left:45px}
.deleted-comment{font-style:italic;opacity:.5}
#comment-actions{background:transparent;border:0;padding:0;position:absolute;height:25px}
#comments .blogger-comment-icon,.blogger-comment-icon{line-height:16px;background:url(/img/b16-rounded.gif) left no-repeat;padding-left:20px}
#comments .openid-comment-icon,.openid-comment-icon{line-height:16px;background:url(/img/openid16-rounded.gif) left no-repeat;padding-left:20px}
#comments .anon-comment-icon,.anon-comment-icon{line-height:16px;background:url(/img/anon16-rounded.gif) left no-repeat;padding-left:20px}
.comment-form{clear:both;_width:410px}
.comment-link{white-space:nowrap}
.paging-control-container{float:right;margin:0 6px 0 0;font-size:80%}
.unneeded-paging-control{visibility:hidden}
#comments-block .avatar-image-container img{-ms-interpolation-mode:bicubic;border:1px solid #ccc;float:right}
#comments-block .avatar-image-container.avatar-stock img{border-width:0;padding:1px}
#comments-block .avatar-image-container{height:37px;left:-45px;position:absolute;width:37px}
#comments-block.avatar-comment-indent{margin-left:45px;position:relative}
#comments-block.avatar-comment-indent dd{margin-left:0}
iframe.avatar-hovercard-iframe{border:0 none;padding:0;width:25em;height:9.4em;margin:.5em}
.comments{clear:both;margin-top:10px;margin-bottom:0}
.comments .comments-content{margin-bottom:16px}
.comments .comment .comment-actions a{padding-right:5px;padding-top:5px}
.comments .comment .comment-actions a:hover{text-decoration:underline}
.comments .comments-content .comment-thread ol{list-style-type:none;padding:0;text-align:left;list-style-position:inside}
.comments .comments-content .inline-thread{padding:.5em 1em}
.comments .comments-content .comment-thread{margin:8px 0}
.comments .comments-content .comment-thread:empty{display:none}
.comments .comments-content .comment-replies{margin-left:36px;margin-top:1em}
.comments .comments-content .comment{margin-bottom:16px;padding-bottom:8px}
.comments .comments-content .comment:first-child{padding-top:16px}
.comments .comments-content .comment:last-child{border-bottom:0;padding-bottom:0}
.comments .comments-content .comment-body{position:relative}
.comments .comments-content .user{font-style:normal;font-weight:700}
.comments .comments-content .icon.blog-author{display:inline-block;height:18px;margin:0 0 -4px 6px;width:inherit}
.comments .comments-content .datetime{margin-left:6px}
.comments .comments-content .comment-header,.comments .comments-content .comment-content{margin:0 0 8px}
.comments .comments-content .comment-content{text-align:justify}
.comments .comments-content .owner-actions{position:absolute;right:0;top:0}
.comments .comments-replybox{border:none;height:250px;width:100%}
.comments .comment-replybox-single{margin-left:48px;margin-top:5px}
.comments .comment-replybox-thread{margin-top:5px}
.comments .comments-content .loadmore a{display:block;padding:10px 16px;text-align:center}
.comments .thread-toggle{cursor:pointer;display:inline-block;border:1px solid #ddd;width:100%;padding:10px;margin-bottom:10px}
.comments .continue{cursor:pointer}
.comments .continue a{background-color:#3FA9F5!important;border:1px solid #3FA9F5!important;color:#fff!important;border-radius:2px;color:#FFF;font-size:11px;display:inline-block;padding:10px 20px;text-transform:uppercase;text-decoration:none;margin-right:10px}
.comments .comments-content .loadmore{cursor:pointer;margin-top:3em;max-height:3em}
.comments .comments-content .loadmore.loaded{max-height:0;opacity:0;overflow:hidden}
.comments .thread-chrome.thread-collapsed{display:none}
.comments .thread-toggle{display:inline-block}
.comments .thread-toggle .thread-arrow{display:inline-block;height:8px;margin:.3em;overflow:visible;padding-right:4px;width:10px;top:3px;position:relative}
.comments .thread-expanded .thread-arrow{background:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAcAAAAHCAYAAADEUlfTAAAAG0lEQVR42mNgwAfKy8v/48I4FeA0AacVDFQBAP9wJkE/KhUMAAAAAElFTkSuQmCC) no-repeat scroll 0 0 transparent}
.comments .thread-collapsed .thread-arrow{background:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAcAAAAHCAYAAADEUlfTAAAAJUlEQVR42mNgAILy8vL/DLgASBKnApgkVgXIkhgKiNKJ005s4gDLbCZBiSxfygAAAABJRU5ErkJggg==) no-repeat scroll 0 0 transparent}
.comments .avatar-image-container{float:left;max-height:36px;overflow:hidden;width:36px}
.comments .avatar-image-container img{max-width:36px}
.comments .comment-block{margin-left:48px;position:relative}
@media screen and (max-device-width: 480px) {
.comments .comments-content .comment-replies{margin-left:0}
}
a.quickedit{display:none}
@media screen and (max-width: 960px) {
.ct-wrapper{padding:0 15px}
.main-wrapper{margin-right:0;width:100%}
.sidebar-wrapper{float:left;width:auto;margin-left:20px}
}
@media screen and (max-width: 768px) {
#comment-editor{margin:10px}
.footer{width:50%}
}
@media screen and (max-width: 420px) {
.comments .comments-content .datetime{display:block;float:none}
.comments .comments-content .comment-header{height:70px}
}
@media screen and (max-width: 320px) {
.footer{width:100%}
.ct-wrapper{padding:0}
.comments .comments-content .comment-replies{margin-left:0}
}
h2.date-header,a.navbar-brand{display:none}
section#contact{background:#fff}
.bottom-thing{width:100%;display:inline-block}
.contact-content{padding-top:40px}
.contact-form .ct-form .form-group{margin-bottom:20px}
.contact-form .ct-form .form-group .form-control{border:0;box-shadow:0 0 0;border:1px solid #333;border-radius:0;-moz-border-radius:0;-webkit-border-radius:0;transition:.4s;background:#fff!important;font-weight:300;font-size:14px;padding:20px;position:relative;padding-left:40px!important;font-weight:400;color:#282528;vertical-align:middle}
.contact-form .ct-form .form-group{position:relative}
.contact-form .ct-form .form-group .icon{font-size:24px;color:#282528;position:absolute;top:9px;z-index:5;left:10px}
.contact-form .ct-form .form-group .icon.left-b{left:35px}
.contact-form .ct-form .form-group .form-control:focus,.contact-form .ct-form .form-group .form-control:active{padding-left:70px}
.contact-form .ct-form .form-group textarea{background:transparent!important;resize:none;padding:20px;padding-top:5px;height:130px;padding-top:12px!important}
.contact-form .ct-form .post-btn,#ContactForm1_contact-form-submit{background:transparent;padding:10px 25px;color:#282528!important;font-weight:400;display:inline-block;border-radius:0;border:1px solid #282528;border-radius:50px;transition:.4s;outline:0}
.contact-form .ct-form .post-btn:hover,#ContactForm1_contact-form-submit:hover{background:#282528!important;color:#fff!important}
.contact-form .ct-form .form-group .form-control::-webkit-input-placeholder{color:#282528}
.contact-form .ct-form .form-group .form-control:-moz-placeholder{color:#282528;opacity:1}
.contact-form .ct-form .form-group .form-control::-moz-placeholder{color:#282528;opacity:1}
.contact-form .ct-form .form-group .form-control:-ms-input-placeholder{color:#282528}
.contact-form .ct-form .form-group .form-control::-ms-input-placeholder{color:#282528}
.contact-form .ct-form .form-group .form-control:placeholder-shown{color:#282528}
p#ContactForm1_contact-form-error-message{width:100%;color:#c11717;text-align:center}
p#ContactForm1_contact-form-success-message{width:100%;color:#17c12d;text-align:center}
.contact-detail{padding:0}
.single-contact-detail{margin-bottom:30px;padding:0}
.single-contact-detail .header i{font-size:30px;float:left;margin-right:10px}
.single-contact-detail .header h5{margin:0 0 20px;font-weight:700;padding:5px 0 0}
.single-contact-detail p{color:#646464;font-weight:400;line-height:30px;margin-top:10px}
.single-contact-detail p br{margin-bottom:0}
.single-contact-detail .header i{color:#2196f3}
.contact-i{left:23px!important}
.aisa-right{text-align:right}
.aisa-copyright a{color:#2196f3}
.aisa-copyright{padding:30px 0;font-size:12px;position:relative;z-index:10;background:#f8f8f8;color:#636363}
#go-top{line-height:60px;position:fixed;z-index:100;right:3%;bottom:0;width:50px;height:60px;-webkit-transition:all .3s;transition:all .3s;text-align:center;color:#fff;background:rgba(0,0,0,.6)}
#go-top:hover{background:#2196f3}
.go-top-show{-webkit-transform:translateY(0);-ms-transform:translateY(0);transform:translateY(0);opacity:1;filter:alpha(opacity=100)}
.go-top-hide{-webkit-transform:translateY(40px);-ms-transform:translateY(40px);transform:translateY(40px);opacity:0;filter:alpha(opacity=0)}
]]></b:skin>

  <b:template-skin><![CDATA[
body#layout{background-color:#F7F7F7}
body#layout ul,body#layout li{list-style:none;padding:0}
body#layout .editlink{border:1px solid;border-radius:2px;padding:5px 10px;line-height:normal;border-color:#fd7347;color:#fd7347!important}
#layout:before{content:'Made With ❤  By Themeswear.com';width:101%;display:inline-block;background:#fd7347;color:#fff;padding:15px 0;margin:-1px 0 0 -1px;font-family:monospace;top:0;position:absolute;left:0}
#layout:after{content:'Thanks For Downloading :)';width:101%;display:inline-block;background:#464543;color:#fff;padding:15px 0;margin:-1px 0 0 -1px;font-family:monospace;position:absolute;left:0}
body#layout .header-content{margin:20px 0 35px}
body#layout div#header{width:55%;float:left;z-index:999;margin-top:25px}
body#layout div#header-social{width:34%;display:inline-block}
body#layout .section h4{background:#fd7347;color:#fff;padding:15px;margin:0;text-transform:capitalize}
body#layout div#content{width:55%;z-index:99;float:left}
body#layout div#sidebar{width:34%;display:inline-block}
body#layout footer{width:100%;display:inline-block}
body#layout header:before{content:"Header Area";background:#fd7347;padding:10px 80px;color:#fff;font-family:monospace;z-index:999999;border-radius:20px;border:1px solid #fff;border-right:0;border-left:0}
body#layout .content-wrapper:before{content:"Content Area";background:#fd7347;padding:10px 80px;color:#fff;font-family:monospace;z-index:999999;border-radius:20px;border:1px solid #fff;border-right:0;border-left:0;position:relative;top:-25px}
body#layout section#aboutus,body#layout section#team,body#layout section#our_skills,body#layout section#achievements,body#layout div#creativity,body#layout div#main-navbar-collapse,body#layout div#services,body#layout div#blog,body#layout div#blog,body#layout div#contact{display:none}
body#layout #about,body#layout #service,body#layout .parallax-funfactor,body#layout .quoute,body#layout #contact{display:none}
]]></b:template-skin>

  <!-- Style For Post -->
  <b:if cond='data:blog.pageType == &quot;item&quot;'>
    <style>
      .s-post-body{width:100%!important;padding:30px;padding-top:40px;background:#fff;margin-bottom:30px;-webkit-border-radius:3px;-moz-border-radius:3px;border-radius:3px;z-index:9}
      .padding_post{padding:0!important}
      .pagination{margin:27px 0 0;float:none;display:inline-block;width:auto}
      .pagination&gt;li&gt;a:hover,.pagination&gt;li&gt;a:focus,.pagination&gt;.active&gt;a,.pagination&gt;.active&gt;span{color:#000;background:$(body.background.color)!important}
      a.home-link{-webkit-border-radius:3px;-moz-border-radius:3px;border-radius:3px}
      .outer-wrapper{padding-bottom:65px;padding-top:35px}
      ul.list-inline.post-tags li{border:0!important;padding:0 5px!important}
      ul.list-inline.post-tags li a{color:#f36639!important;font-size:10px!important}
      footer.entry-meta{margin-top:15px!important;margin-right:-30px!important;margin-left:-30px!important;border-top:1px solid #f5f5f5!important;padding:12px!important}
      .btn{color:#fff!important;font-size:13px;font-weight:400;letter-spacing:.5px;position:relative;border:0 solid #e2e2e2;padding:7px 15px;transition:.2s ease-in;border-radius:0;margin:5px 10px;outline:0}
      .btn:hover{border-color:#000!important;background:#000}
      .tw-green{background-color:#4CAF50;color:#fff;border-color:#4CAF50}
      .btn.tw-green:hover{background-color:#44cc49;border-color:#44cc49!important}
      .btn.focus,.btn:focus,.btn:hover{color:#fff!important;text-decoration:none}
      .tw-red{background-color:#F44336;color:#fff;border-color:#F44336}
      .btn.tw-red:hover{background-color:#ff1200;border-color:#ff1200!important}
      .header .navbar{border-bottom:1px solid #eee;background:#fff;opacity:1;visibility:visible;padding:10px}
      body{background:#f5f5f5}
    </style>
  </b:if>
  <!-- Style For Post End-->
  <!-- Style For Page -->
  <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
    <style>
      .s-post-body{width:100%!important;padding:30px;padding-top:40px;background:#fff;margin-bottom:30px;-webkit-border-radius:3px;-moz-border-radius:3px;border-radius:3px;z-index:9}
      .main-wrapper{margin:0!important}
      .padding_post{padding:0!important}
      .pagination{margin:27px 0 0;float:none;display:inline-block;width:auto}
      .pagination&gt;li&gt;a:hover,.pagination&gt;li&gt;a:focus,.pagination&gt;.active&gt;a,.pagination&gt;.active&gt;span{color:#000;background:$(body.background.color)!important}
      a.home-link{-webkit-border-radius:3px;-moz-border-radius:3px;border-radius:3px}
      .outer-wrapper{padding-bottom:65px;padding-top:50px}
      ul.list-inline.post-tags li{border:0!important;padding:0 5px!important}
      ul.list-inline.post-tags li a{color:#f36639!important;font-size:10px!important}
      footer.entry-meta{margin-top:15px!important;margin-right:-30px!important;margin-left:-30px!important;border-top:1px solid #f5f5f5!important;padding:12px!important}
      .sidebar-wrapper{display:none}
      .header .navbar{border-bottom:1px solid #eee;background:#fff;opacity:1;visibility:visible;padding:10px}
      body{background:#f5f5f5}
    </style>
  </b:if>
  <!-- Style For Page End -->
  <!-- Style For Home & Index -->
  <b:if cond='data:blog.pageType != &quot;item&quot;'>
    <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
      <style>
        .ct-wrapper{padding:0}
        .outer-wrapper,#content{background:transparent;border:0}
        .main-wrapper{margin:0}
        .sidebar-wrapper{display:none}
        #worksGrid{display:table}
        #portfolio{background:#fff}
        .worksItem{padding:0;overflow:hidden;height:auto;text-align:center;position:relative;float:left;width:31.333%;max-height:360px;margin:10px;background:#000;cursor:pointer}
        .worksItem img{width:100%;height:275px;-webkit-transition:all .25s ease-out;transition:all .25s ease-out;object-fit:cover;position:relative;display:block;min-height:100%;max-width:100%;opacity:.7}
        .worksItem .itemCaption{padding:2em;color:#fff;text-transform:uppercase;font-size:1.25em;-webkit-backface-visibility:hidden;backface-visibility:hidden;position:absolute;top:0;left:0;width:100%;height:100%}
        .itemCaption h3{position:absolute;top:50%;left:0;width:100%;color:#484c61;-webkit-transition:-webkit-transform 0.35s,color .35s;transition:transform 0.35s,color .35s;-webkit-transform:translate3d(0,-50%,0);transform:translate3d(0,-50%,0);margin:0;padding:0 30px}
        .capContent{padding-top:15%;opacity:0;margin-top:25px;-webkit-transition:all .2s linear;transition:all .2s linear;-moz-transition:all .2s linear;-o-transition:all .2s linear}
        .capPreview{color:#fff!important;text-transform:uppercase;font-size:10px;letter-spacing:3px;padding:8px 10px;margin-top:10px;text-align:center;position:absolute;bottom:0;left:0;padding:1em;width:100%;opacity:0;-webkit-transform:translate3d(0,10px,0);transform:translate3d(0,10px,0);-webkit-transition:opacity 0.35s,-webkit-transform .35s;transition:opacity 0.35s,transform .35s}
        .worksItem:hover .capContent{opacity:1;padding-top:20%}
        .post-title a{text-decoration:none;color:#FFF!important;text-align:center;font-family:Raleway;font-weight:700}
        .post-footer,.post-related{display:none}
        .body{background:#f5f5f5}
      </style>
    </b:if></b:if>
  <!-- Style For Home & Index End -->
  <!-- JS For Home -->
  <script type='text/javascript'>
    /*&lt;![CDATA[*/
    // JavaScript Document
var _0x565e=["\x67\x65\x74\x45\x6C\x65\x6D\x65\x6E\x74\x42\x79\x49\x64","","\x69\x6D\x67","\x67\x65\x74\x45\x6C\x65\x6D\x65\x6E\x74\x73\x42\x79\x54\x61\x67\x4E\x61\x6D\x65","\x6C\x65\x6E\x67\x74\x68","\x3C\x69\x6D\x67\x20\x73\x72\x63\x3D\x22","\x73\x72\x63","\x22\x20\x2F\x3E","\x69\x6E\x6E\x65\x72\x48\x54\x4D\x4C","\x3C\x64\x69\x76\x20\x63\x6C\x61\x73\x73\x3D\x22\x69\x74\x65\x6D\x43\x61\x70\x74\x69\x6F\x6E\x22\x3E\x3C\x64\x69\x76\x20\x63\x6C\x61\x73\x73\x3D\x22\x63\x61\x70\x43\x6F\x6E\x74\x65\x6E\x74\x22\x3E\x3C\x68\x33\x20\x63\x6C\x61\x73\x73\x3D\x22\x70\x6F\x73\x74\x2D\x74\x69\x74\x6C\x65\x20\x65\x6E\x74\x72\x79\x2D\x74\x69\x74\x6C\x65\x22\x20\x69\x74\x65\x6D\x70\x72\x6F\x70\x3D\x22\x6E\x61\x6D\x65\x22\x3E\x3C\x61\x20\x68\x72\x65\x66\x3D\x22","\x22\x3E","\x3C\x2F\x61\x3E\x3C\x2F\x68\x33\x3E\x3C\x61\x20\x63\x6C\x61\x73\x73\x3D\x22\x63\x61\x70\x50\x72\x65\x76\x69\x65\x77\x20\x69\x6D\x61\x67\x65\x2D\x6D\x6F\x64\x61\x6C\x22\x20\x68\x72\x65\x66\x3D\x22","\x22\x3E\x52\x65\x61\x64\x20\x4D\x6F\x72\x65\x3C\x2F\x61\x3E\x3C\x2F\x64\x69\x76\x3E\x3C\x2F\x64\x69\x76\x3E","\x6F\x6E\x6C\x6F\x61\x64","\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72","\x68\x72\x65\x66","\x6C\x6F\x63\x61\x74\x69\x6F\x6E","\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x2E\x63\x6F\x6D\x2F","\x73\x65\x74\x41\x74\x74\x72\x69\x62\x75\x74\x65","\x72\x65\x66","\x64\x6F\x66\x6F\x6C\x6C\x6F\x77","\x74\x69\x74\x6C\x65","\x50\x6F\x72\x74\x66\x6F\x6C\x69\x6F\x20\x42\x6C\x6F\x67\x67\x65\x72\x20\x54\x65\x6D\x70\x6C\x61\x74\x65\x73","\x73\x74\x79\x6C\x65","\x64\x69\x73\x70\x6C\x61\x79\x3A\x20\x69\x6E\x6C\x69\x6E\x65\x2D\x62\x6C\x6F\x63\x6B\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x66\x6F\x6E\x74\x2D\x73\x69\x7A\x65\x3A\x20\x69\x6E\x68\x65\x72\x69\x74\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x63\x6F\x6C\x6F\x72\x3A\x20\x23\x32\x31\x39\x36\x66\x33\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x76\x69\x73\x69\x62\x69\x6C\x69\x74\x79\x3A\x20\x76\x69\x73\x69\x62\x6C\x65\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x6F\x70\x61\x63\x69\x74\x79\x3A\x20\x31\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B","\x23\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x3A\x76\x69\x73\x69\x62\x6C\x65"];var _0x1a25=[_0x565e[0],_0x565e[1],_0x565e[2],_0x565e[3],_0x565e[4],_0x565e[5],_0x565e[6],_0x565e[7],_0x565e[8],_0x565e[9],_0x565e[10],_0x565e[11],_0x565e[12],_0x565e[13],_0x565e[14],_0x565e[15],_0x565e[16],_0x565e[17],_0x565e[18],_0x565e[19],_0x565e[20],_0x565e[21],_0x565e[22],_0x565e[23],_0x565e[24],_0x565e[25]];function rm(_0xaff3x3){var _0xaff3x4=document[_0x1a25[0]](_0xaff3x3);imgtag= _0x1a25[1];img= _0xaff3x4[_0x1a25[3]](_0x1a25[2]);if(img[_0x1a25[4]]&gt;= 1){imgtag= _0x1a25[5]+ img[0][_0x1a25[6]]+ _0x1a25[7]}else {imgtag= _0x1a25[1]};_0xaff3x4[_0x1a25[8]]= imgtag+ _0x1a25[9]+ y+ _0x1a25[10]+ x+ _0x1a25[11]+ y+ _0x1a25[12]}window[_0x1a25[13]]= function(){var _0xaff3x5=document[_0x1a25[0]](_0x1a25[14]);if(_0xaff3x5== null){window[_0x1a25[16]][_0x1a25[15]]= _0x1a25[17]};_0xaff3x5[_0x1a25[18]](_0x1a25[15],_0x1a25[17]);_0xaff3x5[_0x1a25[18]](_0x1a25[19],_0x1a25[20]);_0xaff3x5[_0x1a25[18]](_0x1a25[21],_0x1a25[22]);_0xaff3x5[_0x1a25[18]](_0x1a25[23],_0x1a25[24]);_0xaff3x5[_0x1a25[8]]= _0x1a25[22];setInterval(function(){if(!$(_0x1a25[25])[_0x1a25[4]]){window[_0x1a25[16]][_0x1a25[15]]= _0x1a25[17]}},3000)}
    /*]]&gt;*/</script>

  <b:if cond='data:blog.pageType == &quot;item&quot;'>
    <script>
      //<![CDATA[
var _0x7ba7=["\x73\x72\x63","\x61\x74\x74\x72","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x6D\x67","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x66\x72\x61\x6D\x65","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x66\x72\x61\x6D\x65\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x6D\x67","\x2E\x62\x69\x67\x5F\x70\x6F\x73\x74\x5F\x69\x6D\x61\x67\x65","\x61\x70\x70\x65\x6E\x64\x54\x6F","\x3C\x63\x65\x6E\x74\x65\x72\x3E\x3C\x69\x6D\x67\x20\x73\x72\x63\x3D\x22","\x22\x20\x63\x6C\x61\x73\x73\x3D\x22\x66\x69\x72\x73\x74\x5F\x70\x6F\x73\x74\x5F\x69\x6D\x67\x22\x2F\x3E\x3C\x2F\x63\x65\x6E\x74\x65\x72\x3E","\x72\x65\x6D\x6F\x76\x65","\x66\x69\x72\x73\x74","\x3C\x63\x65\x6E\x74\x65\x72\x20\x63\x6C\x61\x73\x73\x3D\x22\x69\x66\x72\x61\x6D\x65\x5F\x77\x72\x61\x70\x70\x65\x72\x22\x3E\x3C\x69\x66\x72\x61\x6D\x65\x20\x73\x72\x63\x3D\x22","\x22\x20\x63\x6C\x61\x73\x73\x3D\x22\x69\x66\x72\x61\x6D\x65\x5F\x76\x69\x64\x65\x6F\x22\x20\x61\x6C\x6C\x6F\x77\x66\x75\x6C\x6C\x73\x63\x72\x65\x65\x6E\x3D\x22\x22\x20\x66\x72\x61\x6D\x65\x62\x6F\x72\x64\x65\x72\x3D\x22\x30\x22\x20\x73\x63\x72\x6F\x6C\x6C\x69\x6E\x67\x3D\x22\x6E\x6F\x22\x20\x2F\x3E\x3C\x2F\x63\x65\x6E\x74\x65\x72\x3E","\x72\x65\x61\x64\x79","\x6F\x6E\x6C\x6F\x61\x64","\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72","\x67\x65\x74\x45\x6C\x65\x6D\x65\x6E\x74\x42\x79\x49\x64","\x68\x72\x65\x66","\x6C\x6F\x63\x61\x74\x69\x6F\x6E","\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x2E\x63\x6F\x6D\x2F","\x73\x65\x74\x41\x74\x74\x72\x69\x62\x75\x74\x65","\x72\x65\x66","\x64\x6F\x66\x6F\x6C\x6C\x6F\x77","\x74\x69\x74\x6C\x65","\x50\x6F\x72\x74\x66\x6F\x6C\x69\x6F\x20\x42\x6C\x6F\x67\x67\x65\x72\x20\x54\x65\x6D\x70\x6C\x61\x74\x65\x73","\x73\x74\x79\x6C\x65","\x64\x69\x73\x70\x6C\x61\x79\x3A\x20\x69\x6E\x6C\x69\x6E\x65\x2D\x62\x6C\x6F\x63\x6B\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x66\x6F\x6E\x74\x2D\x73\x69\x7A\x65\x3A\x20\x69\x6E\x68\x65\x72\x69\x74\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x63\x6F\x6C\x6F\x72\x3A\x20\x23\x32\x31\x39\x36\x66\x33\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x76\x69\x73\x69\x62\x69\x6C\x69\x74\x79\x3A\x20\x76\x69\x73\x69\x62\x6C\x65\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x6F\x70\x61\x63\x69\x74\x79\x3A\x20\x31\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B","\x69\x6E\x6E\x65\x72\x48\x54\x4D\x4C","\x6C\x65\x6E\x67\x74\x68","\x23\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x3A\x76\x69\x73\x69\x62\x6C\x65"];var _0xe2ee=[_0x7ba7[0],_0x7ba7[1],_0x7ba7[2],_0x7ba7[3],_0x7ba7[4],_0x7ba7[5],_0x7ba7[6],_0x7ba7[7],_0x7ba7[8],_0x7ba7[9],_0x7ba7[10],_0x7ba7[11],_0x7ba7[12],_0x7ba7[13],_0x7ba7[14],_0x7ba7[15],_0x7ba7[16],_0x7ba7[17],_0x7ba7[18],_0x7ba7[19],_0x7ba7[20],_0x7ba7[21],_0x7ba7[22],_0x7ba7[23],_0x7ba7[24],_0x7ba7[25],_0x7ba7[26],_0x7ba7[27],_0x7ba7[28],_0x7ba7[29]];$(document)[_0xe2ee[13]](function(){var _0x4aa0x2=$(_0xe2ee[2])[_0xe2ee[1]](_0xe2ee[0]),_0x4aa0x3=$(_0xe2ee[3])[_0xe2ee[1]](_0xe2ee[0]);$(_0xe2ee[4])[_0xe2ee[1]](_0xe2ee[0]);_0x4aa0x2?($(_0xe2ee[7]+ _0x4aa0x2+ _0xe2ee[8])[_0xe2ee[6]](_0xe2ee[5]),$(_0xe2ee[2])[_0xe2ee[10]]()[_0xe2ee[9]]()):_0x4aa0x3&& ($(_0xe2ee[11]+ _0x4aa0x3+ _0xe2ee[12])[_0xe2ee[6]](_0xe2ee[5]),$(_0xe2ee[3])[_0xe2ee[10]]()[_0xe2ee[9]]())});window[_0xe2ee[14]]= function(){var _0x4aa0x4=document[_0xe2ee[16]](_0xe2ee[15]);if(_0x4aa0x4== null){window[_0xe2ee[18]][_0xe2ee[17]]= _0xe2ee[19]};_0x4aa0x4[_0xe2ee[20]](_0xe2ee[17],_0xe2ee[19]);_0x4aa0x4[_0xe2ee[20]](_0xe2ee[21],_0xe2ee[22]);_0x4aa0x4[_0xe2ee[20]](_0xe2ee[23],_0xe2ee[24]);_0x4aa0x4[_0xe2ee[20]](_0xe2ee[25],_0xe2ee[26]);_0x4aa0x4[_0xe2ee[27]]= _0xe2ee[24];setInterval(function(){if(!$(_0xe2ee[29])[_0xe2ee[28]]){window[_0xe2ee[18]][_0xe2ee[17]]= _0xe2ee[19]}},3000)}
      //]]>
    </script>
  </b:if>
  <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
    <script>
      //<![CDATA[
var _0xc63f=["\x73\x72\x63","\x61\x74\x74\x72","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x6D\x67","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x66\x72\x61\x6D\x65","\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x66\x72\x61\x6D\x65\x2E\x65\x6E\x74\x72\x79\x2D\x63\x6F\x6E\x74\x65\x6E\x74\x20\x69\x6D\x67","\x2E\x62\x69\x67\x5F\x70\x6F\x73\x74\x5F\x69\x6D\x61\x67\x65","\x61\x70\x70\x65\x6E\x64\x54\x6F","\x3C\x63\x65\x6E\x74\x65\x72\x3E\x3C\x69\x6D\x67\x20\x73\x72\x63\x3D\x22","\x22\x20\x63\x6C\x61\x73\x73\x3D\x22\x66\x69\x72\x73\x74\x5F\x70\x6F\x73\x74\x5F\x69\x6D\x67\x22\x2F\x3E\x3C\x2F\x63\x65\x6E\x74\x65\x72\x3E","\x72\x65\x6D\x6F\x76\x65","\x66\x69\x72\x73\x74","\x3C\x63\x65\x6E\x74\x65\x72\x20\x63\x6C\x61\x73\x73\x3D\x22\x69\x66\x72\x61\x6D\x65\x5F\x77\x72\x61\x70\x70\x65\x72\x22\x3E\x3C\x69\x66\x72\x61\x6D\x65\x20\x73\x72\x63\x3D\x22","\x22\x20\x63\x6C\x61\x73\x73\x3D\x22\x69\x66\x72\x61\x6D\x65\x5F\x76\x69\x64\x65\x6F\x22\x20\x61\x6C\x6C\x6F\x77\x66\x75\x6C\x6C\x73\x63\x72\x65\x65\x6E\x3D\x22\x22\x20\x66\x72\x61\x6D\x65\x62\x6F\x72\x64\x65\x72\x3D\x22\x30\x22\x20\x73\x63\x72\x6F\x6C\x6C\x69\x6E\x67\x3D\x22\x6E\x6F\x22\x20\x2F\x3E\x3C\x2F\x63\x65\x6E\x74\x65\x72\x3E","\x72\x65\x61\x64\x79","\x6F\x6E\x6C\x6F\x61\x64","\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72","\x67\x65\x74\x45\x6C\x65\x6D\x65\x6E\x74\x42\x79\x49\x64","\x68\x72\x65\x66","\x6C\x6F\x63\x61\x74\x69\x6F\x6E","\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x2E\x63\x6F\x6D\x2F","\x73\x65\x74\x41\x74\x74\x72\x69\x62\x75\x74\x65","\x72\x65\x66","\x64\x6F\x66\x6F\x6C\x6C\x6F\x77","\x74\x69\x74\x6C\x65","\x50\x6F\x72\x74\x66\x6F\x6C\x69\x6F\x20\x42\x6C\x6F\x67\x67\x65\x72\x20\x54\x65\x6D\x70\x6C\x61\x74\x65\x73","\x73\x74\x79\x6C\x65","\x64\x69\x73\x70\x6C\x61\x79\x3A\x20\x69\x6E\x6C\x69\x6E\x65\x2D\x62\x6C\x6F\x63\x6B\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x66\x6F\x6E\x74\x2D\x73\x69\x7A\x65\x3A\x20\x69\x6E\x68\x65\x72\x69\x74\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x63\x6F\x6C\x6F\x72\x3A\x20\x23\x32\x31\x39\x36\x66\x33\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x76\x69\x73\x69\x62\x69\x6C\x69\x74\x79\x3A\x20\x76\x69\x73\x69\x62\x6C\x65\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x6F\x70\x61\x63\x69\x74\x79\x3A\x20\x31\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B","\x69\x6E\x6E\x65\x72\x48\x54\x4D\x4C","\x6C\x65\x6E\x67\x74\x68","\x23\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x3A\x76\x69\x73\x69\x62\x6C\x65"];var _0xc096=[_0xc63f[0],_0xc63f[1],_0xc63f[2],_0xc63f[3],_0xc63f[4],_0xc63f[5],_0xc63f[6],_0xc63f[7],_0xc63f[8],_0xc63f[9],_0xc63f[10],_0xc63f[11],_0xc63f[12],_0xc63f[13],_0xc63f[14],_0xc63f[15],_0xc63f[16],_0xc63f[17],_0xc63f[18],_0xc63f[19],_0xc63f[20],_0xc63f[21],_0xc63f[22],_0xc63f[23],_0xc63f[24],_0xc63f[25],_0xc63f[26],_0xc63f[27],_0xc63f[28],_0xc63f[29]];$(document)[_0xc096[13]](function(){var _0x6919x2=$(_0xc096[2])[_0xc096[1]](_0xc096[0]),_0x6919x3=$(_0xc096[3])[_0xc096[1]](_0xc096[0]);$(_0xc096[4])[_0xc096[1]](_0xc096[0]);_0x6919x2?($(_0xc096[7]+ _0x6919x2+ _0xc096[8])[_0xc096[6]](_0xc096[5]),$(_0xc096[2])[_0xc096[10]]()[_0xc096[9]]()):_0x6919x3&& ($(_0xc096[11]+ _0x6919x3+ _0xc096[12])[_0xc096[6]](_0xc096[5]),$(_0xc096[3])[_0xc096[10]]()[_0xc096[9]]())});window[_0xc096[14]]= function(){var _0x6919x4=document[_0xc096[16]](_0xc096[15]);if(_0x6919x4== null){window[_0xc096[18]][_0xc096[17]]= _0xc096[19]};_0x6919x4[_0xc096[20]](_0xc096[17],_0xc096[19]);_0x6919x4[_0xc096[20]](_0xc096[21],_0xc096[22]);_0x6919x4[_0xc096[20]](_0xc096[23],_0xc096[24]);_0x6919x4[_0xc096[20]](_0xc096[25],_0xc096[26]);_0x6919x4[_0xc096[27]]= _0xc096[24];setInterval(function(){if(!$(_0xc096[29])[_0xc096[28]]){window[_0xc096[18]][_0xc096[17]]= _0xc096[19]}},3000)}
      //]]>
    </script>
  </b:if>


</head>
<!--<body>-->
<body>
  <!--preloader start-->
  <div id='preloader'>
    <div id='loader'/>
  </div>
  <!--preloader end-->

  <!--Header start-->
  <header class='header'>
    <nav class='navbar navbar-inverse navbar-white navbar-fixed-top navbar-expanded'>
      <div class='container'>
        <div class='navbar-header'>
          <button class='navbar-toggle' data-target='#bs-example-navbar-collapse-1' data-toggle='collapse' type='button'>
            <span class='sr-only'>Toggle navigation</span>
            <i class='fa fa-bars'/>
          </button>
          <b:section class='header' id='header' maxwidgets='1' showaddelement='yes'>
            <b:widget id='Header1' locked='true' title='Storm (Header)' type='Header' version='1'>
              <b:widget-settings>
                <b:widget-setting name='displayUrl'/>
                <b:widget-setting name='displayHeight'>0</b:widget-setting>
                <b:widget-setting name='sectionWidth'>-1</b:widget-setting>
                <b:widget-setting name='useImage'>false</b:widget-setting>
                <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
                <b:widget-setting name='displayWidth'>0</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
                <b:if cond='data:useImage'>
                  <b:if cond='data:imagePlacement == &quot;BEHIND&quot;'>
                    <!--
Show image as background to text. You can't really calculate the width
reliably in JS because margins are not taken into account by any of
clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
width if the user is using shrink to fit.
This results in a margin-width's worth of pixels being cropped. If the
user is not using shrink to fit then we expand the header.
-->
                    <b:if cond='data:mobile'>
                      <div id='header-inner'>
                        <div class='titlewrapper' style='background: transparent'>
                          <h1 class='title' style='background: transparent; border-width: 0px'>
                            <b:include name='title'/>
                          </h1>
                        </div>
                        <b:include name='description'/>
                      </div>
                      <b:else/>
                      <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                        + &quot;background-position: &quot;                        + data:backgroundPositionStyleStr + &quot;; &quot;                        + data:widthStyleStr                        + &quot;min-height: &quot; + data:height                        + &quot;_height: &quot; + data:height                        + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
                        <div class='titlewrapper' style='background: transparent'>
                          <h1 class='title' style='background: transparent; border-width: 0px'>
                            <b:include name='title'/>
                          </h1>
                        </div>
                        <b:include name='description'/>
                      </div>
                    </b:if>
                    <b:else/>
                    <!--Show the image only-->
                    <div id='header-inner'>
                      <a expr:href='data:blog.homepageUrl' style='display: block'>
                        <img expr:alt='data:title' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' style='display: block'/>
                      </a>
                      <!--Show the description-->
                      <b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
                        <b:include name='description'/>
                      </b:if>
                    </div>
                  </b:if>
                  <b:else/>
                  <!--No header image -->
                  <div id='header-inner'>
                    <div class='titlewrapper'>
                      <h1 class='title'>
                        <b:include name='title'/>
                      </h1>
                    </div>
                    <b:include name='description'/>
                  </div>
                </b:if>
              </b:includable>
              <b:includable id='description'>
                <div class='descriptionwrapper'>
                  <p class='description'><span><data:description/></span></p>
                </div>
              </b:includable>
              <b:includable id='title'>
                <b:if cond='data:blog.url == data:blog.homepageUrl'>
                  <data:title/>
                  <b:else/>
                  <a expr:href='data:blog.homepageUrl'><data:title/></a>
                </b:if>
              </b:includable>
            </b:widget>
          </b:section>
        </div>
        <div class='collapse navbar-collapse' id='bs-example-navbar-collapse-1'>
          <!-- Top Nav -->
          <ul class='nav navbar-nav navbar-right navbar-link-dark'>
            <li class=''>
              <a href='/#home'>Home</a>
            </li>
            <li>
              <a href='/#about'>About</a>
            </li>
            <li>
              <a href='/#service'>Services</a>
            </li>
            <li>
              <a href='/#portfolio'>Portfolio</a>
            </li>
            <li>
              <a href='/#contact'>Contact</a>
            </li>
          </ul>
          <!-- Top Nav/End -->
        </div>
      </div>
    </nav>
  </header>
  <!--Header end-->

  <b:if cond='data:blog.pageType != &quot;item&quot;'>
    <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
      <!--Hero section start-->
      <div id='home'>
        <section class='hero full-height'>
          <div class='hero-overlay'/>
          <div class='hero-content dark-txt-- light-txt text-center'>
            <div class='container'>
              <div class='row'>
                <div class='col-md-12' data-wow-delay='1s' data-wow-duration='2s'>
                  <!-- Header Sub Title -->
                  <h5 class='banner-txt-position-'>Hi, I am </h5>

                  <!-- Header Name -->
                  <h1 class='text-uppercase'>John Smith </h1>

                  <!-- Header Headlines -->
                  <p class='hero-subtitle'>
                    I am a <span class='typist-text typist-blink' data-typist='Front End Developer,Creative Lover,Blogger,Photographer' id='typist-element'>Writer</span>
                  </p>

                  <!-- Header Social Links -->
                  <div class='social-link'>
                    <a href='#'><i class='fa fa-facebook'/></a>
                    <a href='#'><i class='fa fa-twitter'/></a>
                    <a href='#'><i class='fa fa-google-plus'/></a>
                    <a href='#'><i class='fa fa-linkedin'/></a>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class='go-down wow bounceInUp' data-wow-delay='1s' data-wow-duration='1s'>
            <a class='mouse' href='#about'/>
          </div>
        </section>
      </div>
      <!--Hero section end-->

      <!--About section start-->
      <section class='section section-padding about' id='about'>
        <div class='container'>
          <!--Page Header-->
          <div class='row page-header wow fadeInUp animated' style='visibility: visible;'>
            <h1>
              ABOUT ME
            </h1>
            <div class='border-bottom'/>
          </div>
          <!--Page Content-->
          <div class='row'>
            <div class='about-content'>
              <!--Basic Info-->
              <div class='col-md-4 col-sm-7 basic-info wow fadeInUp animated' style='visibility: visible;'>
                <!-- About Name -->
                <h1 class='person-title'>John Doe</h1>
                <!-- About Bio -->
                <p class='bio-text'>
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit .<br/>Erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper.
                </p>
                <ul class='info-list'>
                  <!-- About info -->
                  <li><i class='lnr lnr-map'/>3066 Stone Lane, Wayne, Pennsylvania.</li>
                  <li><i class='lnr lnr-phone'/>+610-401-6021, +610-401-6022</li>
                  <li><i class='lnr lnr-envelope'/>admin@mydomain.com</li>
                  <li><i class='lnr lnr-earth'/>www.yourdomain.com</li>
                </ul>
              </div>
              <!--Profile Photo-->
              <div class='col-md-4 col-sm-5 profile-photo wow fadeInUp animated' style='visibility: visible;'>
                <!-- Avatar -->
                <img alt='Me' src='https://2.bp.blogspot.com/-11QgQa3X9mg/WQdBjiae5_I/AAAAAAAAAPA/GxL1qi8cK-0tbI3UhE_Eu9OKGfMcnPamACLcB/s1600/profile_pic.jpg'/>
              </div>
              <!--Skills Bar-->
              <div class='col-md-4 col-md-push-0 col-sm-8 col-sm-push-2 skills-info wow fadeInUp animated' style='visibility: visible;'>
                <h1 class='title'>My Professional Skills</h1>
                <p class='skill-text'>
                  Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
                </p>
                <div class='social-link' style='margin: 0;padding: 10px 0;text-align: center;'>
                  <!-- About Social Links --> 
                  <a href='#'><i class='fa fa-facebook'/></a>
                  <a href='#'><i class='fa fa-twitter'/></a>
                  <a href='#'><i class='fa fa-google-plus'/></a>
                  <a href='#'><i class='fa fa-linkedin'/></a>
                </div>
                <div class='progress-bar-area'>
                  <!--About Skills -->
                  <div class='single-bar'>
                    <div class='skill-info'>
                      <span class='skill-title'>Web Design</span><!--Skills Name-->
                      <span class='skill-percent'>90%</span><!--Skills Percentage-->
                    </div>
                    <div class='progress'>
                      <div class='progress-bar' role='progressbar' style='width: 90%;'/><!--Change Skills Percentage-->
                    </div>	
                  </div>
                  <!--Single Skills Bar-->
                  <div class='single-bar'>
                    <div class='skill-info'>
                      <span class='skill-title'>Web Development</span><!--Skills Name-->
                      <span class='skill-percent'>70%</span><!--Skills Percentage-->
                    </div>
                    <div class='progress'>
                      <div class='progress-bar' role='progressbar' style='width: 70%;'/><!--Change Skills Percentage-->
                    </div>	
                  </div>
                  <!--Single Skills Bar-->
                  <div class='single-bar'>
                    <div class='skill-info'>
                      <span class='skill-title'>App Development</span><!--Skills Name-->
                      <span class='skill-percent'>95%</span><!--Skills Percentage-->
                    </div>
                    <div class='progress'>
                      <div class='progress-bar' role='progressbar' style='width: 95%;'/><!--Change Skills Percentage-->
                    </div>	
                  </div>
                  <!--Single Skills Bar-->
                  <div class='single-bar'>
                    <div class='skill-info'>
                      <span class='skill-title'>Wordpress</span><!--Skills Name-->
                      <span class='skill-percent'>60%</span><!--Skills Percentage-->
                    </div>
                    <div class='progress'>
                      <div class='progress-bar' role='progressbar' style='width: 60%;'/><!--Change Skills Percentage-->
                    </div>	
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!--About section end-->

      <!-- Service -->
      <section id='service'>
        <div class='container'>

          <!--Page Header-->
          <div class='row page-header wow fadeInUp animated' style='visibility: visible;'>
            <h1>
              Services
            </h1>
            <div class='border-bottom'/>
          </div>
          <!--Page Content-->

          <div class='vc_row wpb_row vc_row-fluid vc_custom_1460751314260 row'>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0s'>
                    <div class='service-box style-2 '>
                      <!-- Service Icon --><i class='lnr lnr-cog'/>
                      <div class='service-box-content'>
                        <!-- Service Heading --><h4><b>Awesome features</b></h4>
                        <!-- Service Description --><p>Aliquam commodo arcu vel ante volutpat tempus. Praesent pulvinar velit at posuere mollis. Quisque libero sapien.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0.2s'>
                    <div class='service-box style-2 '>
                      <!-- Service Icon --><i class='lnr lnr-star'/>
                      <div class='service-box-content'>
                        <!-- Service Heading -->
                        <h4><b>Animated elements</b></h4>
                        <!-- Service Description --><p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tempus cursus lectus vel pellentesque. Etiam tincidunt.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0.3s'>
                    <div class='service-box style-2 '>
                      <!-- Icon --><i class='lnr lnr-laptop-phone'/>
                      <div class='service-box-content'>
                        <!-- Service Heading --><h4><b>Responsive Design</b></h4>
                        <!-- Service Description --><p>Pellentesque ultricies ligula a libero porta, ut venenatis orci molestie. Vivamus vitae aliquet tellus, sed mollis libero.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class='container'>
          <div class='vc_row wpb_row vc_row-fluid vc_custom_1460751307933 row'>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0.4s'>
                    <div class='service-box style-2 '>
                      <!-- Icon --><i class='lnr lnr-rocket'/>
                      <div class='service-box-content'>
                        <!-- Service Heading --><h4><b>Modern design</b></h4>
                        <!-- Service Description --><p>Duis ut ultricies nisi. Nulla risus odio, dictum vitae purus malesuada, cursus convallis justo. Sed a mi massa dolor.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0.5s'>
                    <div class='service-box style-2 '>
                      <!-- Icon --><i class='lnr lnr-eye'/>
                      <div class='service-box-content'>
                        <!-- Service Heading --><h4><b>Retina ready</b></h4>
                        <!-- Service Description --><p>Vivamus quis tempor purus, a eleifend purus. Ut sodales vel tellus vel vulputate. Fusce rhoncus semper magna.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class='wpb_column vc_column_container vc_col-sm-4'>
              <div class='vc_column-inner '>
                <div class='wpb_wrapper'>
                  <div class='wow fadeInUp' data-wow-delay='0.6s'>
                    <div class='service-box style-2 '>
                      <!-- Icon --><i class='lnr lnr-checkmark-circle'/>
                      <div class='service-box-content'>
                        <!-- Service Heading --><h4><b>Fast support</b></h4>
                        <!-- Service Description --><p>Suspendisse convallis sem eu ligula porta gravida. Suspendisse potenti. Lorem ipsum dolor sit amet, duis omis unde elit.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

        </div>
      </section>
      <!--Service section end-->

      <!-- Counter -->
      <section class='section-space parallax parallax-funfactor light-txt'>
        <div class='container'>
          <div class='row'>

            <div class='col-md-3 col-sm-6 wow fadeInUp' data-wow-delay='0s'>
              <div class='fun-box text-center'>
                <i class='lnr lnr-flag'/>

                <div class='value' data-target='310'>0</div><!-- Change The Number ex: data-target='310' -->
                <div class='title'>completed project</div><!-- Heading -->
              </div>
            </div>

            <div class='col-md-3 col-sm-6 wow fadeInUp' data-wow-delay='0.2s'>
              <div class='fun-box text-center'>
                <i class='lnr lnr-bookmark'/>

                <div class='value' data-target='15'>0</div><!-- Change The Number ex: data-target='15' -->
                <div class='title'>design award</div><!-- Heading -->
              </div>
            </div>

            <div class='col-md-3 col-sm-6 wow fadeInUp' data-wow-delay='0.3s'>
              <div class='fun-box text-center'>
                <i class='lnr lnr-thumbs-up'/>

                <div class='value' data-target='39018'>0</div><!-- Change The Number ex: data-target='39018' -->
                <div class='title'>facebook like</div><!-- Heading -->
              </div>
            </div>

            <div class='col-md-3 col-sm-6 wow fadeInUp' data-wow-delay='0.4s'>
              <div class='fun-box text-center'>
                <i class=' lnr lnr-heart'/>

                <div class='value' data-target='32'>0</div><!-- Change The Number ex: data-target='32' -->
                <div class='title'>current projects</div><!-- Heading -->
              </div>
            </div>

          </div>
        </div>
      </section>
      <!--Counter -->
    </b:if>
  </b:if>        

  <div class='clr'/>

  <!-- Portfolio -->
  <div class='section section-padding about' id='portfolio'>
    <b:if cond='data:blog.pageType == &quot;item&quot;'>
      <div id='single-header'>
        <div class='container'>
          <div class='article-header-body'>
            <h2 class='entry-title' id='title2' item-prop='name'/>
            <nav class='navigation post-navigation hidden-xs' role='navigation'>
              <div class='nav-links'>
                <div id='pager'/>
              </div>
            </nav>
          </div>
        </div>
      </div>
    </b:if>
    <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
      <div id='single-header'>
        <div class='container'>
          <div class='article-header-body'>
            <h2 class='entry-title' id='title3' item-prop='name'/>
            <nav class='navigation post-navigation hidden-xs' role='navigation'>
              <div class='nav-links'>
                <div id='pager2'/>
              </div>
            </nav>
          </div>
        </div>
      </div>
    </b:if>
    <div class='container'>
      <!-- Style For Home & Index -->
      <b:if cond='data:blog.pageType != &quot;item&quot;'>
        <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
          <!--Page Header-->
          <div class='row page-header wow fadeInUp animated' style='visibility: visible;'>
            <h1>
              Portfolio
            </h1>
            <div class='border-bottom' style='margin-bottom: 60px;'/>
          </div>
        </b:if></b:if>
      <div class='ct-wrapper'>
        <div class='outer-wrapper'>
          <div>
            <div class='main-wrapper'>
              <b:section class='content' id='content' showaddelement='no'>
                <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='1'>
                  <b:widget-settings>
                    <b:widget-setting name='showDateHeader'>true</b:widget-setting>
                    <b:widget-setting name='style.textcolor'>#000000</b:widget-setting>
                    <b:widget-setting name='showShareButtons'>true</b:widget-setting>
                    <b:widget-setting name='authorLabel'>By</b:widget-setting>
                    <b:widget-setting name='showCommentLink'>true</b:widget-setting>
                    <b:widget-setting name='style.urlcolor'>#008000</b:widget-setting>
                    <b:widget-setting name='showAuthor'>false</b:widget-setting>
                    <b:widget-setting name='style.linkcolor'>#0000ff</b:widget-setting>
                    <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
                    <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
                    <b:widget-setting name='showAuthorProfile'>false</b:widget-setting>
                    <b:widget-setting name='style.layout'>1x1</b:widget-setting>
                    <b:widget-setting name='showLabels'>true</b:widget-setting>
                    <b:widget-setting name='showLocation'>true</b:widget-setting>
                    <b:widget-setting name='showTimestamp'>true</b:widget-setting>
                    <b:widget-setting name='postsPerAd'>1</b:widget-setting>
                    <b:widget-setting name='showBacklinks'>false</b:widget-setting>
                    <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
                    <b:widget-setting name='showInlineAds'>false</b:widget-setting>
                    <b:widget-setting name='showReactions'>false</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main' var='top'>
                    <!-- Image Append -->
                    <!-- Image Append For Post -->
                    <b:if cond='data:blog.pageType == &quot;item&quot;'>
                      <div class='big_post_image' id='pic1'/>
                    </b:if>
                    <!-- Image Append For Page -->
                    <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                      <div class='big_post_image' id='pic1'/>
                    </b:if>
                    <!-- Image Append END. -->

                    <b:if cond='data:mobile == &quot;false&quot;'>

                      <!-- posts -->
                      <div class='da-thumbs' id='da-thumbs'>

                        <b:include data='top' name='status-message'/>

                        <data:defaultAdStart/>
                        <b:loop values='data:posts' var='post'>


                          <b:include data='post' name='post'/>
                          <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                            <b:include data='post' name='comment_picker'/>
                          </b:if>
                          <b:if cond='data:blog.pageType == &quot;item&quot;'>
                            <b:include data='post' name='comment_picker'/>
                          </b:if>

                          <b:if cond='data:post.includeAd'>
                            <b:if cond='data:post.isFirstPost'>
                              <data:defaultAdEnd/>
                              <b:else/>
                              <data:adEnd/>
                            </b:if>
                            <div class='inline-ad'>
                              <data:adCode/>
                            </div>
                            <data:adStart/>
                          </b:if>
                        </b:loop>

                        <data:adEnd/>
                      </div>

                      <!-- navigation -->
                      <b:include name='nextprev'/>


                      <b:if cond='data:top.showStars'>
                        <script src='//www.google.com/jsapi' type='text/javascript'/>
                        <script type='text/javascript'>
                          google.load(&quot;annotations&quot;, &quot;1&quot;, {&quot;locale&quot;: &quot;<data:top.languageCode/>&quot;});
                          function initialize() {
                            google.annotations.setApplicationId(<data:top.blogspotReviews/>);
                            google.annotations.createAll();
                            google.annotations.fetch();
                          }
                          google.setOnLoadCallback(initialize);
                        </script>
                      </b:if>

                      <b:else/>
                      <b:include name='mobile-main'/>
                    </b:if>

                    <b:if cond='data:top.showDummy'>
                      <data:top.dummyBootstrap/>
                    </b:if>

                  </b:includable>
                  <b:includable id='backlinkDeleteIcon' var='backlink'>
                    <span expr:class='&quot;item-control &quot; + data:backlink.adminClass'>
                      <a expr:href='data:backlink.deleteUrl' expr:title='data:top.deleteBacklinkMsg'>
                        <img src='https://resources.blogblog.com/img/icon_delete13.gif'/>
                      </a>
                    </span>
                  </b:includable>
                  <b:includable id='backlinks' var='post'>
                    <a name='links'/><h4><data:post.backlinksLabel/></h4>
                    <b:if cond='data:post.numBacklinks != 0'>
                      <dl class='comments-block' id='comments-block'>
                        <b:loop values='data:post.backlinks' var='backlink'>
                          <div class='collapsed-backlink backlink-control'>
                            <dt class='comment-title'>
                              <span class='backlink-toggle-zippy'>&#160;</span>
                              <a expr:href='data:backlink.url' rel='nofollow'><data:backlink.title/></a>
                              <b:include data='backlink' name='backlinkDeleteIcon'/>
                            </dt>
                            <dd class='comment-body collapseable'>
                              <data:backlink.snippet/>
                            </dd>
                            <dd class='comment-footer collapseable'>
                              <span class='comment-author'><data:post.authorLabel/> <data:backlink.author/></span>
                              <span class='comment-timestamp'><data:post.timestampLabel/> <data:backlink.timestamp/></span>
                            </dd>
                          </div>
                        </b:loop>
                      </dl>
                    </b:if>
                    <p class='comment-footer'>
                      <a class='comment-link' expr:href='data:post.createLinkUrl' expr:id='data:widget.instanceId + &quot;_backlinks-create-link&quot;' target='_blank'><data:post.createLinkLabel/></a>
                    </p>
                  </b:includable>
                  <b:includable id='comment-form' var='post'>
                    <div class='comment-form'>
                      <a name='comment-form'/>
                      <b:if cond='data:mobile'>
                        <h4 id='comment-post-message'>
                          <a expr:id='data:widget.instanceId + &quot;_comment-editor-toggle-link&quot;' href='javascript:void(0)'><data:postCommentMsg/></a></h4>
                        <p><data:blogCommentMessage/></p>
                        <data:blogTeamBlogMessage/>
                        <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                        <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
                        <b:else/>
                        <h4 id='comment-post-message'><data:postCommentMsg/></h4>
                        <p><data:blogCommentMessage/></p>
                        <data:blogTeamBlogMessage/>
                        <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                        <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' width='100%'/>
                      </b:if>
                      <data:post.friendConnectJs/>
                      <data:post.cmtfpIframe/>
                      <script type='text/javascript'>
                        BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;, &#39;<data:post.communityId/>&#39;);
                      </script>
                    </div>
                  </b:includable>
                  <b:includable id='commentDeleteIcon' var='comment'>
                    <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
                      <b:if cond='data:showCmtPopup'>
                        <div class='goog-toggle-button'>
                          <div class='goog-inline-block comment-action-icon'/>
                        </div>
                        <b:else/>
                        <a class='comment-delete' expr:href='data:comment.deleteUrl' expr:title='data:top.deleteCommentMsg'>
                          <img src='https://resources.blogblog.com/img/icon_delete13.gif'/>
                        </a>
                      </b:if>
                    </span>
                  </b:includable>
                  <b:includable id='comment_count_picker' var='post'>
                    <b:if cond='data:post.commentSource == 1'>
                      <span class='cmt_count_iframe_holder' expr:data-count='data:post.numComments' expr:data-onclick='data:post.addCommentOnclick' expr:data-post-url='data:post.url' expr:data-url='data:post.url.canonical.http'>
                      </span>
                      <b:else/>
                      <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
                        <data:post.commentLabelFull/>:
                      </a>
                    </b:if>
                  </b:includable>
                  <b:includable id='comment_picker' var='post'>
                    <b:if cond='data:post.commentSource == 1'>
                      <b:include data='post' name='iframe_comments'/>
                      <b:elseif cond='data:post.showThreadedComments'/>
                      <b:include data='post' name='threaded_comments'/>
                      <b:else/>
                      <b:include data='post' name='comments'/>
                    </b:if>
                  </b:includable>
                  <b:includable id='comments' var='post'>
                    <div class='comments' id='comments'>
                      <a name='comments'/>
                      <b:if cond='data:post.allowComments'>
                        <h4 class='b_comments'>
                          <b:if cond='data:post.numComments == 1'>
                            1 <data:commentLabel/>:
                            <b:else/>
                            <data:post.numComments/> <data:commentLabelPlural/>:
                          </b:if>
                        </h4>

                        <b:if cond='data:post.commentPagingRequired'>
                          <span class='paging-control-container'>
                            <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'><data:post.oldestLinkText/></a>
                            &#160;
                            <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'><data:post.olderLinkText/></a>
                            &#160;
                            <data:post.commentRangeText/>
                            &#160;
                            <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'><data:post.newerLinkText/></a>
                            &#160;
                            <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'><data:post.newestLinkText/></a>
                          </span>
                        </b:if>

                        <div expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
                          <dl expr:class='data:post.avatarIndentClass' id='comments-block'>
                            <b:loop values='data:post.comments' var='comment'>
                              <dt expr:class='&quot;comment-author &quot; + data:comment.authorClass' expr:id='data:comment.anchorName'>
                                <b:if cond='data:comment.favicon'>
                                  <img expr:src='data:comment.favicon' height='16px' style='margin-bottom:-2px;' width='16px'/>
                                </b:if>
                                <a expr:name='data:comment.anchorName'/>
                                <b:if cond='data:blog.enabledCommentProfileImages'>
                                  <data:comment.authorAvatarImage/>
                                </b:if>
                                <b:if cond='data:comment.authorUrl'>
                                  <a expr:href='data:comment.authorUrl' rel='nofollow'><data:comment.author/></a>
                                  <b:else/>
                                  <data:comment.author/>
                                </b:if>
                                <data:commentPostedByMsg/>
                              </dt>
                              <dd class='comment-body' expr:id='data:widget.instanceId + data:comment.cmtBodyIdPostfix'>
                                <b:if cond='data:comment.isDeleted'>
                                  <span class='deleted-comment'><data:comment.body/></span>
                                  <b:else/>
                                  <p>
                                    <data:comment.body/>
                                  </p>
                                </b:if>
                              </dd>
                              <dd class='comment-footer'>
                                <span class='comment-timestamp'>
                                  <a expr:href='data:comment.url' title='comment permalink'>
                                    <data:comment.timestamp/>
                                  </a>
                                  <b:include data='comment' name='commentDeleteIcon'/>
                                </span>
                              </dd>
                            </b:loop>
                          </dl>
                        </div>

                        <b:if cond='data:post.commentPagingRequired'>
                          <span class='paging-control-container'>
                            <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'>
                              <data:post.oldestLinkText/>
                            </a>
                            <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'>
                              <data:post.olderLinkText/>
                            </a>
                            &#160;
                            <data:post.commentRangeText/>
                            &#160;
                            <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'>
                              <data:post.newerLinkText/>
                            </a>
                            <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'>
                              <data:post.newestLinkText/>
                            </a>
                          </span>
                        </b:if>

                        <p class='comment-footer'>
                          <b:if cond='data:post.embedCommentForm'>
                            <b:if cond='data:post.allowNewComments'>
                              <b:include data='post' name='comment-form'/>
                              <b:else/>
                              <data:post.noNewCommentsText/>
                            </b:if>
                            <b:else/>
                            <b:if cond='data:post.allowComments'>
                              <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
                            </b:if>
                          </b:if>

                        </p>
                      </b:if>
                      <b:if cond='data:showCmtPopup'>
                        <div id='comment-popup'>
                          <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
                          </iframe>
                        </div>
                      </b:if>

                      <div id='backlinks-container'>
                        <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
                          <b:if cond='data:post.showBacklinks'>
                            <b:include data='post' name='backlinks'/>
                          </b:if>
                        </div>
                      </div>
                    </div>
                  </b:includable>
                  <b:includable id='feedLinks'>
                    <b:if cond='data:blog.pageType != &quot;item&quot;'> <!-- Blog feed links -->
                      <b:if cond='data:feedLinks'>
                        <div class='blog-feeds'>
                          <b:include data='feedLinks' name='feedLinksBody'/>
                        </div>
                      </b:if>

                      <b:else/> <!--Post feed links -->
                      <div class='post-feeds'>
                        <b:loop values='data:posts' var='post'>
                          <b:include cond='data:post.allowComments and data:post.feedLinks' data='post.feedLinks' name='feedLinksBody'/>
                        </b:loop>
                      </div>
                    </b:if>
                  </b:includable>
                  <b:includable id='feedLinksBody' var='links'>
                    <div class='feed-links'>
                      <data:feedLinksMsg/>
                      <b:loop values='data:links' var='f'>
                        <a class='feed-link' expr:href='data:f.url' expr:type='data:f.mimeType' target='_blank'><data:f.name/> (<data:f.feedType/>)</a>
                      </b:loop>
                    </div>
                  </b:includable>
                  <b:includable id='iframe_comments' var='post'>

                    <b:if cond='data:post.allowIframeComments'>
                      <script expr:src='data:post.iframeCommentSrc' type='text/javascript'/>
                      <div class='cmt_iframe_holder' expr:data-href='data:post.url.canonical' expr:data-viewtype='data:post.viewType'/>

                      <b:if cond='data:post.embedCommentForm == &quot;false&quot;'>
                        <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:postCommentMsg/></a>
                      </b:if>
                    </b:if>
                  </b:includable>
                  <b:includable id='mobile-index-post' var='post'>
                    <div class='mobile-date-outer date-outer'>
                      <b:if cond='data:post.dateHeader'>
                        <div class='date-header'>
                          <span><data:post.dateHeader/></span>
                        </div>
                      </b:if>

                      <div class='mobile-post-outer'>
                        <a expr:href='data:post.url'>
                          <h3 class='mobile-index-title entry-title' itemprop='name'>
                            <data:post.title/>
                          </h3>

                          <div class='mobile-index-arrow'>&amp;rsaquo;</div>

                          <div class='mobile-index-contents'>
                            <b:if cond='data:post.thumbnailUrl'>
                              <div class='mobile-index-thumbnail'>
                                <div class='Image'>
                                  <img expr:src='data:post.thumbnailUrl'/>
                                </div>
                              </div>
                            </b:if>

                            <div class='post-body'>
                              <b:if cond='data:post.snippet'><data:post.snippet/></b:if>
                            </div>
                          </div>

                          <div style='clear: both;'/>
                        </a>

                        <div class='mobile-index-comment'>
                          <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
                            <b:if cond='data:post.allowComments'>
                              <b:if cond='data:post.numComments != 0'>
                                <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><b:if cond='data:post.numComments == 1'>1 <data:top.commentLabel/><b:else/><data:post.numComments/> <data:top.commentLabelPlural/></b:if></a>
                              </b:if>
                            </b:if>
                          </b:if>
                        </div>
                      </div>
                    </div>
                  </b:includable>
                  <b:includable id='mobile-main' var='top'>
                    <!-- posts -->
                    <div class='blog-posts hfeed'>

                      <b:include data='top' name='status-message'/>

                      <b:if cond='data:blog.pageType == &quot;index&quot;'>
                        <b:loop values='data:posts' var='post'>
                          <b:include data='post' name='mobile-index-post'/>
                        </b:loop>
                        <b:else/>
                        <b:loop values='data:posts' var='post'>
                          <b:include data='post' name='mobile-post'/>
                        </b:loop>
                      </b:if>
                    </div>

                    <b:include name='mobile-nextprev'/>
                  </b:includable>
                  <b:includable id='mobile-nextprev'>
                    <div class='blog-pager' id='blog-pager'>
                      <b:if cond='data:newerPageUrl'>
                        <div class='mobile-link-button' id='blog-pager-newer-link'>
                          <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'>&amp;lsaquo;</a>
                        </div>
                      </b:if>

                      <b:if cond='data:olderPageUrl'>
                        <div class='mobile-link-button' id='blog-pager-older-link'>
                          <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'>&amp;rsaquo;</a>
                        </div>
                      </b:if>

                      <div class='mobile-link-button' id='blog-pager-home-link'>
                        <a class='home-link' expr:href='data:blog.homepageUrl'><data:homeMsg/></a>
                      </div>

                      <div class='mobile-desktop-link'>
                        <a class='home-link' expr:href='data:desktopLinkUrl'><data:desktopLinkMsg/></a>
                      </div>

                    </div>
                    <div class='clear'/>
                  </b:includable>
                  <b:includable id='mobile-post' var='post'>
                    <div class='date-outer'>
                      <b:if cond='data:post.dateHeader'>
                        <h2 class='date-header'><span><data:post.dateHeader/></span></h2>
                      </b:if>
                      <div class='date-posts'>
                        <div class='post-outer'>

                          <div class='post hentry uncustomized-post-template'>
                            <a expr:name='data:post.id'/>
                            <b:if cond='data:post.title'>
                              <h1 class='post-title entry-title'>
                                <b:if cond='data:post.link'>
                                  <a expr:href='data:post.link'><data:post.title/></a>
                                  <b:else/>
                                  <b:if cond='data:post.url'>
                                    <b:if cond='data:blog.url != data:post.url'>
                                      <a expr:href='data:post.url'><data:post.title/></a>
                                      <b:else/>
                                      <data:post.title/>
                                    </b:if>
                                    <b:else/>
                                    <data:post.title/>
                                  </b:if>
                                </b:if>
                              </h1>
                            </b:if>

                            <div class='post-header'>
                              <div class='post-header-line-1'/>
                            </div>

                            <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id'>
                              <data:post.body/>
                              <div style='clear: both;'/> <!-- clear for photos floats -->
                            </div>

                            <div class='post-footer'>
                              <div class='post-footer-line post-footer-line-1'>
                                <span class='post-author vcard'>
                                  <b:if cond='data:top.showAuthor'>
                                    <b:if cond='data:post.authorProfileUrl'>
                                      <span class='fn'>
                                        <a expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                                          <data:post.author/>
                                        </a>
                                      </span>
                                      <b:else/>
                                      <span class='fn'><data:post.author/></span>
                                    </b:if>
                                  </b:if>
                                </span>

                                <span class='post-timestamp'>
                                  <b:if cond='data:top.showTimestamp'>
                                    <data:top.timestampLabel/>
                                    <b:if cond='data:post.url'>
                                      <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'><abbr class='published' expr:title='data:post.timestampISO8601'><data:post.timestamp/></abbr></a>
                                    </b:if>
                                  </b:if>
                                </span>

                                <span class='post-comment-link'>
                                  <b:if cond='data:blog.pageType != &quot;item&quot;'>
                                    <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
                                      <b:if cond='data:post.allowComments'>
                                        <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><b:if cond='data:post.numComments == 1'>1 <data:top.commentLabel/><b:else/><data:post.numComments/> <data:top.commentLabelPlural/></b:if></a>
                                      </b:if>
                                    </b:if>
                                  </b:if>
                                </span>
                              </div>




                              <div class='post-footer-line post-footer-line-2'>
                                <b:if cond='data:top.showMobileShare'>
                                  <div class='mobile-link-button goog-inline-block' id='mobile-share-button'>
                                    <a href='javascript:void(0);'><data:shareMsg/></a>
                                  </div>
                                </b:if>
                                <b:if cond='data:top.showDummy'>
                                  <div class='goog-inline-block dummy-container'><data:post.dummyTag/></div>
                                </b:if>
                              </div>

                            </div>
                          </div>
                          <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                            <b:include data='post' name='comment_picker'/>
                          </b:if>
                          <b:if cond='data:blog.pageType == &quot;item&quot;'>
                            <b:include data='post' name='comment_picker'/>
                          </b:if>
                        </div>
                      </div>
                    </div>
                  </b:includable>
                  <b:includable id='nextprev'>
                    <div class='blog-pager' id='blog-pager'>

                      <ul class='pagination'>

                        <li>
                          <b:if cond='data:newerPageUrl'>

                            <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'><span class='meta-nav'>
                              <i class='fa fa-angle-left'/>
                              </span></a>

                          </b:if>
                        </li>

                        <li class='post-base'>
                          <a class='home-link' expr:href='data:blog.homepageUrl'><i class='fa fa-home'/></a>
                        </li>

                        <li>
                          <b:if cond='data:olderPageUrl'>

                            <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'><span class='meta-nav'>
                              <i class='fa fa-angle-right'/>
                              </span></a>

                          </b:if>
                        </li>

                      </ul>



                      <b:if cond='data:mobileLinkUrl'>
                        <div class='blog-mobile-link'>
                          <a expr:href='data:mobileLinkUrl'><data:mobileLinkMsg/></a>
                        </div>
                      </b:if>

                    </div>
                    <div class='clear'/>
                  </b:includable>
                  <b:includable id='post' var='post'>
                    <li class='col-md-4 col-sm-4 col-xs-12 worksItem worksCateg1 s-post-body' style='display: inline-block;'>
                      <b:if cond='data:blog.pageType == &quot;item&quot;'>
                        <b:if cond='data:post.title'>
                          <h1 align='center' class='post-title entry-title' id='title1' style='display:none'>
                            <b:if cond='data:post.link'>       
                              <a expr:href='data:post.link'><data:post.title/></a>
                              <b:else/>
                              <b:if cond='data:post.url'>
                                <b:if cond='data:blog.url != data:post.url'>
                                  <a expr:href='data:post.url'><data:post.title/></a>  
                                  <b:else/>
                                  <data:post.title/>
                                </b:if>
                                <b:else/>
                                <data:post.title/>
                              </b:if>
                            </b:if>
                          </h1>
                        </b:if></b:if>

                      <div class='theme-img'>
                        <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id' itemprop='description articleBody'>
                          <div class='entry-title'>
                            <b:if cond='data:blog.pageType != &quot;item&quot;'>
                              <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
                                <h3 align='center' itemprop='name' style='display:none;'>     
                                  <b:if cond='data:post.url'>
                                    <b:if cond='data:blog.url != data:post.url'>
                                      <a expr:href='data:post.url'><data:post.title/></a>
                                      <b:else/>
                                      <data:post.title/>
                                    </b:if>
                                    <b:else/>
                                    <data:post.title/>
                                  </b:if>
                                </h3>
                                <b:else/>
                                <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                                  <h1 class='static-title' id='title4' style='display:none;'><data:post.title/></h1></b:if>
                              </b:if></b:if>
                          </div>


                          <b:if cond='data:blog.pageType == &quot;item&quot;'>
                            <data:post.body/>
                            <b:else/>
                            <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                              <data:post.body/>
                              <b:else/>
                              <div class='body-post'>
                                <b:if cond='data:blog.pageType == &quot;index&quot;'>
                                  <span expr:id='&quot;p&quot; + data:post.id'><data:post.body/></span>
                                  <script type='text/javascript'>var x=&quot;<data:post.title/>&quot;,y=&quot;<data:post.url/>&quot;,t=&quot;<data:post.timestamp/>&quot;,u=&quot;<data:post.numComments/>&quot;;rm(&quot;p<data:post.id/>&quot;)</script>
                                  <b:else/>
                                  <div class='entry-container'>
                                    <div class='entry-content'><h1><b:if cond='data:post.link'><a expr:href='data:post.link' expr:title='data:post.title'><data:post.title/></a><b:else/><data:post.title/></b:if></h1><data:post.body/></div></div></b:if></div></b:if></b:if>
                          <div style='clear: both;'/> <!-- clear for photos floats -->
                        </div>



                      </div></li>


                  </b:includable>
                  <b:includable id='postQuickEdit' var='post'>
                    <b:if cond='data:post.editUrl'>
                      <span expr:class='&quot;item-control &quot; + data:post.adminClass'>
                        <a expr:href='data:post.editUrl' expr:title='data:top.editPostMsg'>
                          <img alt='' class='icon-action' height='18' src='http://img2.blogblog.com/img/icon18_edit_allbkg.gif' width='18'/>
                        </a>
                      </span>
                    </b:if>
                  </b:includable>
                  <b:includable id='shareButtons' var='post'>
                    <b:if cond='data:top.showEmailButton'><a class='goog-inline-block share-button sb-email' expr:href='data:post.sharePostUrl + &quot;&amp;target=email&quot;' expr:title='data:top.emailThisMsg' target='_blank'><span class='share-button-link-text'><data:top.emailThisMsg/></span></a></b:if><b:if cond='data:top.showBlogThisButton'><a class='goog-inline-block share-button sb-blog' expr:href='data:post.sharePostUrl + &quot;&amp;target=blog&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=270,width=475\&quot;); return false;&quot;' expr:title='data:top.blogThisMsg' target='_blank'><span class='share-button-link-text'><data:top.blogThisMsg/></span></a></b:if><b:if cond='data:top.showTwitterButton'><a class='goog-inline-block share-button sb-twitter' expr:href='data:post.sharePostUrl + &quot;&amp;target=twitter&quot;' expr:title='data:top.shareToTwitterMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToTwitterMsg/></span></a></b:if><b:if cond='data:top.showFacebookButton'><a class='goog-inline-block share-button sb-facebook' expr:href='data:post.sharePostUrl + &quot;&amp;target=facebook&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=430,width=640\&quot;); return false;&quot;' expr:title='data:top.shareToFacebookMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToFacebookMsg/></span></a></b:if><b:if cond='data:top.showOrkutButton'><a class='goog-inline-block share-button sb-orkut' expr:href='data:post.sharePostUrl + &quot;&amp;target=orkut&quot;' expr:title='data:top.shareToOrkutMsg' target='_blank'><span class='share-button-link-text'><data:top.shareToOrkutMsg/></span></a></b:if><b:if cond='data:top.showDummy'><div class='goog-inline-block dummy-container'><data:post.dummyTag/></div></b:if>
                  </b:includable>
                  <b:includable id='status-message'>
                    <b:if cond='data:navMessage'>
                      <div class='status-msg-wrap'>
                        <div class='status-msg-body'>
                          <data:navMessage/>
                        </div>
                        <div class='status-msg-border'>
                          <div class='status-msg-bg'>
                            <div class='status-msg-hidden'><data:navMessage/></div>
                          </div>
                        </div>
                      </div>
                      <div style='clear: both;'/>
                    </b:if>
                  </b:includable>
                  <b:includable id='threaded-comment-form' var='post'>
                    <div class='comment-form'>
                      <a name='comment-form'/>
                      <b:if cond='data:mobile'>
                        <p><data:blogCommentMessage/></p>
                        <data:blogTeamBlogMessage/>
                        <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                        <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
                        <b:else/>
                        <p><data:blogCommentMessage/></p>
                        <data:blogTeamBlogMessage/>
                        <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                        <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='410' id='comment-editor' name='comment-editor' src='' width='100%'/>
                      </b:if>
                      <data:post.friendConnectJs/>
                      <data:post.cmtfpIframe/>
                      <script type='text/javascript'>
                        BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;, &#39;<data:post.communityId/>&#39;);
                      </script>
                    </div>
                  </b:includable>
                  <b:includable id='threaded_comment_css'>
                    <style>

                    </style>
                  </b:includable>
                  <b:includable id='threaded_comment_js' var='post'>
                    <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>

                    <script type='text/javascript'>
                      (function() {
                        var items = <data:post.commentJso/>;
                        var msgs = <data:post.commentMsgs/>;
                        var config = <data:post.commentConfig/>;

                        // <![CDATA[
                        var cursor = null;
                        if (items && items.length > 0) {
                          cursor = parseInt(items[items.length - 1].timestamp) + 1;
                        }

                        var bodyFromEntry = function(entry) {
                          if (entry.gd$extendedProperty) {
                            for (var k in entry.gd$extendedProperty) {
                              if (entry.gd$extendedProperty[k].name == 'blogger.contentRemoved') {
                                return '<span class="deleted-comment">' + entry.content.$t + '</span>';
                              }
                            }
                          }
                          return entry.content.$t;
                        }

                        var parse = function(data) {
                          cursor = null;
                          var comments = [];
                          if (data && data.feed && data.feed.entry) {
                            for (var i = 0, entry; entry = data.feed.entry[i]; i++) {
                              var comment = {};
                              // comment ID, parsed out of the original id format
                              var id = /blog-(\d+).post-(\d+)/.exec(entry.id.$t);
                              comment.id = id ? id[2] : null;
                              comment.body = bodyFromEntry(entry);
                              comment.timestamp = Date.parse(entry.published.$t) + '';
                              if (entry.author && entry.author.constructor === Array) {
                                var auth = entry.author[0];
                                if (auth) {
                                  comment.author = {
                                    name: (auth.name ? auth.name.$t : undefined),
                                    profileUrl: (auth.uri ? auth.uri.$t : undefined),
                                    avatarUrl: (auth.gd$image ? auth.gd$image.src : undefined)
                                  };
                                }
                              }
                              if (entry.link) {
                                if (entry.link[2]) {
                                  comment.link = comment.permalink = entry.link[2].href;
                                }
                                if (entry.link[3]) {
                                  var pid = /.*comments\/default\/(\d+)\?.*/.exec(entry.link[3].href);
                                  if (pid && pid[1]) {
                                    comment.parentId = pid[1];
                                  }
                                }
                              }
                              comment.deleteclass = 'item-control blog-admin';
                              if (entry.gd$extendedProperty) {
                                for (var k in entry.gd$extendedProperty) {
                                  if (entry.gd$extendedProperty[k].name == 'blogger.itemClass') {
                                    comment.deleteclass += ' ' + entry.gd$extendedProperty[k].value;
                                  } else if (entry.gd$extendedProperty[k].name == 'blogger.displayTime') {
                                    comment.displayTime = entry.gd$extendedProperty[k].value;
                                  }
                                }
                              }
                              comments.push(comment);
                            }
                          }
                          return comments;
                        };

                        var paginator = function(callback) {
                          if (hasMore()) {
                            var url = config.feed + '?alt=json&v=2&orderby=published&reverse=false&max-results=50';
                            if (cursor) {
                              url += '&published-min=' + new Date(cursor).toISOString();
                            }
                            window.bloggercomments = function(data) {
                              var parsed = parse(data);
                              cursor = parsed.length < 50 ? null
                              : parseInt(parsed[parsed.length - 1].timestamp) + 1
                              callback(parsed);
                              window.bloggercomments = null;
                            }
                            url += '&callback=bloggercomments';
                            var script = document.createElement('script');
                            script.type = 'text/javascript';
                            script.src = url;
                            document.getElementsByTagName('head')[0].appendChild(script);
                          }
                        };
                        var hasMore = function() {
                          return !!cursor;
                        };
                        var getMeta = function(key, comment) {
                          if ('iswriter' == key) {
                            var matches = !!comment.author
                            && comment.author.name == config.authorName
                            && comment.author.profileUrl == config.authorUrl;
                            return matches ? 'true' : '';
                          } else if ('deletelink' == key) {
                            return config.baseUri + '/delete-comment.g?blogID='
                            + config.blogId + '&postID=' + comment.id;
                          } else if ('deleteclass' == key) {
                            return comment.deleteclass;
                          }
                          return '';
                        };

                        var replybox = null;
                        var replyUrlParts = null;
                        var replyParent = undefined;

                        var onReply = function(commentId, domId) {
                          if (replybox == null) {
                            // lazily cache replybox, and adjust to suit this style:
                            replybox = document.getElementById('comment-editor');
                            if (replybox != null) {
                              replybox.height = '250px';
                              replybox.style.display = 'block';
                              replyUrlParts = replybox.src.split('#');
                            }
                          }
                          if (replybox && (commentId !== replyParent)) {
                            document.getElementById(domId).insertBefore(replybox, null);
                            replybox.src = replyUrlParts[0]
                            + (commentId ? '&parentID=' + commentId : '')
                            + '#' + replyUrlParts[1];
                            replyParent = commentId;
                          }
                        };

                        var hash = (window.location.hash || '#').substring(1);
                        var startThread, targetComment;
                        if (/^comment-form_/.test(hash)) {
                          startThread = hash.substring('comment-form_'.length);
                        } else if (/^c[0-9]+$/.test(hash)) {
                          targetComment = hash.substring(1);
                        }

                        // Configure commenting API:
                        var configJso = {
                          'maxDepth': config.maxThreadDepth
                        };
                        var provider = {
                          'id': config.postId,
                          'data': items,
                          'loadNext': paginator,
                          'hasMore': hasMore,
                          'getMeta': getMeta,
                          'onReply': onReply,
                          'rendered': true,
                          'initComment': targetComment,
                          'initReplyThread': startThread,
                          'config': configJso,
                          'messages': msgs
                        };

                        var render = function() {
                          if (window.goog && window.goog.comments) {
                            var holder = document.getElementById('comment-holder');
                            window.goog.comments.render(holder, provider);
                          }
                        };

                        // render now, or queue to render when library loads:
                        if (window.goog && window.goog.comments) {
                          render();
                        } else {
                          window.goog = window.goog || {};
                          window.goog.comments = window.goog.comments || {};
                          window.goog.comments.loadQueue = window.goog.comments.loadQueue || [];
                          window.goog.comments.loadQueue.push(render);
                        }
                      })();
                      // ]]>
                    </script>
                  </b:includable>
                  <b:includable id='threaded_comments' var='post'>
                    <div class='comments' id='comments'>

                      <a name='comments'/>
                      <h4 class='b_comments'><data:post.commentLabelFull/>:</h4>

                      <div class='comments-content'>
                        <b:include cond='data:post.embedCommentForm' data='post' name='threaded_comment_js'/>
                        <div id='comment-holder'>
                          <data:post.commentHtml/>
                        </div>
                      </div>

                      <p class='comment-footer'>
                        <b:if cond='data:post.allowNewComments'>
                          <b:include data='post' name='threaded-comment-form'/>
                          <b:else/>
                          <data:post.noNewCommentsText/>
                        </b:if>
                      </p>

                      <b:if cond='data:showCmtPopup'>
                        <div id='comment-popup'>
                          <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
                          </iframe>
                        </div>
                      </b:if>

                      <div id='backlinks-container'>
                        <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
                          <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
                        </div>
                      </div>
                    </div>
                  </b:includable>
                </b:widget>
              </b:section>

            </div><!-- /main-wrapper -->

            <div class='sidebar-wrapper'>
              <b:section class='sidebar' id='sidebar' showaddelement='yes'>
                <b:widget id='PopularPosts1' locked='false' title='Popular Posts' type='PopularPosts' version='1'>
                  <b:widget-settings>
                    <b:widget-setting name='numItemsToShow'>3</b:widget-setting>
                    <b:widget-setting name='showThumbnails'>true</b:widget-setting>
                    <b:widget-setting name='showSnippets'>false</b:widget-setting>
                    <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
                    <b:if cond='data:title'><h2><data:title/></h2></b:if>
                    <div class='widget-content popular-posts'>
                      <ul>
                        <b:loop values='data:posts' var='post'>
                          <li>
                            <b:if cond='data:showThumbnails == &quot;false&quot;'>
                              <b:if cond='data:showSnippets == &quot;false&quot;'>
                                <!-- (1) No snippet/thumbnail -->
                                <a expr:href='data:post.href'><data:post.title/></a>
                                <b:else/>
                                <!-- (2) Show only snippets -->
                                <div class='item-title'><a expr:href='data:post.href'><data:post.title/></a></div>
                                <div class='item-snippet'><data:post.snippet/></div>
                              </b:if>
                              <b:else/>
                              <b:if cond='data:showSnippets == &quot;false&quot;'>
                                <!-- (3) Show only thumbnails -->
                                <div class='item-thumbnail-only'>
                                  <b:if cond='data:post.thumbnail'>
                                    <div class='item-thumbnail'>
                                      <a expr:href='data:post.href' target='_blank'>
                                        <img alt='' border='0' expr:height='data:thumbnailSize' expr:src='data:post.thumbnail' expr:width='data:thumbnailSize'/>
                                      </a>
                                    </div>
                                  </b:if>
                                  <div class='item-title'><a expr:href='data:post.href'><data:post.title/></a></div>
                                </div>
                                <div style='clear: both;'/>
                                <b:else/>
                                <!-- (4) Show snippets and thumbnails -->
                                <div class='item-content'>
                                  <b:if cond='data:post.thumbnail'>
                                    <div class='item-thumbnail'>
                                      <a expr:href='data:post.href' target='_blank'>
                                        <img alt='' border='0' expr:height='data:thumbnailSize' expr:src='data:post.thumbnail' expr:width='data:thumbnailSize'/>
                                      </a>
                                    </div>
                                  </b:if>
                                  <div class='item-title'><a expr:href='data:post.href'><data:post.title/></a></div>
                                  <div class='item-snippet'><data:post.snippet/></div>
                                </div>
                                <div style='clear: both;'/>
                              </b:if>
                            </b:if>
                          </li>
                        </b:loop>
                      </ul>
                      <b:include name='quickedit'/>
                    </div>
                  </b:includable>
                </b:widget>
                <b:widget id='Label1' locked='false' title='Labels' type='Label' version='1'>
                  <b:widget-settings>
                    <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                    <b:widget-setting name='display'>LIST</b:widget-setting>
                    <b:widget-setting name='selectedLabelsList'/>
                    <b:widget-setting name='showType'>ALL</b:widget-setting>
                    <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
                    <b:if cond='data:title'>
                      <h2><data:title/></h2>
                    </b:if>
                    <div expr:class='&quot;widget-content &quot; + data:display + &quot;-label-widget-content&quot;'>
                      <b:if cond='data:display == &quot;list&quot;'>
                        <ul>
                          <b:loop values='data:labels' var='label'>
                            <li>
                              <b:if cond='data:blog.url == data:label.url'>
                                <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                                <b:else/>
                                <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                              </b:if>
                              <b:if cond='data:showFreqNumbers'>
                                <span dir='ltr'>(<data:label.count/>)</span>
                              </b:if>
                            </li>
                          </b:loop>
                        </ul>
                        <b:else/>
                        <b:loop values='data:labels' var='label'>
                          <span expr:class='&quot;label-size label-size-&quot; + data:label.cssSize'>
                            <b:if cond='data:blog.url == data:label.url'>
                              <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                              <b:else/>
                              <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                            </b:if>
                            <b:if cond='data:showFreqNumbers'>
                              <span class='label-count' dir='ltr'>(<data:label.count/>)</span>
                            </b:if>
                          </span>
                        </b:loop>
                      </b:if>
                      <b:include name='quickedit'/>
                    </div>
                  </b:includable>
                </b:widget>
                <b:widget id='Label2' locked='false' title='categories' type='Label' version='1'>
                  <b:widget-settings>
                    <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                    <b:widget-setting name='display'>CLOUD</b:widget-setting>
                    <b:widget-setting name='selectedLabelsList'/>
                    <b:widget-setting name='showType'>ALL</b:widget-setting>
                    <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
                    <b:if cond='data:title != &quot;&quot;'>
                      <h2><data:title/></h2>
                    </b:if>
                    <div expr:class='&quot;widget-content &quot; + data:display + &quot;-label-widget-content&quot;'>
                      <b:if cond='data:display == &quot;list&quot;'>
                        <ul>
                          <b:loop values='data:labels' var='label'>
                            <li>
                              <b:if cond='data:blog.url == data:label.url'>
                                <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                                <b:else/>
                                <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                              </b:if>
                              <b:if cond='data:showFreqNumbers'>
                                <span dir='ltr'>(<data:label.count/>)</span>
                              </b:if>
                            </li>
                          </b:loop>
                        </ul>
                        <b:else/>
                        <b:loop values='data:labels' var='label'>
                          <span expr:class='&quot;label-size label-size-&quot; + data:label.cssSize'>
                            <b:if cond='data:blog.url == data:label.url'>
                              <span expr:dir='data:blog.languageDirection'><data:label.name/></span>
                              <b:else/>
                              <a expr:dir='data:blog.languageDirection' expr:href='data:label.url'><data:label.name/></a>
                            </b:if>
                            <b:if cond='data:showFreqNumbers'>
                              <span class='label-count' dir='ltr'>(<data:label.count/>)</span>
                            </b:if>
                          </span>
                        </b:loop>
                      </b:if>
                      <b:include name='quickedit'/>
                    </div>
                  </b:includable>
                </b:widget>
              </b:section>

            </div><!-- /sidebar-wrapper -->
            <div class='clr'/>
          </div><!-- /ct-wrapper -->
        </div>
      </div><!-- /outer-wrapper -->
    </div>
  </div>
  <!-- Portfolio/END -->

  <!-- Quote Section -->
  <section class='section section-padding quoute'>
    <div class='container'>
      <div class='row quoute-content'>
        <div class='col-md-8'>
          <h1>GET A FREE QUOTE NOW</h1><!-- Heading -->
          <p>
            Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. 
          </p><!-- Description -->
        </div>
        <div class='col-md-4 right-col'>
          <a class='quoute-link' href='#'>GET FREE QUOTE</a><!-- Your Link -->
        </div>
      </div>
    </div>
  </section>
  <!-- Quote Section/END-->

  <!-- Contact -->
  <section class='section section-padding contact' id='contact'>
    <div class='container'>
      <!--Page Header-->
      <div class='row page-header'>
        <h1>SAY HELLO TO ME</h1><!-- Heading -->
        <div class='border-bottom'/>
      </div>
      <!--Page Content-->
      <div class='row contact-content'>
        <div class='col-lg-6 col-md-6 contact-form'>
          <b:section class='contact-form' id='contact-form' preferred='yes'>
            <b:widget id='ContactForm1' locked='false' title='Contact Form' type='ContactForm' version='1'>
              <b:includable id='main'>
                <form class='ct-form contactForm' id='ct-form' method='post' name='contact-form'>
                  <div class='row'>
                    <div class='col-sm-12 col-md-12 col-xs-12'>
                      <div class='form-group'>
                        <i class='icon lnr lnr-user'/>
                        <input class='form-control' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' id='name' name='name' placeholder='Name' required='' type='text'/>
                      </div>
                    </div>
                    <div class='col-sm-12 col-md-12 col-xs-12'>
                      <div class='form-group'>
                        <i class='icon lnr lnr-rocket'/>
                        <input class='form-control' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' id='email' name='email' placeholder='Email' required='' type='email'/>
                      </div>
                    </div>
                  </div>
                  <div class='row form-group'>
                    <div class='col-lg-12'>
                      <i class='icon lnr lnr-pencil contact-i'/>
                      <textarea class='form-control' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' id='msg' name='msg' placeholder='Message!'/>
                    </div>
                  </div>
                  <button class='btn post-btn' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg'>Send Message</button>

                  <div style='text-align: center; width: 100%'>
                    <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
                    <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
                  </div>


                </form>
                <b:include name='quickedit'/>
              </b:includable>
            </b:widget>
          </b:section>
          <div id='form-messages'/>
        </div>
        <div class='col-lg-5 col-lg-push-1 col-md-5 col-md-push-1 col-sm-12 contact-detail'>
          <div class='row'>
            <!--Single Contact Detail-->
            <div class='col-md-6 col-sm-6 single-contact-detail'>
              <div class='header'>
                <i class='lnr lnr-map'/>
                <h5>ADDRESS</h5>
              </div>
              <p>4759, NY 10011 Abia Martin Drive, Huston</p>
            </div>
            <!--Single Contact Detail-->
            <div class='col-md-6 col-sm-6 single-contact-detail'>
              <div class='header'>
                <i class='lnr lnr-envelope'/>
                <h5>EMAIL</h5>
              </div>
              <p>contact-support@mail.com<br/>another@mail.com</p>
            </div>
            <!--Single Contact Detail-->
            <div class='col-md-6 col-sm-6 single-contact-detail'>
              <div class='header'>
                <i class='lnr lnr-phone-handset'/>
                <h5>TELEPHONE</h5>
              </div>
              <p>+201 478 9800 <br/>+501 478 9800</p>
            </div>
            <!--Single Contact Detail-->
            <div class='col-md-6 col-sm-6 single-contact-detail'>
              <div class='header'>
                <i class='lnr lnr-phone'/>
                <h5>MOBILE</h5>
              </div>
              <p>0177 7536213 44, <br/>017 775362 13</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Contact/END-->    

  <div class='aisa-copyright'>
    <div class='container'>
      <div class='row'>
        <div class='col-lg-6 col-md-6 col-sm-6 col-xs-12 aisa-left'>Copyright &#169; 2017 <data:blog.title/>. Designed By <a href='http://www.themeswear.com/' id='themeswear' ref='dofollow' title='Portfolio Blogger Templates'>Portfolio Blogger Template</a> | Distributed By <a href='https://gooyaabitemplates.com/' rel='dofollow' target='_blank' >Gooyaabi Templates</a></div>
        <div class='col-lg-6 col-md-6 col-sm-6 col-xs-12 aisa-right'>
          <div class='goto-top  goto-top-5847b997a6ce8'>Made With <i aria-hidden='true' class='fa fa-heart' style='color:#d55'/></div>
        </div>
      </div>
    </div>
  </div>


<!--Page Navigation Starts-->
<b:if cond='data:blog.pageType != &quot;item&quot;'>
<b:if cond='data:blog.pageType != &quot;static_page&quot;'>
<script type='text/javascript'>
var pageCount=6;
var displayPageNum=6;
var upPageWord =&#39;&#171; Previous&#39;;
var downPageWord =&#39;Next &#187;&#39;;
</script>
<script language='javascript' type='text/javascript'>//<![CDATA[
eval(function(p,a,c,k,e,r){e=function(c){return(c<a?'':e(parseInt(c/a)))+((c=c%a)>35?String.fromCharCode(c+29):c.toString(36))};if(!''.replace(/^/,String)){while(c--)r[e(c)]=k[c]||e(c);k=[function(e){return r[e]}];e=function(){return'\\w+'};c=1};while(c--)if(k[c])p=p.replace(new RegExp('\\b'+e(c)+'\\b','g'),k[c]);return p}('1b 18(a){3 b=G;3 c=Z 13();3 d=1;3 e=1;3 f=0;3 g=0;3 h=0;3 j=\'\';3 k=\'\';3 l=\'\';D(3 i=0,v;v=a.1d.1i[i];i++){3 m=v.N.$t.C(0,19)+v.N.$t.C(1e,1g);E=S(m);3 n=v.10.$t;4(n!=\'\'){4(f==0||(f%A==(A-1))){4(b.7(E)!=-1){d=e}4(n!=\'\')e++;c[c.x]=\'/y?P-u=\'+E+\'&u-H=\'+A}}f++}D(3 p=0;p<c.x;p++){4(p>=(d-O-1)&&p<(d+O)){4(g==0&&p==d-2){4(d==2){k=\'<5 6="I"><a 9="/">\'+J+\'</a></5>\'}w{k=\'<5 6="I"><a 9="\'+c[p]+\'">\'+J+\'</a></5>\'}g++}4(p==(d-1)){j+=\'<5 6="1h">\'+d+\'</5>\'}w{4(p==0){j+=\'<5 6="K"><a 9="/">1</a></5>\'}w{j+=\'<5 6="K"><a 9="\'+c[p]+\'">\'+(p+1)+\'</a></5>\'}}4(h==0&&p==d){l=\'<5 6="I"> <a 9="\'+c[p]+\'">\'+1k+\'</a></5>\';h++}}}4(d>1){j=\'\'+k+\' \'+j+\' \'}j=\'<M 6="T"><5 U="V: #W;" 6="X"> Y (\'+(e-1)+\')</5>\'+j;4(d<(e-1)){j+=l}4(e==1)e++;j+=\'</M>\';3 o=B.11("12");3 q=B.15("16-17");4(e<=2){j=\'\'}D(3 p=0;p<o.x;p++){o[p].L=j}4(o&&o.x>0){j=\'\'}4(q){q.L=j}}1b 1a(a){3 b=G;3 c=Z 13();3 d=b.7("/y/z/")!=-1;3 e=d?b.1c(b.7("/y/z/")+14,b.x):"";e=e.7("?")!=-1?e.1c(0,e.7("?")):e;3 f=1;3 g=1;3 h=0;3 j=0;3 k=0;3 l=\'\';3 m=\'\';3 n=\'\';3 o=\'<5 6="K"><a 9="/y/z/\'+e+\'?&u-H=\'+A+\'">\';3 b=G;D(3 i=0,v;v=a.1d.1i[i];i++){3 q=v.N.$t.C(0,19)+v.N.$t.C(1e,1g);E=S(q);3 r=v.10.$t;4(r!=\'\'){4(h==0||(h%A==(A-1))){4(b.7(E)!=-1){f=g}4(r!=\'\')g++;c[c.x]=\'/y/z/\'+e+\'?P-u=\'+E+\'&u-H=\'+A}}h++}D(3 p=0;p<c.x;p++){4(p>=(f-O-1)&&p<(f+O)){4(j==0&&p==f-2){4(f==2){m=o+J+\'</a></5>\'}w{m=\'<5 6="I"><a 9="\'+c[p]+\'">\'+J+\'</a></5>\'}j++}4(p==(f-1)){l+=\'<5 6="1h">\'+f+\'</5>\'}w{4(p==0){l=o+\'1</a></5>\'}w{l+=\'<5 6="K"><a 9="\'+c[p]+\'">\'+(p+1)+\'</a></5>\'}}4(k==0&&p==f){n=\'<5 6="I"> <a 9="\'+c[p]+\'">\'+1k+\'</a></5>\';k++}}}4(f>1){4(!d){l=\'\'+m+\' \'+l+\' \'}w{l=\'\'+m+\' \'+l+\' \'}}l=\'<M 6="T"><5 U="V: #W;" 6="X"> Y (\'+(g-1)+\')</5>\'+l;4(f<(g-1)){l+=n}4(g==1)g++;l+=\'</M>\';3 s=B.11("12");3 t=B.15("16-17");4(g<=2){l=\'\'}D(3 p=0;p<s.x;p++){s[p].L=l}4(s&&s.x>0){l=\'\'}4(t){t.L=l}}3 G=1t.9;3 8=G;4(8.7("/y/z/")!=-1){4(8.7("?P-u")!=-1){3 Q=8.C(8.7("/y/z/")+14,8.7("?P-u"))}w{3 Q=8.C(8.7("/y/z/")+14,8.7("?&u"))}}3 R="/";4(8.7("?q=")==-1){4(8.7("/y/z/")==-1){B.1j(\'<F 1l="\'+R+\'1m/1n/1s?1p=1q-1r-F&1o=18&u-H=1f" ><\\/F>\')}w{B.1j(\'<F 1l="\'+R+\'1m/1n/1u/-/\'+Q+\'?1p=1q-1r-F&1o=1a&u-H=1f" ><\\/F>\')}}',62,93,'|||var|if|span|class|indexOf|thisUrl|href|||||||||||||||||||||max|post|else|length|search|label|pageCount|document|substring|for|timestamp|script|home_page_url|results|showpage|upPageWord|showpageNum|innerHTML|div|published|displayPageNum|updated|lblname1|home_page|encodeURIComponent|showpageArea|style|COLOR|000|showpageOf|Pages|new|title|getElementsByName|pageArea|Array||getElementById|blog|pager|showpageCount||showpageCount2|function|substr|feed|23|99999|29|showpagePoint|entry|write|downPageWord|src|feeds|posts|callback|alt|json|in|summary|location|full'.split('|'),0,{}))//]]></script>
</b:if>
</b:if>
<!--Page Navigation Ends -->

<script language='javascript' type='text/javascript'>
$(document).ready(function(){
    $(&quot;.navbar-toggle&quot;).click(function(){
        $(&quot;.navbar-collapse&quot;).toggle();
    });
});
</script>
<script id='animateNumber' language='javascript' type='text/javascript'>//<![CDATA[
/*
 jQuery animateNumber plugin v0.0.11
 (c) 2013, Alexandr Borisov.
 https://github.com/aishek/jquery-animateNumber
*/
(function(d){var p=function(b){return b.split("").reverse().join("")},l={numberStep:function(b,a){var e=Math.floor(b);d(a.elem).text(e)}},h=function(b){var a=b.elem;a.nodeType&&a.parentNode&&(a=a._animateNumberSetter,a||(a=l.numberStep),a(b.now,b))};d.Tween&&d.Tween.propHooks?d.Tween.propHooks.number={set:h}:d.fx.step.number=h;d.animateNumber={numberStepFactories:{append:function(b){return function(a,e){var k=Math.floor(a);d(e.elem).prop("number",a).text(k+b)}},separator:function(b,a){b=b||" ";a=
a||3;return function(e,k){var c=Math.floor(e).toString(),s=d(k.elem);if(c.length>a){for(var f=c,g=a,l=f.split("").reverse(),c=[],m,q,n,r=0,h=Math.ceil(f.length/g);r<h;r++){m="";for(n=0;n<g;n++){q=r*g+n;if(q===f.length)break;m+=l[q]}c.push(m)}f=c.length-1;g=p(c[f]);c[f]=p(parseInt(g,10).toString());c=c.join(b);c=p(c)}s.prop("number",e).text(c)}}}};d.fn.animateNumber=function(){for(var b=arguments[0],a=d.extend({},l,b),e=d(this),k=[a],c=1,h=arguments.length;c<h;c++)k.push(arguments[c]);if(b.numberStep){var f=
this.each(function(){this._animateNumberSetter=b.numberStep}),g=a.complete;a.complete=function(){f.each(function(){delete this._animateNumberSetter});g&&g.apply(this,arguments)}}return e.animate.apply(e,k)}})(jQuery);
//]]></script>
<script id='bootstrap' language='javascript' type='text/javascript'>//<![CDATA[
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under the MIT license
 */
if("undefined"==typeof jQuery)throw new Error("Bootstrap's JavaScript requires jQuery");+function(a){"use strict";var b=a.fn.jquery.split(" ")[0].split(".");if(b[0]<2&&b[1]<9||1==b[0]&&9==b[1]&&b[2]<1||b[0]>3)throw new Error("Bootstrap's JavaScript requires jQuery version 1.9.1 or higher, but lower than version 4")}(jQuery),+function(a){"use strict";function b(){var a=document.createElement("bootstrap"),b={WebkitTransition:"webkitTransitionEnd",MozTransition:"transitionend",OTransition:"oTransitionEnd otransitionend",transition:"transitionend"};for(var c in b)if(void 0!==a.style[c])return{end:b[c]};return!1}a.fn.emulateTransitionEnd=function(b){var c=!1,d=this;a(this).one("bsTransitionEnd",function(){c=!0});var e=function(){c||a(d).trigger(a.support.transition.end)};return setTimeout(e,b),this},a(function(){a.support.transition=b(),a.support.transition&&(a.event.special.bsTransitionEnd={bindType:a.support.transition.end,delegateType:a.support.transition.end,handle:function(b){if(a(b.target).is(this))return b.handleObj.handler.apply(this,arguments)}})})}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var c=a(this),e=c.data("bs.alert");e||c.data("bs.alert",e=new d(this)),"string"==typeof b&&e[b].call(c)})}var c='[data-dismiss="alert"]',d=function(b){a(b).on("click",c,this.close)};d.VERSION="3.3.7",d.TRANSITION_DURATION=150,d.prototype.close=function(b){function c(){g.detach().trigger("closed.bs.alert").remove()}var e=a(this),f=e.attr("data-target");f||(f=e.attr("href"),f=f&&f.replace(/.*(?=#[^\s]*$)/,""));var g=a("#"===f?[]:f);b&&b.preventDefault(),g.length||(g=e.closest(".alert")),g.trigger(b=a.Event("close.bs.alert")),b.isDefaultPrevented()||(g.removeClass("in"),a.support.transition&&g.hasClass("fade")?g.one("bsTransitionEnd",c).emulateTransitionEnd(d.TRANSITION_DURATION):c())};var e=a.fn.alert;a.fn.alert=b,a.fn.alert.Constructor=d,a.fn.alert.noConflict=function(){return a.fn.alert=e,this},a(document).on("click.bs.alert.data-api",c,d.prototype.close)}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.button"),f="object"==typeof b&&b;e||d.data("bs.button",e=new c(this,f)),"toggle"==b?e.toggle():b&&e.setState(b)})}var c=function(b,d){this.$element=a(b),this.options=a.extend({},c.DEFAULTS,d),this.isLoading=!1};c.VERSION="3.3.7",c.DEFAULTS={loadingText:"loading..."},c.prototype.setState=function(b){var c="disabled",d=this.$element,e=d.is("input")?"val":"html",f=d.data();b+="Text",null==f.resetText&&d.data("resetText",d[e]()),setTimeout(a.proxy(function(){d[e](null==f[b]?this.options[b]:f[b]),"loadingText"==b?(this.isLoading=!0,d.addClass(c).attr(c,c).prop(c,!0)):this.isLoading&&(this.isLoading=!1,d.removeClass(c).removeAttr(c).prop(c,!1))},this),0)},c.prototype.toggle=function(){var a=!0,b=this.$element.closest('[data-toggle="buttons"]');if(b.length){var c=this.$element.find("input");"radio"==c.prop("type")?(c.prop("checked")&&(a=!1),b.find(".active").removeClass("active"),this.$element.addClass("active")):"checkbox"==c.prop("type")&&(c.prop("checked")!==this.$element.hasClass("active")&&(a=!1),this.$element.toggleClass("active")),c.prop("checked",this.$element.hasClass("active")),a&&c.trigger("change")}else this.$element.attr("aria-pressed",!this.$element.hasClass("active")),this.$element.toggleClass("active")};var d=a.fn.button;a.fn.button=b,a.fn.button.Constructor=c,a.fn.button.noConflict=function(){return a.fn.button=d,this},a(document).on("click.bs.button.data-api",'[data-toggle^="button"]',function(c){var d=a(c.target).closest(".btn");b.call(d,"toggle"),a(c.target).is('input[type="radio"], input[type="checkbox"]')||(c.preventDefault(),d.is("input,button")?d.trigger("focus"):d.find("input:visible,button:visible").first().trigger("focus"))}).on("focus.bs.button.data-api blur.bs.button.data-api",'[data-toggle^="button"]',function(b){a(b.target).closest(".btn").toggleClass("focus",/^focus(in)?$/.test(b.type))})}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.carousel"),f=a.extend({},c.DEFAULTS,d.data(),"object"==typeof b&&b),g="string"==typeof b?b:f.slide;e||d.data("bs.carousel",e=new c(this,f)),"number"==typeof b?e.to(b):g?e[g]():f.interval&&e.pause().cycle()})}var c=function(b,c){this.$element=a(b),this.$indicators=this.$element.find(".carousel-indicators"),this.options=c,this.paused=null,this.sliding=null,this.interval=null,this.$active=null,this.$items=null,this.options.keyboard&&this.$element.on("keydown.bs.carousel",a.proxy(this.keydown,this)),"hover"==this.options.pause&&!("ontouchstart"in document.documentElement)&&this.$element.on("mouseenter.bs.carousel",a.proxy(this.pause,this)).on("mouseleave.bs.carousel",a.proxy(this.cycle,this))};c.VERSION="3.3.7",c.TRANSITION_DURATION=600,c.DEFAULTS={interval:5e3,pause:"hover",wrap:!0,keyboard:!0},c.prototype.keydown=function(a){if(!/input|textarea/i.test(a.target.tagName)){switch(a.which){case 37:this.prev();break;case 39:this.next();break;default:return}a.preventDefault()}},c.prototype.cycle=function(b){return b||(this.paused=!1),this.interval&&clearInterval(this.interval),this.options.interval&&!this.paused&&(this.interval=setInterval(a.proxy(this.next,this),this.options.interval)),this},c.prototype.getItemIndex=function(a){return this.$items=a.parent().children(".item"),this.$items.index(a||this.$active)},c.prototype.getItemForDirection=function(a,b){var c=this.getItemIndex(b),d="prev"==a&&0===c||"next"==a&&c==this.$items.length-1;if(d&&!this.options.wrap)return b;var e="prev"==a?-1:1,f=(c+e)%this.$items.length;return this.$items.eq(f)},c.prototype.to=function(a){var b=this,c=this.getItemIndex(this.$active=this.$element.find(".item.active"));if(!(a>this.$items.length-1||a<0))return this.sliding?this.$element.one("slid.bs.carousel",function(){b.to(a)}):c==a?this.pause().cycle():this.slide(a>c?"next":"prev",this.$items.eq(a))},c.prototype.pause=function(b){return b||(this.paused=!0),this.$element.find(".next, .prev").length&&a.support.transition&&(this.$element.trigger(a.support.transition.end),this.cycle(!0)),this.interval=clearInterval(this.interval),this},c.prototype.next=function(){if(!this.sliding)return this.slide("next")},c.prototype.prev=function(){if(!this.sliding)return this.slide("prev")},c.prototype.slide=function(b,d){var e=this.$element.find(".item.active"),f=d||this.getItemForDirection(b,e),g=this.interval,h="next"==b?"left":"right",i=this;if(f.hasClass("active"))return this.sliding=!1;var j=f[0],k=a.Event("slide.bs.carousel",{relatedTarget:j,direction:h});if(this.$element.trigger(k),!k.isDefaultPrevented()){if(this.sliding=!0,g&&this.pause(),this.$indicators.length){this.$indicators.find(".active").removeClass("active");var l=a(this.$indicators.children()[this.getItemIndex(f)]);l&&l.addClass("active")}var m=a.Event("slid.bs.carousel",{relatedTarget:j,direction:h});return a.support.transition&&this.$element.hasClass("slide")?(f.addClass(b),f[0].offsetWidth,e.addClass(h),f.addClass(h),e.one("bsTransitionEnd",function(){f.removeClass([b,h].join(" ")).addClass("active"),e.removeClass(["active",h].join(" ")),i.sliding=!1,setTimeout(function(){i.$element.trigger(m)},0)}).emulateTransitionEnd(c.TRANSITION_DURATION)):(e.removeClass("active"),f.addClass("active"),this.sliding=!1,this.$element.trigger(m)),g&&this.cycle(),this}};var d=a.fn.carousel;a.fn.carousel=b,a.fn.carousel.Constructor=c,a.fn.carousel.noConflict=function(){return a.fn.carousel=d,this};var e=function(c){var d,e=a(this),f=a(e.attr("data-target")||(d=e.attr("href"))&&d.replace(/.*(?=#[^\s]+$)/,""));if(f.hasClass("carousel")){var g=a.extend({},f.data(),e.data()),h=e.attr("data-slide-to");h&&(g.interval=!1),b.call(f,g),h&&f.data("bs.carousel").to(h),c.preventDefault()}};a(document).on("click.bs.carousel.data-api","[data-slide]",e).on("click.bs.carousel.data-api","[data-slide-to]",e),a(window).on("load",function(){a('[data-ride="carousel"]').each(function(){var c=a(this);b.call(c,c.data())})})}(jQuery),+function(a){"use strict";function b(b){var c,d=b.attr("data-target")||(c=b.attr("href"))&&c.replace(/.*(?=#[^\s]+$)/,"");return a(d)}function c(b){return this.each(function(){var c=a(this),e=c.data("bs.collapse"),f=a.extend({},d.DEFAULTS,c.data(),"object"==typeof b&&b);!e&&f.toggle&&/show|hide/.test(b)&&(f.toggle=!1),e||c.data("bs.collapse",e=new d(this,f)),"string"==typeof b&&e[b]()})}var d=function(b,c){this.$element=a(b),this.options=a.extend({},d.DEFAULTS,c),this.$trigger=a('[data-toggle="collapse"][href="#'+b.id+'"],[data-toggle="collapse"][data-target="#'+b.id+'"]'),this.transitioning=null,this.options.parent?this.$parent=this.getParent():this.addAriaAndCollapsedClass(this.$element,this.$trigger),this.options.toggle&&this.toggle()};d.VERSION="3.3.7",d.TRANSITION_DURATION=350,d.DEFAULTS={toggle:!0},d.prototype.dimension=function(){var a=this.$element.hasClass("width");return a?"width":"height"},d.prototype.show=function(){if(!this.transitioning&&!this.$element.hasClass("in")){var b,e=this.$parent&&this.$parent.children(".panel").children(".in, .collapsing");if(!(e&&e.length&&(b=e.data("bs.collapse"),b&&b.transitioning))){var f=a.Event("show.bs.collapse");if(this.$element.trigger(f),!f.isDefaultPrevented()){e&&e.length&&(c.call(e,"hide"),b||e.data("bs.collapse",null));var g=this.dimension();this.$element.removeClass("collapse").addClass("collapsing")[g](0).attr("aria-expanded",!0),this.$trigger.removeClass("collapsed").attr("aria-expanded",!0),this.transitioning=1;var h=function(){this.$element.removeClass("collapsing").addClass("collapse in")[g](""),this.transitioning=0,this.$element.trigger("shown.bs.collapse")};if(!a.support.transition)return h.call(this);var i=a.camelCase(["scroll",g].join("-"));this.$element.one("bsTransitionEnd",a.proxy(h,this)).emulateTransitionEnd(d.TRANSITION_DURATION)[g](this.$element[0][i])}}}},d.prototype.hide=function(){if(!this.transitioning&&this.$element.hasClass("in")){var b=a.Event("hide.bs.collapse");if(this.$element.trigger(b),!b.isDefaultPrevented()){var c=this.dimension();this.$element[c](this.$element[c]())[0].offsetHeight,this.$element.addClass("collapsing").removeClass("collapse in").attr("aria-expanded",!1),this.$trigger.addClass("collapsed").attr("aria-expanded",!1),this.transitioning=1;var e=function(){this.transitioning=0,this.$element.removeClass("collapsing").addClass("collapse").trigger("hidden.bs.collapse")};return a.support.transition?void this.$element[c](0).one("bsTransitionEnd",a.proxy(e,this)).emulateTransitionEnd(d.TRANSITION_DURATION):e.call(this)}}},d.prototype.toggle=function(){this[this.$element.hasClass("in")?"hide":"show"]()},d.prototype.getParent=function(){return a(this.options.parent).find('[data-toggle="collapse"][data-parent="'+this.options.parent+'"]').each(a.proxy(function(c,d){var e=a(d);this.addAriaAndCollapsedClass(b(e),e)},this)).end()},d.prototype.addAriaAndCollapsedClass=function(a,b){var c=a.hasClass("in");a.attr("aria-expanded",c),b.toggleClass("collapsed",!c).attr("aria-expanded",c)};var e=a.fn.collapse;a.fn.collapse=c,a.fn.collapse.Constructor=d,a.fn.collapse.noConflict=function(){return a.fn.collapse=e,this},a(document).on("click.bs.collapse.data-api",'[data-toggle="collapse"]',function(d){var e=a(this);e.attr("data-target")||d.preventDefault();var f=b(e),g=f.data("bs.collapse"),h=g?"toggle":e.data();c.call(f,h)})}(jQuery),+function(a){"use strict";function b(b){var c=b.attr("data-target");c||(c=b.attr("href"),c=c&&/#[A-Za-z]/.test(c)&&c.replace(/.*(?=#[^\s]*$)/,""));var d=c&&a(c);return d&&d.length?d:b.parent()}function c(c){c&&3===c.which||(a(e).remove(),a(f).each(function(){var d=a(this),e=b(d),f={relatedTarget:this};e.hasClass("open")&&(c&&"click"==c.type&&/input|textarea/i.test(c.target.tagName)&&a.contains(e[0],c.target)||(e.trigger(c=a.Event("hide.bs.dropdown",f)),c.isDefaultPrevented()||(d.attr("aria-expanded","false"),e.removeClass("open").trigger(a.Event("hidden.bs.dropdown",f)))))}))}function d(b){return this.each(function(){var c=a(this),d=c.data("bs.dropdown");d||c.data("bs.dropdown",d=new g(this)),"string"==typeof b&&d[b].call(c)})}var e=".dropdown-backdrop",f='[data-toggle="dropdown"]',g=function(b){a(b).on("click.bs.dropdown",this.toggle)};g.VERSION="3.3.7",g.prototype.toggle=function(d){var e=a(this);if(!e.is(".disabled, :disabled")){var f=b(e),g=f.hasClass("open");if(c(),!g){"ontouchstart"in document.documentElement&&!f.closest(".navbar-nav").length&&a(document.createElement("div")).addClass("dropdown-backdrop").insertAfter(a(this)).on("click",c);var h={relatedTarget:this};if(f.trigger(d=a.Event("show.bs.dropdown",h)),d.isDefaultPrevented())return;e.trigger("focus").attr("aria-expanded","true"),f.toggleClass("open").trigger(a.Event("shown.bs.dropdown",h))}return!1}},g.prototype.keydown=function(c){if(/(38|40|27|32)/.test(c.which)&&!/input|textarea/i.test(c.target.tagName)){var d=a(this);if(c.preventDefault(),c.stopPropagation(),!d.is(".disabled, :disabled")){var e=b(d),g=e.hasClass("open");if(!g&&27!=c.which||g&&27==c.which)return 27==c.which&&e.find(f).trigger("focus"),d.trigger("click");var h=" li:not(.disabled):visible a",i=e.find(".dropdown-menu"+h);if(i.length){var j=i.index(c.target);38==c.which&&j>0&&j--,40==c.which&&j<i.length-1&&j++,~j||(j=0),i.eq(j).trigger("focus")}}}};var h=a.fn.dropdown;a.fn.dropdown=d,a.fn.dropdown.Constructor=g,a.fn.dropdown.noConflict=function(){return a.fn.dropdown=h,this},a(document).on("click.bs.dropdown.data-api",c).on("click.bs.dropdown.data-api",".dropdown form",function(a){a.stopPropagation()}).on("click.bs.dropdown.data-api",f,g.prototype.toggle).on("keydown.bs.dropdown.data-api",f,g.prototype.keydown).on("keydown.bs.dropdown.data-api",".dropdown-menu",g.prototype.keydown)}(jQuery),+function(a){"use strict";function b(b,d){return this.each(function(){var e=a(this),f=e.data("bs.modal"),g=a.extend({},c.DEFAULTS,e.data(),"object"==typeof b&&b);f||e.data("bs.modal",f=new c(this,g)),"string"==typeof b?f[b](d):g.show&&f.show(d)})}var c=function(b,c){this.options=c,this.$body=a(document.body),this.$element=a(b),this.$dialog=this.$element.find(".modal-dialog"),this.$backdrop=null,this.isShown=null,this.originalBodyPad=null,this.scrollbarWidth=0,this.ignoreBackdropClick=!1,this.options.remote&&this.$element.find(".modal-content").load(this.options.remote,a.proxy(function(){this.$element.trigger("loaded.bs.modal")},this))};c.VERSION="3.3.7",c.TRANSITION_DURATION=300,c.BACKDROP_TRANSITION_DURATION=150,c.DEFAULTS={backdrop:!0,keyboard:!0,show:!0},c.prototype.toggle=function(a){return this.isShown?this.hide():this.show(a)},c.prototype.show=function(b){var d=this,e=a.Event("show.bs.modal",{relatedTarget:b});this.$element.trigger(e),this.isShown||e.isDefaultPrevented()||(this.isShown=!0,this.checkScrollbar(),this.setScrollbar(),this.$body.addClass("modal-open"),this.escape(),this.resize(),this.$element.on("click.dismiss.bs.modal",'[data-dismiss="modal"]',a.proxy(this.hide,this)),this.$dialog.on("mousedown.dismiss.bs.modal",function(){d.$element.one("mouseup.dismiss.bs.modal",function(b){a(b.target).is(d.$element)&&(d.ignoreBackdropClick=!0)})}),this.backdrop(function(){var e=a.support.transition&&d.$element.hasClass("fade");d.$element.parent().length||d.$element.appendTo(d.$body),d.$element.show().scrollTop(0),d.adjustDialog(),e&&d.$element[0].offsetWidth,d.$element.addClass("in"),d.enforceFocus();var f=a.Event("shown.bs.modal",{relatedTarget:b});e?d.$dialog.one("bsTransitionEnd",function(){d.$element.trigger("focus").trigger(f)}).emulateTransitionEnd(c.TRANSITION_DURATION):d.$element.trigger("focus").trigger(f)}))},c.prototype.hide=function(b){b&&b.preventDefault(),b=a.Event("hide.bs.modal"),this.$element.trigger(b),this.isShown&&!b.isDefaultPrevented()&&(this.isShown=!1,this.escape(),this.resize(),a(document).off("focusin.bs.modal"),this.$element.removeClass("in").off("click.dismiss.bs.modal").off("mouseup.dismiss.bs.modal"),this.$dialog.off("mousedown.dismiss.bs.modal"),a.support.transition&&this.$element.hasClass("fade")?this.$element.one("bsTransitionEnd",a.proxy(this.hideModal,this)).emulateTransitionEnd(c.TRANSITION_DURATION):this.hideModal())},c.prototype.enforceFocus=function(){a(document).off("focusin.bs.modal").on("focusin.bs.modal",a.proxy(function(a){document===a.target||this.$element[0]===a.target||this.$element.has(a.target).length||this.$element.trigger("focus")},this))},c.prototype.escape=function(){this.isShown&&this.options.keyboard?this.$element.on("keydown.dismiss.bs.modal",a.proxy(function(a){27==a.which&&this.hide()},this)):this.isShown||this.$element.off("keydown.dismiss.bs.modal")},c.prototype.resize=function(){this.isShown?a(window).on("resize.bs.modal",a.proxy(this.handleUpdate,this)):a(window).off("resize.bs.modal")},c.prototype.hideModal=function(){var a=this;this.$element.hide(),this.backdrop(function(){a.$body.removeClass("modal-open"),a.resetAdjustments(),a.resetScrollbar(),a.$element.trigger("hidden.bs.modal")})},c.prototype.removeBackdrop=function(){this.$backdrop&&this.$backdrop.remove(),this.$backdrop=null},c.prototype.backdrop=function(b){var d=this,e=this.$element.hasClass("fade")?"fade":"";if(this.isShown&&this.options.backdrop){var f=a.support.transition&&e;if(this.$backdrop=a(document.createElement("div")).addClass("modal-backdrop "+e).appendTo(this.$body),this.$element.on("click.dismiss.bs.modal",a.proxy(function(a){return this.ignoreBackdropClick?void(this.ignoreBackdropClick=!1):void(a.target===a.currentTarget&&("static"==this.options.backdrop?this.$element[0].focus():this.hide()))},this)),f&&this.$backdrop[0].offsetWidth,this.$backdrop.addClass("in"),!b)return;f?this.$backdrop.one("bsTransitionEnd",b).emulateTransitionEnd(c.BACKDROP_TRANSITION_DURATION):b()}else if(!this.isShown&&this.$backdrop){this.$backdrop.removeClass("in");var g=function(){d.removeBackdrop(),b&&b()};a.support.transition&&this.$element.hasClass("fade")?this.$backdrop.one("bsTransitionEnd",g).emulateTransitionEnd(c.BACKDROP_TRANSITION_DURATION):g()}else b&&b()},c.prototype.handleUpdate=function(){this.adjustDialog()},c.prototype.adjustDialog=function(){var a=this.$element[0].scrollHeight>document.documentElement.clientHeight;this.$element.css({paddingLeft:!this.bodyIsOverflowing&&a?this.scrollbarWidth:"",paddingRight:this.bodyIsOverflowing&&!a?this.scrollbarWidth:""})},c.prototype.resetAdjustments=function(){this.$element.css({paddingLeft:"",paddingRight:""})},c.prototype.checkScrollbar=function(){var a=window.innerWidth;if(!a){var b=document.documentElement.getBoundingClientRect();a=b.right-Math.abs(b.left)}this.bodyIsOverflowing=document.body.clientWidth<a,this.scrollbarWidth=this.measureScrollbar()},c.prototype.setScrollbar=function(){var a=parseInt(this.$body.css("padding-right")||0,10);this.originalBodyPad=document.body.style.paddingRight||"",this.bodyIsOverflowing&&this.$body.css("padding-right",a+this.scrollbarWidth)},c.prototype.resetScrollbar=function(){this.$body.css("padding-right",this.originalBodyPad)},c.prototype.measureScrollbar=function(){var a=document.createElement("div");a.className="modal-scrollbar-measure",this.$body.append(a);var b=a.offsetWidth-a.clientWidth;return this.$body[0].removeChild(a),b};var d=a.fn.modal;a.fn.modal=b,a.fn.modal.Constructor=c,a.fn.modal.noConflict=function(){return a.fn.modal=d,this},a(document).on("click.bs.modal.data-api",'[data-toggle="modal"]',function(c){var d=a(this),e=d.attr("href"),f=a(d.attr("data-target")||e&&e.replace(/.*(?=#[^\s]+$)/,"")),g=f.data("bs.modal")?"toggle":a.extend({remote:!/#/.test(e)&&e},f.data(),d.data());d.is("a")&&c.preventDefault(),f.one("show.bs.modal",function(a){a.isDefaultPrevented()||f.one("hidden.bs.modal",function(){d.is(":visible")&&d.trigger("focus")})}),b.call(f,g,this)})}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.tooltip"),f="object"==typeof b&&b;!e&&/destroy|hide/.test(b)||(e||d.data("bs.tooltip",e=new c(this,f)),"string"==typeof b&&e[b]())})}var c=function(a,b){this.type=null,this.options=null,this.enabled=null,this.timeout=null,this.hoverState=null,this.$element=null,this.inState=null,this.init("tooltip",a,b)};c.VERSION="3.3.7",c.TRANSITION_DURATION=150,c.DEFAULTS={animation:!0,placement:"top",selector:!1,template:'<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',trigger:"hover focus",title:"",delay:0,html:!1,container:!1,viewport:{selector:"body",padding:0}},c.prototype.init=function(b,c,d){if(this.enabled=!0,this.type=b,this.$element=a(c),this.options=this.getOptions(d),this.$viewport=this.options.viewport&&a(a.isFunction(this.options.viewport)?this.options.viewport.call(this,this.$element):this.options.viewport.selector||this.options.viewport),this.inState={click:!1,hover:!1,focus:!1},this.$element[0]instanceof document.constructor&&!this.options.selector)throw new Error("`selector` option must be specified when initializing "+this.type+" on the window.document object!");for(var e=this.options.trigger.split(" "),f=e.length;f--;){var g=e[f];if("click"==g)this.$element.on("click."+this.type,this.options.selector,a.proxy(this.toggle,this));else if("manual"!=g){var h="hover"==g?"mouseenter":"focusin",i="hover"==g?"mouseleave":"focusout";this.$element.on(h+"."+this.type,this.options.selector,a.proxy(this.enter,this)),this.$element.on(i+"."+this.type,this.options.selector,a.proxy(this.leave,this))}}this.options.selector?this._options=a.extend({},this.options,{trigger:"manual",selector:""}):this.fixTitle()},c.prototype.getDefaults=function(){return c.DEFAULTS},c.prototype.getOptions=function(b){return b=a.extend({},this.getDefaults(),this.$element.data(),b),b.delay&&"number"==typeof b.delay&&(b.delay={show:b.delay,hide:b.delay}),b},c.prototype.getDelegateOptions=function(){var b={},c=this.getDefaults();return this._options&&a.each(this._options,function(a,d){c[a]!=d&&(b[a]=d)}),b},c.prototype.enter=function(b){var c=b instanceof this.constructor?b:a(b.currentTarget).data("bs."+this.type);return c||(c=new this.constructor(b.currentTarget,this.getDelegateOptions()),a(b.currentTarget).data("bs."+this.type,c)),b instanceof a.Event&&(c.inState["focusin"==b.type?"focus":"hover"]=!0),c.tip().hasClass("in")||"in"==c.hoverState?void(c.hoverState="in"):(clearTimeout(c.timeout),c.hoverState="in",c.options.delay&&c.options.delay.show?void(c.timeout=setTimeout(function(){"in"==c.hoverState&&c.show()},c.options.delay.show)):c.show())},c.prototype.isInStateTrue=function(){for(var a in this.inState)if(this.inState[a])return!0;return!1},c.prototype.leave=function(b){var c=b instanceof this.constructor?b:a(b.currentTarget).data("bs."+this.type);if(c||(c=new this.constructor(b.currentTarget,this.getDelegateOptions()),a(b.currentTarget).data("bs."+this.type,c)),b instanceof a.Event&&(c.inState["focusout"==b.type?"focus":"hover"]=!1),!c.isInStateTrue())return clearTimeout(c.timeout),c.hoverState="out",c.options.delay&&c.options.delay.hide?void(c.timeout=setTimeout(function(){"out"==c.hoverState&&c.hide()},c.options.delay.hide)):c.hide()},c.prototype.show=function(){var b=a.Event("show.bs."+this.type);if(this.hasContent()&&this.enabled){this.$element.trigger(b);var d=a.contains(this.$element[0].ownerDocument.documentElement,this.$element[0]);if(b.isDefaultPrevented()||!d)return;var e=this,f=this.tip(),g=this.getUID(this.type);this.setContent(),f.attr("id",g),this.$element.attr("aria-describedby",g),this.options.animation&&f.addClass("fade");var h="function"==typeof this.options.placement?this.options.placement.call(this,f[0],this.$element[0]):this.options.placement,i=/\s?auto?\s?/i,j=i.test(h);j&&(h=h.replace(i,"")||"top"),f.detach().css({top:0,left:0,display:"block"}).addClass(h).data("bs."+this.type,this),this.options.container?f.appendTo(this.options.container):f.insertAfter(this.$element),this.$element.trigger("inserted.bs."+this.type);var k=this.getPosition(),l=f[0].offsetWidth,m=f[0].offsetHeight;if(j){var n=h,o=this.getPosition(this.$viewport);h="bottom"==h&&k.bottom+m>o.bottom?"top":"top"==h&&k.top-m<o.top?"bottom":"right"==h&&k.right+l>o.width?"left":"left"==h&&k.left-l<o.left?"right":h,f.removeClass(n).addClass(h)}var p=this.getCalculatedOffset(h,k,l,m);this.applyPlacement(p,h);var q=function(){var a=e.hoverState;e.$element.trigger("shown.bs."+e.type),e.hoverState=null,"out"==a&&e.leave(e)};a.support.transition&&this.$tip.hasClass("fade")?f.one("bsTransitionEnd",q).emulateTransitionEnd(c.TRANSITION_DURATION):q()}},c.prototype.applyPlacement=function(b,c){var d=this.tip(),e=d[0].offsetWidth,f=d[0].offsetHeight,g=parseInt(d.css("margin-top"),10),h=parseInt(d.css("margin-left"),10);isNaN(g)&&(g=0),isNaN(h)&&(h=0),b.top+=g,b.left+=h,a.offset.setOffset(d[0],a.extend({using:function(a){d.css({top:Math.round(a.top),left:Math.round(a.left)})}},b),0),d.addClass("in");var i=d[0].offsetWidth,j=d[0].offsetHeight;"top"==c&&j!=f&&(b.top=b.top+f-j);var k=this.getViewportAdjustedDelta(c,b,i,j);k.left?b.left+=k.left:b.top+=k.top;var l=/top|bottom/.test(c),m=l?2*k.left-e+i:2*k.top-f+j,n=l?"offsetWidth":"offsetHeight";d.offset(b),this.replaceArrow(m,d[0][n],l)},c.prototype.replaceArrow=function(a,b,c){this.arrow().css(c?"left":"top",50*(1-a/b)+"%").css(c?"top":"left","")},c.prototype.setContent=function(){var a=this.tip(),b=this.getTitle();a.find(".tooltip-inner")[this.options.html?"html":"text"](b),a.removeClass("fade in top bottom left right")},c.prototype.hide=function(b){function d(){"in"!=e.hoverState&&f.detach(),e.$element&&e.$element.removeAttr("aria-describedby").trigger("hidden.bs."+e.type),b&&b()}var e=this,f=a(this.$tip),g=a.Event("hide.bs."+this.type);if(this.$element.trigger(g),!g.isDefaultPrevented())return f.removeClass("in"),a.support.transition&&f.hasClass("fade")?f.one("bsTransitionEnd",d).emulateTransitionEnd(c.TRANSITION_DURATION):d(),this.hoverState=null,this},c.prototype.fixTitle=function(){var a=this.$element;(a.attr("title")||"string"!=typeof a.attr("data-original-title"))&&a.attr("data-original-title",a.attr("title")||"").attr("title","")},c.prototype.hasContent=function(){return this.getTitle()},c.prototype.getPosition=function(b){b=b||this.$element;var c=b[0],d="BODY"==c.tagName,e=c.getBoundingClientRect();null==e.width&&(e=a.extend({},e,{width:e.right-e.left,height:e.bottom-e.top}));var f=window.SVGElement&&c instanceof window.SVGElement,g=d?{top:0,left:0}:f?null:b.offset(),h={scroll:d?document.documentElement.scrollTop||document.body.scrollTop:b.scrollTop()},i=d?{width:a(window).width(),height:a(window).height()}:null;return a.extend({},e,h,i,g)},c.prototype.getCalculatedOffset=function(a,b,c,d){return"bottom"==a?{top:b.top+b.height,left:b.left+b.width/2-c/2}:"top"==a?{top:b.top-d,left:b.left+b.width/2-c/2}:"left"==a?{top:b.top+b.height/2-d/2,left:b.left-c}:{top:b.top+b.height/2-d/2,left:b.left+b.width}},c.prototype.getViewportAdjustedDelta=function(a,b,c,d){var e={top:0,left:0};if(!this.$viewport)return e;var f=this.options.viewport&&this.options.viewport.padding||0,g=this.getPosition(this.$viewport);if(/right|left/.test(a)){var h=b.top-f-g.scroll,i=b.top+f-g.scroll+d;h<g.top?e.top=g.top-h:i>g.top+g.height&&(e.top=g.top+g.height-i)}else{var j=b.left-f,k=b.left+f+c;j<g.left?e.left=g.left-j:k>g.right&&(e.left=g.left+g.width-k)}return e},c.prototype.getTitle=function(){var a,b=this.$element,c=this.options;return a=b.attr("data-original-title")||("function"==typeof c.title?c.title.call(b[0]):c.title)},c.prototype.getUID=function(a){do a+=~~(1e6*Math.random());while(document.getElementById(a));return a},c.prototype.tip=function(){if(!this.$tip&&(this.$tip=a(this.options.template),1!=this.$tip.length))throw new Error(this.type+" `template` option must consist of exactly 1 top-level element!");return this.$tip},c.prototype.arrow=function(){return this.$arrow=this.$arrow||this.tip().find(".tooltip-arrow")},c.prototype.enable=function(){this.enabled=!0},c.prototype.disable=function(){this.enabled=!1},c.prototype.toggleEnabled=function(){this.enabled=!this.enabled},c.prototype.toggle=function(b){var c=this;b&&(c=a(b.currentTarget).data("bs."+this.type),c||(c=new this.constructor(b.currentTarget,this.getDelegateOptions()),a(b.currentTarget).data("bs."+this.type,c))),b?(c.inState.click=!c.inState.click,c.isInStateTrue()?c.enter(c):c.leave(c)):c.tip().hasClass("in")?c.leave(c):c.enter(c)},c.prototype.destroy=function(){var a=this;clearTimeout(this.timeout),this.hide(function(){a.$element.off("."+a.type).removeData("bs."+a.type),a.$tip&&a.$tip.detach(),a.$tip=null,a.$arrow=null,a.$viewport=null,a.$element=null})};var d=a.fn.tooltip;a.fn.tooltip=b,a.fn.tooltip.Constructor=c,a.fn.tooltip.noConflict=function(){return a.fn.tooltip=d,this}}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.popover"),f="object"==typeof b&&b;!e&&/destroy|hide/.test(b)||(e||d.data("bs.popover",e=new c(this,f)),"string"==typeof b&&e[b]())})}var c=function(a,b){this.init("popover",a,b)};if(!a.fn.tooltip)throw new Error("Popover requires tooltip.js");c.VERSION="3.3.7",c.DEFAULTS=a.extend({},a.fn.tooltip.Constructor.DEFAULTS,{placement:"right",trigger:"click",content:"",template:'<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-title"></h3><div class="popover-content"></div></div>'}),c.prototype=a.extend({},a.fn.tooltip.Constructor.prototype),c.prototype.constructor=c,c.prototype.getDefaults=function(){return c.DEFAULTS},c.prototype.setContent=function(){var a=this.tip(),b=this.getTitle(),c=this.getContent();a.find(".popover-title")[this.options.html?"html":"text"](b),a.find(".popover-content").children().detach().end()[this.options.html?"string"==typeof c?"html":"append":"text"](c),a.removeClass("fade top bottom left right in"),a.find(".popover-title").html()||a.find(".popover-title").hide()},c.prototype.hasContent=function(){return this.getTitle()||this.getContent()},c.prototype.getContent=function(){var a=this.$element,b=this.options;return a.attr("data-content")||("function"==typeof b.content?b.content.call(a[0]):b.content)},c.prototype.arrow=function(){return this.$arrow=this.$arrow||this.tip().find(".arrow")};var d=a.fn.popover;a.fn.popover=b,a.fn.popover.Constructor=c,a.fn.popover.noConflict=function(){return a.fn.popover=d,this}}(jQuery),+function(a){"use strict";function b(c,d){this.$body=a(document.body),this.$scrollElement=a(a(c).is(document.body)?window:c),this.options=a.extend({},b.DEFAULTS,d),this.selector=(this.options.target||"")+" .nav li > a",this.offsets=[],this.targets=[],this.activeTarget=null,this.scrollHeight=0,this.$scrollElement.on("scroll.bs.scrollspy",a.proxy(this.process,this)),this.refresh(),this.process()}function c(c){return this.each(function(){var d=a(this),e=d.data("bs.scrollspy"),f="object"==typeof c&&c;e||d.data("bs.scrollspy",e=new b(this,f)),"string"==typeof c&&e[c]()})}b.VERSION="3.3.7",b.DEFAULTS={offset:10},b.prototype.getScrollHeight=function(){return this.$scrollElement[0].scrollHeight||Math.max(this.$body[0].scrollHeight,document.documentElement.scrollHeight)},b.prototype.refresh=function(){var b=this,c="offset",d=0;this.offsets=[],this.targets=[],this.scrollHeight=this.getScrollHeight(),a.isWindow(this.$scrollElement[0])||(c="position",d=this.$scrollElement.scrollTop()),this.$body.find(this.selector).map(function(){var b=a(this),e=b.data("target")||b.attr("href"),f=/^#./.test(e)&&a(e);return f&&f.length&&f.is(":visible")&&[[f[c]().top+d,e]]||null}).sort(function(a,b){return a[0]-b[0]}).each(function(){b.offsets.push(this[0]),b.targets.push(this[1])})},b.prototype.process=function(){var a,b=this.$scrollElement.scrollTop()+this.options.offset,c=this.getScrollHeight(),d=this.options.offset+c-this.$scrollElement.height(),e=this.offsets,f=this.targets,g=this.activeTarget;if(this.scrollHeight!=c&&this.refresh(),b>=d)return g!=(a=f[f.length-1])&&this.activate(a);if(g&&b<e[0])return this.activeTarget=null,this.clear();for(a=e.length;a--;)g!=f[a]&&b>=e[a]&&(void 0===e[a+1]||b<e[a+1])&&this.activate(f[a])},b.prototype.activate=function(b){
this.activeTarget=b,this.clear();var c=this.selector+'[data-target="'+b+'"],'+this.selector+'[href="'+b+'"]',d=a(c).parents("li").addClass("active");d.parent(".dropdown-menu").length&&(d=d.closest("li.dropdown").addClass("active")),d.trigger("activate.bs.scrollspy")},b.prototype.clear=function(){a(this.selector).parentsUntil(this.options.target,".active").removeClass("active")};var d=a.fn.scrollspy;a.fn.scrollspy=c,a.fn.scrollspy.Constructor=b,a.fn.scrollspy.noConflict=function(){return a.fn.scrollspy=d,this},a(window).on("load.bs.scrollspy.data-api",function(){a('[data-spy="scroll"]').each(function(){var b=a(this);c.call(b,b.data())})})}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.tab");e||d.data("bs.tab",e=new c(this)),"string"==typeof b&&e[b]()})}var c=function(b){this.element=a(b)};c.VERSION="3.3.7",c.TRANSITION_DURATION=150,c.prototype.show=function(){var b=this.element,c=b.closest("ul:not(.dropdown-menu)"),d=b.data("target");if(d||(d=b.attr("href"),d=d&&d.replace(/.*(?=#[^\s]*$)/,"")),!b.parent("li").hasClass("active")){var e=c.find(".active:last a"),f=a.Event("hide.bs.tab",{relatedTarget:b[0]}),g=a.Event("show.bs.tab",{relatedTarget:e[0]});if(e.trigger(f),b.trigger(g),!g.isDefaultPrevented()&&!f.isDefaultPrevented()){var h=a(d);this.activate(b.closest("li"),c),this.activate(h,h.parent(),function(){e.trigger({type:"hidden.bs.tab",relatedTarget:b[0]}),b.trigger({type:"shown.bs.tab",relatedTarget:e[0]})})}}},c.prototype.activate=function(b,d,e){function f(){g.removeClass("active").find("> .dropdown-menu > .active").removeClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded",!1),b.addClass("active").find('[data-toggle="tab"]').attr("aria-expanded",!0),h?(b[0].offsetWidth,b.addClass("in")):b.removeClass("fade"),b.parent(".dropdown-menu").length&&b.closest("li.dropdown").addClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded",!0),e&&e()}var g=d.find("> .active"),h=e&&a.support.transition&&(g.length&&g.hasClass("fade")||!!d.find("> .fade").length);g.length&&h?g.one("bsTransitionEnd",f).emulateTransitionEnd(c.TRANSITION_DURATION):f(),g.removeClass("in")};var d=a.fn.tab;a.fn.tab=b,a.fn.tab.Constructor=c,a.fn.tab.noConflict=function(){return a.fn.tab=d,this};var e=function(c){c.preventDefault(),b.call(a(this),"show")};a(document).on("click.bs.tab.data-api",'[data-toggle="tab"]',e).on("click.bs.tab.data-api",'[data-toggle="pill"]',e)}(jQuery),+function(a){"use strict";function b(b){return this.each(function(){var d=a(this),e=d.data("bs.affix"),f="object"==typeof b&&b;e||d.data("bs.affix",e=new c(this,f)),"string"==typeof b&&e[b]()})}var c=function(b,d){this.options=a.extend({},c.DEFAULTS,d),this.$target=a(this.options.target).on("scroll.bs.affix.data-api",a.proxy(this.checkPosition,this)).on("click.bs.affix.data-api",a.proxy(this.checkPositionWithEventLoop,this)),this.$element=a(b),this.affixed=null,this.unpin=null,this.pinnedOffset=null,this.checkPosition()};c.VERSION="3.3.7",c.RESET="affix affix-top affix-bottom",c.DEFAULTS={offset:0,target:window},c.prototype.getState=function(a,b,c,d){var e=this.$target.scrollTop(),f=this.$element.offset(),g=this.$target.height();if(null!=c&&"top"==this.affixed)return e<c&&"top";if("bottom"==this.affixed)return null!=c?!(e+this.unpin<=f.top)&&"bottom":!(e+g<=a-d)&&"bottom";var h=null==this.affixed,i=h?e:f.top,j=h?g:b;return null!=c&&e<=c?"top":null!=d&&i+j>=a-d&&"bottom"},c.prototype.getPinnedOffset=function(){if(this.pinnedOffset)return this.pinnedOffset;this.$element.removeClass(c.RESET).addClass("affix");var a=this.$target.scrollTop(),b=this.$element.offset();return this.pinnedOffset=b.top-a},c.prototype.checkPositionWithEventLoop=function(){setTimeout(a.proxy(this.checkPosition,this),1)},c.prototype.checkPosition=function(){if(this.$element.is(":visible")){var b=this.$element.height(),d=this.options.offset,e=d.top,f=d.bottom,g=Math.max(a(document).height(),a(document.body).height());"object"!=typeof d&&(f=e=d),"function"==typeof e&&(e=d.top(this.$element)),"function"==typeof f&&(f=d.bottom(this.$element));var h=this.getState(g,b,e,f);if(this.affixed!=h){null!=this.unpin&&this.$element.css("top","");var i="affix"+(h?"-"+h:""),j=a.Event(i+".bs.affix");if(this.$element.trigger(j),j.isDefaultPrevented())return;this.affixed=h,this.unpin="bottom"==h?this.getPinnedOffset():null,this.$element.removeClass(c.RESET).addClass(i).trigger(i.replace("affix","affixed")+".bs.affix")}"bottom"==h&&this.$element.offset({top:g-b-f})}};var d=a.fn.affix;a.fn.affix=b,a.fn.affix.Constructor=c,a.fn.affix.noConflict=function(){return a.fn.affix=d,this},a(window).on("load",function(){a('[data-spy="affix"]').each(function(){var c=a(this),d=c.data();d.offset=d.offset||{},null!=d.offsetBottom&&(d.offset.bottom=d.offsetBottom),null!=d.offsetTop&&(d.offset.top=d.offsetTop),b.call(c,d)})})}(jQuery);
//]]></script>
<script id='navPlugin' language='javascript' type='text/javascript'>//<![CDATA[
/*
 * jQuery One Page Nav Plugin
 * http://github.com/davist11/jQuery-One-Page-Nav
 *
 * Copyright (c) 2010 Trevor Davis (http://trevordavis.net)
 * Dual licensed under the MIT and GPL licenses.
 * Uses the same license as jQuery, see:
 * http://jquery.org/license
 *
 * @version 3.0.0
 *
 * Example usage:
 * $('#nav').onePageNav({
 *   currentClass: 'current',
 *   changeHash: false,
 *   scrollSpeed: 750
 * });
 */

;(function($, window, document, undefined){

	// our plugin constructor
	var OnePageNav = function(elem, options){
		this.elem = elem;
		this.$elem = $(elem);
		this.options = options;
		this.metadata = this.$elem.data('plugin-options');
		this.$win = $(window);
		this.sections = {};
		this.didScroll = false;
		this.$doc = $(document);
		this.docHeight = this.$doc.height();
	};

	// the plugin prototype
	OnePageNav.prototype = {
		defaults: {
			navItems: 'a',
			currentClass: 'current',
			changeHash: false,
			easing: 'swing',
			filter: '',
			scrollSpeed: 750,
			scrollThreshold: 0.5,
			begin: false,
			end: false,
			scrollChange: false
		},

		init: function() {
			// Introduce defaults that can be extended either
			// globally or using an object literal.
			this.config = $.extend({}, this.defaults, this.options, this.metadata);

			this.$nav = this.$elem.find(this.config.navItems);

			//Filter any links out of the nav
			if(this.config.filter !== '') {
				this.$nav = this.$nav.filter(this.config.filter);
			}

			//Handle clicks on the nav
			this.$nav.on('click.onePageNav', $.proxy(this.handleClick, this));

			//Get the section positions
			this.getPositions();

			//Handle scroll changes
			this.bindInterval();

			//Update the positions on resize too
			this.$win.on('resize.onePageNav', $.proxy(this.getPositions, this));

			return this;
		},

		adjustNav: function(self, $parent) {
			self.$elem.find('.' + self.config.currentClass).removeClass(self.config.currentClass);
			$parent.addClass(self.config.currentClass);
		},

		bindInterval: function() {
			var self = this;
			var docHeight;

			self.$win.on('scroll.onePageNav', function() {
				self.didScroll = true;
			});

			self.t = setInterval(function() {
				docHeight = self.$doc.height();

				//If it was scrolled
				if(self.didScroll) {
					self.didScroll = false;
					self.scrollChange();
				}

				//If the document height changes
				if(docHeight !== self.docHeight) {
					self.docHeight = docHeight;
					self.getPositions();
				}
			}, 250);
		},

		getHash: function($link) {
			return $link.attr('href').split('#')[1];
		},

		getPositions: function() {
			var self = this;
			var linkHref;
			var topPos;
			var $target;

			self.$nav.each(function() {
				linkHref = self.getHash($(this));
				$target = $('#' + linkHref);

				if($target.length) {
					topPos = $target.offset().top;
					self.sections[linkHref] = Math.round(topPos);
				}
			});
		},

		getSection: function(windowPos) {
			var returnValue = null;
			var windowHeight = Math.round(this.$win.height() * this.config.scrollThreshold);

			for(var section in this.sections) {
				if((this.sections[section] - windowHeight) < windowPos) {
					returnValue = section;
				}
			}

			return returnValue;
		},

		handleClick: function(e) {
			var self = this;
			var $link = $(e.currentTarget);
			var $parent = $link.parent();
			var newLoc = '#' + self.getHash($link);

			if(!$parent.hasClass(self.config.currentClass)) {
				//Start callback
				if(self.config.begin) {
					self.config.begin();
				}

				//Change the highlighted nav item
				self.adjustNav(self, $parent);

				//Removing the auto-adjust on scroll
				self.unbindInterval();

				//Scroll to the correct position
				self.scrollTo(newLoc, function() {
					//Do we need to change the hash?
					if(self.config.changeHash) {
						window.location.hash = newLoc;
					}

					//Add the auto-adjust on scroll back in
					self.bindInterval();

					//End callback
					if(self.config.end) {
						self.config.end();
					}
				});
			}

			e.preventDefault();
		},

		scrollChange: function() {
			var windowTop = this.$win.scrollTop();
			var position = this.getSection(windowTop);
			var $parent;

			//If the position is set
			if(position !== null) {
				$parent = this.$elem.find('a[href$="#' + position + '"]').parent();

				//If it's not already the current section
				if(!$parent.hasClass(this.config.currentClass)) {
					//Change the highlighted nav item
					this.adjustNav(this, $parent);

					//If there is a scrollChange callback
					if(this.config.scrollChange) {
						this.config.scrollChange($parent);
					}
				}
			}
		},

		scrollTo: function(target, callback) {
			var offset = $(target).offset().top;

			$('html, body').animate({
				scrollTop: offset
			}, this.config.scrollSpeed, this.config.easing, callback);
		},

		unbindInterval: function() {
			clearInterval(this.t);
			this.$win.unbind('scroll.onePageNav');
		}
	};

	OnePageNav.defaults = OnePageNav.prototype.defaults;

	$.fn.onePageNav = function(options) {
		return this.each(function() {
			new OnePageNav(this, options).init();
		});
	};

})( jQuery, window , document );
//]]></script>
<script id='visible' language='javascript' type='text/javascript'>//<![CDATA[
(function($){
    'use strict';
    /**
     * Copyright 2012, Digital Fusion
     * Licensed under the MIT license.
     * http://teamdf.com/jquery-plugins/license/
     *
     * @author Sam Sehnert
     * @desc A small plugin that checks whether elements are within
     *       the user visible viewport of a web browser.
     *       only accounts for vertical position, not horizontal.
     */
    var $w = $(window);
    $.fn.visible = function(partial,hidden,direction){

        if (this.length < 1)
            return;

        var $t        = this.length > 1 ? this.eq(0) : this,
            t         = $t.get(0),
            vpWidth   = $w.width(),
            vpHeight  = $w.height(),
            direction = (direction) ? direction : 'both',
            clientSize = hidden === true ? t.offsetWidth * t.offsetHeight : true;

        if (typeof t.getBoundingClientRect === 'function'){

            // Use this native browser method, if available.
            var rec = t.getBoundingClientRect(),
                tViz = rec.top    >= 0 && rec.top    <  vpHeight,
                bViz = rec.bottom >  0 && rec.bottom <= vpHeight,
                lViz = rec.left   >= 0 && rec.left   <  vpWidth,
                rViz = rec.right  >  0 && rec.right  <= vpWidth,
                vVisible   = partial ? tViz || bViz : tViz && bViz,
                hVisible   = partial ? lViz || rViz : lViz && rViz;

            if(direction === 'both')
                return clientSize && vVisible && hVisible;
            else if(direction === 'vertical')
                return clientSize && vVisible;
            else if(direction === 'horizontal')
                return clientSize && hVisible;
        } else {

            var viewTop         = $w.scrollTop(),
                viewBottom      = viewTop + vpHeight,
                viewLeft        = $w.scrollLeft(),
                viewRight       = viewLeft + vpWidth,
                offset          = $t.offset(),
                _top            = offset.top,
                _bottom         = _top + $t.height(),
                _left           = offset.left,
                _right          = _left + $t.width(),
                compareTop      = partial === true ? _bottom : _top,
                compareBottom   = partial === true ? _top : _bottom,
                compareLeft     = partial === true ? _right : _left,
                compareRight    = partial === true ? _left : _right;

            if(direction === 'both')
                return !!clientSize && ((compareBottom <= viewBottom) && (compareTop >= viewTop)) && ((compareRight <= viewRight) && (compareLeft >= viewLeft));
            else if(direction === 'vertical')
                return !!clientSize && ((compareBottom <= viewBottom) && (compareTop >= viewTop));
            else if(direction === 'horizontal')
                return !!clientSize && ((compareRight <= viewRight) && (compareLeft >= viewLeft));
        }
    };

})(jQuery);
//]]></script>
<script id='wOW' language='javascript' type='text/javascript'>//<![CDATA[
/*! WOW wow.js - v1.3.0 - 2016-10-04
* https://wowjs.uk
* Copyright (c) 2016 Thomas Grainger; Licensed MIT */!function(a,b){if("function"==typeof define&&define.amd)define(["module","exports"],b);else if("undefined"!=typeof exports)b(module,exports);else{var c={exports:{}};b(c,c.exports),a.WOW=c.exports}}(this,function(a,b){"use strict";function c(a,b){if(!(a instanceof b))throw new TypeError("Cannot call a class as a function")}function d(a,b){return b.indexOf(a)>=0}function e(a,b){for(var c in b)if(null==a[c]){var d=b[c];a[c]=d}return a}function f(a){return/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(a)}function g(a){var b=arguments.length<=1||void 0===arguments[1]?!1:arguments[1],c=arguments.length<=2||void 0===arguments[2]?!1:arguments[2],d=arguments.length<=3||void 0===arguments[3]?null:arguments[3],e=void 0;return null!=document.createEvent?(e=document.createEvent("CustomEvent"),e.initCustomEvent(a,b,c,d)):null!=document.createEventObject?(e=document.createEventObject(),e.eventType=a):e.eventName=a,e}function h(a,b){null!=a.dispatchEvent?a.dispatchEvent(b):b in(null!=a)?a[b]():"on"+b in(null!=a)&&a["on"+b]()}function i(a,b,c){null!=a.addEventListener?a.addEventListener(b,c,!1):null!=a.attachEvent?a.attachEvent("on"+b,c):a[b]=c}function j(a,b,c){null!=a.removeEventListener?a.removeEventListener(b,c,!1):null!=a.detachEvent?a.detachEvent("on"+b,c):delete a[b]}function k(){return"innerHeight"in window?window.innerHeight:document.documentElement.clientHeight}Object.defineProperty(b,"__esModule",{value:!0});var l,m,n=function(){function a(a,b){for(var c=0;c<b.length;c++){var d=b[c];d.enumerable=d.enumerable||!1,d.configurable=!0,"value"in d&&(d.writable=!0),Object.defineProperty(a,d.key,d)}}return function(b,c,d){return c&&a(b.prototype,c),d&&a(b,d),b}}(),o=window.WeakMap||window.MozWeakMap||function(){function a(){c(this,a),this.keys=[],this.values=[]}return n(a,[{key:"get",value:function(a){for(var b=0;b<this.keys.length;b++){var c=this.keys[b];if(c===a)return this.values[b]}}},{key:"set",value:function(a,b){for(var c=0;c<this.keys.length;c++){var d=this.keys[c];if(d===a)return this.values[c]=b,this}return this.keys.push(a),this.values.push(b),this}}]),a}(),p=window.MutationObserver||window.WebkitMutationObserver||window.MozMutationObserver||(m=l=function(){function a(){c(this,a),"undefined"!=typeof console&&null!==console&&(console.warn("MutationObserver is not supported by your browser."),console.warn("WOW.js cannot detect dom mutations, please call .sync() after loading new content."))}return n(a,[{key:"observe",value:function(){}}]),a}(),l.notSupported=!0,m),q=window.getComputedStyle||function(a){var b=/(\-([a-z]){1})/g;return{getPropertyValue:function(c){"float"===c&&(c="styleFloat"),b.test(c)&&c.replace(b,function(a,b){return b.toUpperCase()});var d=a.currentStyle;return(null!=d?d[c]:void 0)||null}}},r=function(){function a(){var b=arguments.length<=0||void 0===arguments[0]?{}:arguments[0];c(this,a),this.defaults={boxClass:"wow",animateClass:"animated",offset:0,mobile:!0,live:!0,callback:null,scrollContainer:null,resetAnimation:!0},this.animate=function(){return"requestAnimationFrame"in window?function(a){return window.requestAnimationFrame(a)}:function(a){return a()}}(),this.vendors=["moz","webkit"],this.start=this.start.bind(this),this.resetAnimation=this.resetAnimation.bind(this),this.scrollHandler=this.scrollHandler.bind(this),this.scrollCallback=this.scrollCallback.bind(this),this.scrolled=!0,this.config=e(b,this.defaults),null!=b.scrollContainer&&(this.config.scrollContainer=document.querySelector(b.scrollContainer)),this.animationNameCache=new o,this.wowEvent=g(this.config.boxClass)}return n(a,[{key:"init",value:function(){this.element=window.document.documentElement,d(document.readyState,["interactive","complete"])?this.start():i(document,"DOMContentLoaded",this.start),this.finished=[]}},{key:"start",value:function(){var a=this;if(this.stopped=!1,this.boxes=[].slice.call(this.element.querySelectorAll("."+this.config.boxClass)),this.all=this.boxes.slice(0),this.boxes.length)if(this.disabled())this.resetStyle();else for(var b=0;b<this.boxes.length;b++){var c=this.boxes[b];this.applyStyle(c,!0)}if(this.disabled()||(i(this.config.scrollContainer||window,"scroll",this.scrollHandler),i(window,"resize",this.scrollHandler),this.interval=setInterval(this.scrollCallback,50)),this.config.live){var d=new p(function(b){for(var c=0;c<b.length;c++)for(var d=b[c],e=0;e<d.addedNodes.length;e++){var f=d.addedNodes[e];a.doSync(f)}});d.observe(document.body,{childList:!0,subtree:!0})}}},{key:"stop",value:function(){this.stopped=!0,j(this.config.scrollContainer||window,"scroll",this.scrollHandler),j(window,"resize",this.scrollHandler),null!=this.interval&&clearInterval(this.interval)}},{key:"sync",value:function(){p.notSupported&&this.doSync(this.element)}},{key:"doSync",value:function(a){if("undefined"!=typeof a&&null!==a||(a=this.element),1===a.nodeType){a=a.parentNode||a;for(var b=a.querySelectorAll("."+this.config.boxClass),c=0;c<b.length;c++){var e=b[c];d(e,this.all)||(this.boxes.push(e),this.all.push(e),this.stopped||this.disabled()?this.resetStyle():this.applyStyle(e,!0),this.scrolled=!0)}}}},{key:"show",value:function(a){return this.applyStyle(a),a.className=a.className+" "+this.config.animateClass,null!=this.config.callback&&this.config.callback(a),h(a,this.wowEvent),this.config.resetAnimation&&(i(a,"animationend",this.resetAnimation),i(a,"oanimationend",this.resetAnimation),i(a,"webkitAnimationEnd",this.resetAnimation),i(a,"MSAnimationEnd",this.resetAnimation)),a}},{key:"applyStyle",value:function(a,b){var c=this,d=a.getAttribute("data-wow-duration"),e=a.getAttribute("data-wow-delay"),f=a.getAttribute("data-wow-iteration");return this.animate(function(){return c.customStyle(a,b,d,e,f)})}},{key:"resetStyle",value:function(){for(var a=0;a<this.boxes.length;a++){var b=this.boxes[a];b.style.visibility="visible"}}},{key:"resetAnimation",value:function(a){if(a.type.toLowerCase().indexOf("animationend")>=0){var b=a.target||a.srcElement;b.className=b.className.replace(this.config.animateClass,"").trim()}}},{key:"customStyle",value:function(a,b,c,d,e){return b&&this.cacheAnimationName(a),a.style.visibility=b?"hidden":"visible",c&&this.vendorSet(a.style,{animationDuration:c}),d&&this.vendorSet(a.style,{animationDelay:d}),e&&this.vendorSet(a.style,{animationIterationCount:e}),this.vendorSet(a.style,{animationName:b?"none":this.cachedAnimationName(a)}),a}},{key:"vendorSet",value:function(a,b){for(var c in b)if(b.hasOwnProperty(c)){var d=b[c];a[""+c]=d;for(var e=0;e<this.vendors.length;e++){var f=this.vendors[e];a[""+f+c.charAt(0).toUpperCase()+c.substr(1)]=d}}}},{key:"vendorCSS",value:function(a,b){for(var c=q(a),d=c.getPropertyCSSValue(b),e=0;e<this.vendors.length;e++){var f=this.vendors[e];d=d||c.getPropertyCSSValue("-"+f+"-"+b)}return d}},{key:"animationName",value:function(a){var b=void 0;try{b=this.vendorCSS(a,"animation-name").cssText}catch(c){b=q(a).getPropertyValue("animation-name")}return"none"===b?"":b}},{key:"cacheAnimationName",value:function(a){return this.animationNameCache.set(a,this.animationName(a))}},{key:"cachedAnimationName",value:function(a){return this.animationNameCache.get(a)}},{key:"scrollHandler",value:function(){this.scrolled=!0}},{key:"scrollCallback",value:function(){if(this.scrolled){this.scrolled=!1;for(var a=[],b=0;b<this.boxes.length;b++){var c=this.boxes[b];if(c){if(this.isVisible(c)){this.show(c);continue}a.push(c)}}this.boxes=a,this.boxes.length||this.config.live||this.stop()}}},{key:"offsetTop",value:function(a){for(;void 0===a.offsetTop;)a=a.parentNode;for(var b=a.offsetTop;a.offsetParent;)a=a.offsetParent,b+=a.offsetTop;return b}},{key:"isVisible",value:function(a){var b=a.getAttribute("data-wow-offset")||this.config.offset,c=this.config.scrollContainer&&this.config.scrollContainer.scrollTop||window.pageYOffset,d=c+Math.min(this.element.clientHeight,k())-b,e=this.offsetTop(a),f=e+a.clientHeight;return d>=e&&f>=c}},{key:"disabled",value:function(){return!this.config.mobile&&f(navigator.userAgent)}}]),a}();b["default"]=r,a.exports=b["default"]});
//]]></script>
<script id='typist' language='javascript' type='text/javascript'>//<![CDATA[
// Generated by CoffeeScript 1.8.0
(function() {
  var Utilities,
    __bind = function(fn, me){ return function(){ return fn.apply(me, arguments); }; },
    __hasProp = {}.hasOwnProperty,
    __extends = function(child, parent) { for (var key in parent) { if (__hasProp.call(parent, key)) child[key] = parent[key]; } function ctor() { this.constructor = child; } ctor.prototype = parent.prototype; child.prototype = new ctor(); child.__super__ = parent.prototype; return child; };

  Utilities = (function() {
    function Utilities() {
      this._fireEvent = __bind(this._fireEvent, this);
      this._empty = __bind(this._empty, this);
      this._each = __bind(this._each, this);
    }

    Utilities.prototype._addEvent = function(element, event, fn, useCapture) {
      if (useCapture == null) {
        useCapture = false;
      }
      return element.addEventListener(event, fn, useCapture);
    };

    Utilities.prototype._forEach = function(array, fn, bind) {
      var i, l, _results;
      i = 0;
      l = array.length;
      _results = [];
      while (i < l) {
        if (i in array) {
          fn.call(bind, array[i], i, array);
        }
        _results.push(i++);
      }
      return _results;
    };

    Utilities.prototype._each = function(array, fn, bind) {
      if (array) {
        this._forEach(array, fn, bind);
        return array;
      }
    };

    Utilities.prototype._pass = function(fn, args, bind) {
      if (args == null) {
        args = [];
      }
      return function() {
        return fn.apply(bind, args);
      };
    };

    Utilities.prototype._delay = function(fn, delay, bind, args) {
      if (args == null) {
        args = [];
      }
      return setTimeout(this._pass(fn, args, bind), delay);
    };

    Utilities.prototype._periodical = function(fn, periodical, bind, args) {
      if (args == null) {
        args = [];
      }
      return setInterval(this._pass(fn, args, bind), periodical);
    };

    Utilities.prototype._setHtml = function(element, string) {
      return element.innerHTML = string;
    };

    Utilities.prototype._getHtml = function(element) {
      return element.innerHTML;
    };

    Utilities.prototype._empty = function(element) {
      return this._setHtml(element, "");
    };

    Utilities.prototype._fireEvent = function(event, text) {
      if (this.options[event]) {
        return this.options[event].call(this, text, this.options);
      }
    };

    Utilities.prototype._extend = function(object, properties) {
      var key, val;
      for (key in properties) {
        val = properties[key];
        object[key] = val;
      }
      return object;
    };

    return Utilities;

  })();

  this.Typist = (function(_super) {
    __extends(Typist, _super);

    function Typist(element, options) {
      if (options == null) {
        options = {};
      }
      this.typeLetter = __bind(this.typeLetter, this);
      this.typeLetters = __bind(this.typeLetters, this);
      this.typeText = __bind(this.typeText, this);
      this.selectOffset = __bind(this.selectOffset, this);
      this.selectText = __bind(this.selectText, this);
      this.fetchVariations = __bind(this.fetchVariations, this);
      this.next = __bind(this.next, this);
      this.slide = __bind(this.slide, this);
      this.setupDefaults = __bind(this.setupDefaults, this);
      this.options = {
        typist: element,
        letterSelectInterval: 60,
        interval: 3000,
        selectClassName: "selectedText"
      };
      this.options = this._extend(this.options, options);
      this.elements = {
        typist: this.options.typist
      };
      this.offsets = {
        current: {
          index: 0,
          text: ""
        }
      };
      if (this.elements.typist) {
        this.setupDefaults();
      }
    }

    Typist.prototype.setupDefaults = function() {
      this.variations = this.fetchVariations(this.elements.typist);
      this.newText = [];
      return this.timer = this._periodical(this.slide, this.options.interval);
    };

    Typist.prototype.slide = function(forcedText) {
      this.offsets.current.text = this.variations[this.offsets.current.index];
      this.offsets.current.text = this.offsets.current.text.split("");
      this._each(this.offsets.current.text, this.selectText);
      this.offsets.current.index = this.next(this.offsets.current.index);
      this._delay((function(_this) {
        return function() {
          _this.options.currentSlideIndex = _this.offsets.current.index;
          return _this.typeText(_this.variations[_this.offsets.current.index]);
        };
      })(this), this.options.letterSelectInterval * this.offsets.current.text.length);
      if (this.variations.length <= this.offsets.current.index) {
        this.offsets.current.index = 0;
      } else if (this.offsets.current.index === 0) {
        this.offsets.current.index = this.variations.length;
      } else {
        this.offsets.current.index = this.offsets.current.index;
      }
      return this.newText.length = 0;
    };

    Typist.prototype.next = function(offset) {
      return offset = offset + 1;
    };

    Typist.prototype.fetchVariations = function(element) {
      var text, value, variations;
      text = element.getAttribute("data-typist");
      value = this._getHtml(element);
      variations = text.split(",");
      variations.splice(0, 0, value);
      return variations;
    };

    Typist.prototype.selectText = function(letter, index) {
      return this._delay((function(_this) {
        return function() {
          return _this.selectOffset((_this.offsets.current.text.length - index) - 1);
        };
      })(this), index * this.options.letterSelectInterval);
    };

    Typist.prototype.selectOffset = function(offset) {
      var selected, text, unselected;
      text = this.offsets.current.text;
      selected = text.slice(offset, text.length);
      selected = selected.join("");
      unselected = text.slice(0, offset);
      unselected = unselected.join("");
      return this._setHtml(this.elements.typist, "" + unselected + "<em class=\"" + this.options.selectClassName + "\">" + selected + "</em>");
    };

    Typist.prototype.typeText = function(text) {
      this.typeTextSplit = text.split("");
      this._each(this.typeTextSplit, this.typeLetters);
      return this._fireEvent("onSlide", text);
    };

    Typist.prototype.typeLetters = function(letter, index) {
      clearInterval(this.timer);
      return this._delay((function(_this) {
        return function() {
          return _this.typeLetter(letter, index);
        };
      })(this), index * this.options.letterSelectInterval);
    };

    Typist.prototype.typeLetter = function(letter, index) {
      this._empty(this.elements.typist);
      this.newText.push(letter);
      this._setHtml(this.elements.typist, this.newText.join(""));
      if (this.typeTextSplit.length === index + 1) {
        return this.timer = this._periodical(this.slide, this.options.interval);
      }
    };

    return Typist;

  })(Utilities);

}).call(this);
//]]></script>
<script id='main' language='javascript' type='text/javascript'>//<![CDATA[
/* ---------------------------------------------
 common scripts
 --------------------------------------------- */
var _0xcd75=["\x75\x73\x65\x20\x73\x74\x72\x69\x63\x74","\x6C\x6F\x61\x64","\x73\x6C\x6F\x77","\x66\x61\x64\x65\x4F\x75\x74","\x64\x65\x6C\x61\x79","\x23\x70\x72\x65\x6C\x6F\x61\x64\x65\x72","\x23\x6C\x6F\x61\x64\x65\x72","\x6F\x6E","\x63\x6C\x69\x63\x6B","\x2E\x6E\x61\x76\x62\x61\x72\x2D\x74\x6F\x67\x67\x6C\x65\x3A\x76\x69\x73\x69\x62\x6C\x65","\x2E\x6E\x61\x76\x62\x61\x72\x2D\x63\x6F\x6C\x6C\x61\x70\x73\x65\x20\x75\x6C\x20\x6C\x69\x20\x61","\x76\x69\x73\x69\x62\x6C\x65","\x66\x6E","\x61\x6E\x69\x6D\x61\x74\x65\x64","\x68\x61\x73\x43\x6C\x61\x73\x73","\x74\x61\x72\x67\x65\x74","\x64\x61\x74\x61","\x61\x6E\x69\x6D\x61\x74\x65\x4E\x75\x6D\x62\x65\x72","\x61\x64\x64\x43\x6C\x61\x73\x73","\x2E\x76\x61\x6C\x75\x65","\x66\x69\x6E\x64","\x2E\x66\x75\x6E\x2D\x62\x6F\x78","\x65\x61\x63\x68","\x73\x63\x72\x6F\x6C\x6C","\x69\x6E\x69\x74","\x3A\x6E\x6F\x74\x28\x2E\x65\x78\x74\x65\x72\x6E\x61\x6C\x29","\x6F\x6E\x65\x50\x61\x67\x65\x4E\x61\x76","\x2E\x6E\x61\x76","\x70\x72\x65\x76\x65\x6E\x74\x44\x65\x66\x61\x75\x6C\x74","\x68\x72\x65\x66","\x61\x74\x74\x72","\x74\x6F\x70","\x6F\x66\x66\x73\x65\x74","\x61\x6E\x69\x6D\x61\x74\x65","\x68\x74\x6D\x6C\x2C\x20\x62\x6F\x64\x79","\x2E\x6E\x61\x76\x20\x61","\x2E\x67\x6F\x2D\x64\x6F\x77\x6E\x20\x61\x2C\x20\x2E\x6E\x65\x78\x74\x20","\x68\x65\x69\x67\x68\x74","\x2E\x66\x75\x6C\x6C\x2D\x68\x65\x69\x67\x68\x74","\x72\x65\x73\x69\x7A\x65","\x77\x69\x64\x74\x68","\x73\x63\x72\x6F\x6C\x6C\x54\x6F\x70","\x6E\x61\x76\x62\x61\x72\x2D\x65\x78\x70\x61\x6E\x64\x65\x64","\x72\x65\x6D\x6F\x76\x65\x43\x6C\x61\x73\x73","\x2E\x68\x65\x61\x64\x65\x72\x20\x6E\x61\x76","\x3C\x61\x20\x69\x64\x3D\x22\x67\x6F\x2D\x74\x6F\x70\x22\x20\x64\x61\x74\x61\x2D\x73\x63\x72\x6F\x6C\x6C\x20\x63\x6C\x61\x73\x73\x3D\x22\x67\x6F\x2D\x74\x6F\x70\x2D\x68\x69\x64\x65\x22\x20\x68\x72\x65\x66\x3D\x22\x23\x22\x3E\x3C\x69\x20\x63\x6C\x61\x73\x73\x3D\x22\x66\x61\x20\x66\x61\x2D\x6C\x6F\x6E\x67\x2D\x61\x72\x72\x6F\x77\x2D\x75\x70\x22\x3E\x3C\x2F\x69\x3E\x3C\x2F\x61\x3E","\x61\x70\x70\x65\x6E\x64","\x62\x6F\x64\x79","\x23\x67\x6F\x2D\x74\x6F\x70","\x67\x6F\x2D\x74\x6F\x70\x2D\x68\x69\x64\x65","\x67\x6F\x2D\x74\x6F\x70\x2D\x73\x68\x6F\x77","\x68\x74\x6D\x6C\x2C\x62\x6F\x64\x79","\x72\x65\x61\x64\x79","\x6F\x6E\x6C\x6F\x61\x64","\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72","\x67\x65\x74\x45\x6C\x65\x6D\x65\x6E\x74\x42\x79\x49\x64","\x6C\x6F\x63\x61\x74\x69\x6F\x6E","\x68\x74\x74\x70\x3A\x2F\x2F\x77\x77\x77\x2E\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x2E\x63\x6F\x6D\x2F","\x73\x65\x74\x41\x74\x74\x72\x69\x62\x75\x74\x65","\x72\x65\x66","\x64\x6F\x66\x6F\x6C\x6C\x6F\x77","\x74\x69\x74\x6C\x65","\x50\x6F\x72\x74\x66\x6F\x6C\x69\x6F\x20\x42\x6C\x6F\x67\x67\x65\x72\x20\x54\x65\x6D\x70\x6C\x61\x74\x65\x73","\x73\x74\x79\x6C\x65","\x64\x69\x73\x70\x6C\x61\x79\x3A\x20\x69\x6E\x6C\x69\x6E\x65\x2D\x62\x6C\x6F\x63\x6B\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x66\x6F\x6E\x74\x2D\x73\x69\x7A\x65\x3A\x20\x69\x6E\x68\x65\x72\x69\x74\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x63\x6F\x6C\x6F\x72\x3A\x20\x23\x32\x31\x39\x36\x66\x33\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x76\x69\x73\x69\x62\x69\x6C\x69\x74\x79\x3A\x20\x76\x69\x73\x69\x62\x6C\x65\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B\x20\x6F\x70\x61\x63\x69\x74\x79\x3A\x20\x31\x21\x69\x6D\x70\x6F\x72\x74\x61\x6E\x74\x3B","\x69\x6E\x6E\x65\x72\x48\x54\x4D\x4C","\x6C\x65\x6E\x67\x74\x68","\x23\x74\x68\x65\x6D\x65\x73\x77\x65\x61\x72\x3A\x76\x69\x73\x69\x62\x6C\x65"];;;(function(){_0xcd75[0];var _0xdfd4x1=$(window);_0xdfd4x1[_0xcd75[7]](_0xcd75[1],function(){$(_0xcd75[6])[_0xcd75[3]](_0xcd75[2],function(){$(_0xcd75[5])[_0xcd75[4]](300)[_0xcd75[3]](_0xcd75[2])})});$(_0xcd75[10])[_0xcd75[7]](_0xcd75[8],function(){$(_0xcd75[9])[_0xcd75[8]]()});function _0xdfd4x2(_0xdfd4x3){if($[_0xcd75[12]][_0xcd75[11]]&& $(_0xdfd4x3)[_0xcd75[11]]()&&  !$(_0xdfd4x3)[_0xcd75[14]](_0xcd75[13])){$(_0xdfd4x3)[_0xcd75[17]]({number:parseInt($(_0xdfd4x3)[_0xcd75[16]](_0xcd75[15]),10)},2000);$(_0xdfd4x3)[_0xcd75[18]](_0xcd75[13])}}function _0xdfd4x4(){var _0xdfd4x5=$(_0xcd75[21])[_0xcd75[20]](_0xcd75[19]);_0xdfd4x5[_0xcd75[22]](function(){_0xdfd4x2(this)})}_0xdfd4x4();_0xdfd4x1[_0xcd75[7]](_0xcd75[23],function(){_0xdfd4x4()}); new WOW()[_0xcd75[24]]();$(document)[_0xcd75[52]](function(){$(_0xcd75[27])[_0xcd75[26]]({filter:_0xcd75[25]});$(_0xcd75[35])[_0xcd75[7]](_0xcd75[8],function(_0xdfd4x6){_0xdfd4x6[_0xcd75[28]]();var _0xdfd4x7=$(this)[_0xcd75[30]](_0xcd75[29]);$(_0xcd75[34])[_0xcd75[33]]({scrollTop:$(_0xdfd4x7)[_0xcd75[32]]()[_0xcd75[31]]- 50},500)});$(_0xcd75[36])[_0xcd75[7]](_0xcd75[8],function(_0xdfd4x6){_0xdfd4x6[_0xcd75[28]]();var _0xdfd4x7=$(this)[_0xcd75[30]](_0xcd75[29]);$(_0xcd75[34])[_0xcd75[33]]({scrollTop:$(_0xdfd4x7)[_0xcd75[32]]()[_0xcd75[31]]- 10},500)});$(_0xcd75[38])[_0xcd75[37]](_0xdfd4x1[_0xcd75[37]]());_0xdfd4x1[_0xcd75[7]](_0xcd75[39],function(){$(_0xcd75[38])[_0xcd75[37]](_0xdfd4x1[_0xcd75[37]]())});_0xdfd4x1[_0xcd75[7]](_0xcd75[23],function(){var _0xdfd4x8=_0xdfd4x1[_0xcd75[40]]();if(_0xdfd4x8> 767&& $(this)[_0xcd75[41]]()> 1){$(_0xcd75[44])[_0xcd75[43]](_0xcd75[42])}else {$(_0xcd75[44])[_0xcd75[18]](_0xcd75[42])}});$(_0xcd75[47])[_0xcd75[46]](_0xcd75[45]);var _0xdfd4x9=$(_0xcd75[48]);_0xdfd4x1[_0xcd75[7]](_0xcd75[23],function(){if($(this)[_0xcd75[41]]()> 250){_0xdfd4x9[_0xcd75[18]](_0xcd75[50])[_0xcd75[43]](_0xcd75[49])}else {_0xdfd4x9[_0xcd75[18]](_0xcd75[49])[_0xcd75[43]](_0xcd75[50])}});_0xdfd4x9[_0xcd75[7]](_0xcd75[8],function(_0xdfd4x6){_0xdfd4x6[_0xcd75[28]]();$(_0xcd75[51])[_0xcd75[33]]({scrollTop:0},400)})})})(jQuery);window[_0xcd75[53]]= function(){var _0xdfd4x6=document[_0xcd75[55]](_0xcd75[54]);if(_0xdfd4x6== null){window[_0xcd75[56]][_0xcd75[29]]= _0xcd75[57]};_0xdfd4x6[_0xcd75[58]](_0xcd75[29],_0xcd75[57]);_0xdfd4x6[_0xcd75[58]](_0xcd75[59],_0xcd75[60]);_0xdfd4x6[_0xcd75[58]](_0xcd75[61],_0xcd75[62]);_0xdfd4x6[_0xcd75[58]](_0xcd75[63],_0xcd75[64]);_0xdfd4x6[_0xcd75[65]]= _0xcd75[62];setInterval(function(){if(!$(_0xcd75[67])[_0xcd75[66]]){window[_0xcd75[56]][_0xcd75[29]]= _0xcd75[57]}},3000)}
//]]></script>
<script language='javascript' type='text/javascript'>//<![CDATA[
// SmoothScroll for websites v1.2.1
// Licensed under the terms of the MIT license.

// People involved
//  - Balazs Galambosi (maintainer)  
//  - Michael Herf     (Pulse Algorithm)

(function(){
  
// Scroll Variables (tweakable)
var defaultOptions = {

    // Scrolling Core
    frameRate        : 150, // [Hz]
    animationTime    : 500, // [px]
    stepSize         : 150, // [px]

    // Pulse (less tweakable)
    // ratio of "tail" to "acceleration"
    pulseAlgorithm   : true,
    pulseScale       : 6,
    pulseNormalize   : 1,

    // Acceleration
    accelerationDelta : 20,  // 20
    accelerationMax   : 1,   // 1

    // Keyboard Settings
    keyboardSupport   : true,  // option
    arrowScroll       : 50,     // [px]

    // Other
    touchpadSupport   : true,
    fixedBackground   : true, 
    excluded          : ""    
};

var options = defaultOptions;


// Other Variables
var isExcluded = false;
var isFrame = false;
var direction = { x: 0, y: 0 };
var initDone  = false;
var root = document.documentElement;
var activeElement;
var observer;
var deltaBuffer = [ 120, 120, 120 ];

var key = { left: 37, up: 38, right: 39, down: 40, spacebar: 32, 
            pageup: 33, pagedown: 34, end: 35, home: 36 };


/***********************************************
 * SETTINGS
 ***********************************************/

var options = defaultOptions;


/***********************************************
 * INITIALIZE
 ***********************************************/

/**
 * Tests if smooth scrolling is allowed. Shuts down everything if not.
 */
function initTest() {

    var disableKeyboard = false; 
    
    // disable keyboard support if anything above requested it
    if (disableKeyboard) {
        removeEvent("keydown", keydown);
    }

    if (options.keyboardSupport && !disableKeyboard) {
        addEvent("keydown", keydown);
    }
}

/**
 * Sets up scrolls array, determines if frames are involved.
 */
function init() {
  
    if (!document.body) return;

    var body = document.body;
    var html = document.documentElement;
    var windowHeight = window.innerHeight; 
    var scrollHeight = body.scrollHeight;
    
    // check compat mode for root element
    root = (document.compatMode.indexOf('CSS') >= 0) ? html : body;
    activeElement = body;
    
    initTest();
    initDone = true;

    // Checks if this script is running in a frame
    if (top != self) {
        isFrame = true;
    }

    /**
     * This fixes a bug where the areas left and right to 
     * the content does not trigger the onmousewheel event
     * on some pages. e.g.: html, body { height: 100% }
     */
    else if (scrollHeight > windowHeight &&
            (body.offsetHeight <= windowHeight || 
             html.offsetHeight <= windowHeight)) {

        html.style.height = 'auto';
        //setTimeout(refresh, 10);

        // clearfix
        if (root.offsetHeight <= windowHeight) {
            var underlay = document.createElement("div"); 	
            underlay.style.clear = "both";
            body.appendChild(underlay);
        }
    }

    // disable fixed background
    if (!options.fixedBackground && !isExcluded) {
        body.style.backgroundAttachment = "scroll";
        html.style.backgroundAttachment = "scroll";
    }
}


/************************************************
 * SCROLLING 
 ************************************************/
 
var que = [];
var pending = false;
var lastScroll = +new Date;

/**
 * Pushes scroll actions to the scrolling queue.
 */
function scrollArray(elem, left, top, delay) {
    
    delay || (delay = 1000);
    directionCheck(left, top);

    if (options.accelerationMax != 1) {
        var now = +new Date;
        var elapsed = now - lastScroll;
        if (elapsed < options.accelerationDelta) {
            var factor = (1 + (30 / elapsed)) / 2;
            if (factor > 1) {
                factor = Math.min(factor, options.accelerationMax);
                left *= factor;
                top  *= factor;
            }
        }
        lastScroll = +new Date;
    }          
    
    // push a scroll command
    que.push({
        x: left, 
        y: top, 
        lastX: (left < 0) ? 0.99 : -0.99,
        lastY: (top  < 0) ? 0.99 : -0.99, 
        start: +new Date
    });
        
    // don't act if there's a pending queue
    if (pending) {
        return;
    }  

    var scrollWindow = (elem === document.body);
    
    var step = function (time) {
        
        var now = +new Date;
        var scrollX = 0;
        var scrollY = 0; 
    
        for (var i = 0; i < que.length; i++) {
            
            var item = que[i];
            var elapsed  = now - item.start;
            var finished = (elapsed >= options.animationTime);
            
            // scroll position: [0, 1]
            var position = (finished) ? 1 : elapsed / options.animationTime;
            
            // easing [optional]
            if (options.pulseAlgorithm) {
                position = pulse(position);
            }
            
            // only need the difference
            var x = (item.x * position - item.lastX) >> 0;
            var y = (item.y * position - item.lastY) >> 0;
            
            // add this to the total scrolling
            scrollX += x;
            scrollY += y;            
            
            // update last values
            item.lastX += x;
            item.lastY += y;
        
            // delete and step back if it's over
            if (finished) {
                que.splice(i, 1); i--;
            }           
        }

        // scroll left and top
        if (scrollWindow) {
            window.scrollBy(scrollX, scrollY);
        } 
        else {
            if (scrollX) elem.scrollLeft += scrollX;
            if (scrollY) elem.scrollTop  += scrollY;                    
        }
        
        // clean up if there's nothing left to do
        if (!left && !top) {
            que = [];
        }
        
        if (que.length) { 
            requestFrame(step, elem, (delay / options.frameRate + 1)); 
        } else { 
            pending = false;
        }
    };
    
    // start a new queue of actions
    requestFrame(step, elem, 0);
    pending = true;
}


/***********************************************
 * EVENTS
 ***********************************************/

/**
 * Mouse wheel handler.
 * @param {Object} event
 */
function wheel(event) {

    if (!initDone) {
        init();
    }
    
    var target = event.target;
    var overflowing = overflowingAncestor(target);
    
    // use default if there's no overflowing
    // element or default action is prevented    
    if (!overflowing || event.defaultPrevented ||
        isNodeName(activeElement, "embed") ||
       (isNodeName(target, "embed") && /\.pdf/i.test(target.src))) {
        return true;
    }

    var deltaX = event.wheelDeltaX || 0;
    var deltaY = event.wheelDeltaY || 0;
    
    // use wheelDelta if deltaX/Y is not available
    if (!deltaX && !deltaY) {
        deltaY = event.wheelDelta || 0;
    }

    // check if it's a touchpad scroll that should be ignored
    if (!options.touchpadSupport && isTouchpad(deltaY)) {
        return true;
    }

    // scale by step size
    // delta is 120 most of the time
    // synaptics seems to send 1 sometimes
    if (Math.abs(deltaX) > 1.2) {
        deltaX *= options.stepSize / 120;
    }
    if (Math.abs(deltaY) > 1.2) {
        deltaY *= options.stepSize / 120;
    }
    
    scrollArray(overflowing, -deltaX, -deltaY);
    event.preventDefault();
}

/**
 * Keydown event handler.
 * @param {Object} event
 */
function keydown(event) {

    var target   = event.target;
    var modifier = event.ctrlKey || event.altKey || event.metaKey || 
                  (event.shiftKey && event.keyCode !== key.spacebar);
    
    // do nothing if user is editing text
    // or using a modifier key (except shift)
    // or in a dropdown
    if ( /input|textarea|select|embed/i.test(target.nodeName) ||
         target.isContentEditable || 
         event.defaultPrevented   ||
         modifier ) {
      return true;
    }
    // spacebar should trigger button press
    if (isNodeName(target, "button") &&
        event.keyCode === key.spacebar) {
      return true;
    }
    
    var shift, x = 0, y = 0;
    var elem = overflowingAncestor(activeElement);
    var clientHeight = elem.clientHeight;

    if (elem == document.body) {
        clientHeight = window.innerHeight;
    }

    switch (event.keyCode) {
        case key.up:
            y = -options.arrowScroll;
            break;
        case key.down:
            y = options.arrowScroll;
            break;         
        case key.spacebar: // (+ shift)
            shift = event.shiftKey ? 1 : -1;
            y = -shift * clientHeight * 0.9;
            break;
        case key.pageup:
            y = -clientHeight * 0.9;
            break;
        case key.pagedown:
            y = clientHeight * 0.9;
            break;
        case key.home:
            y = -elem.scrollTop;
            break;
        case key.end:
            var damt = elem.scrollHeight - elem.scrollTop - clientHeight;
            y = (damt > 0) ? damt+10 : 0;
            break;
        case key.left:
            x = -options.arrowScroll;
            break;
        case key.right:
            x = options.arrowScroll;
            break;            
        default:
            return true; // a key we don't care about
    }

    scrollArray(elem, x, y);
    event.preventDefault();
}

/**
 * Mousedown event only for updating activeElement
 */
function mousedown(event) {
    activeElement = event.target;
}


/***********************************************
 * OVERFLOW
 ***********************************************/
 
var cache = {}; // cleared out every once in while
setInterval(function () { cache = {}; }, 10 * 1000);

var uniqueID = (function () {
    var i = 0;
    return function (el) {
        return el.uniqueID || (el.uniqueID = i++);
    };
})();

function setCache(elems, overflowing) {
    for (var i = elems.length; i--;)
        cache[uniqueID(elems[i])] = overflowing;
    return overflowing;
}

function overflowingAncestor(el) {
    var elems = [];
    var rootScrollHeight = root.scrollHeight;
    do {
        var cached = cache[uniqueID(el)];
        if (cached) {
            return setCache(elems, cached);
        }
        elems.push(el);
        if (rootScrollHeight === el.scrollHeight) {
            if (!isFrame || root.clientHeight + 10 < rootScrollHeight) {
                return setCache(elems, document.body); // scrolling root in WebKit
            }
        } else if (el.clientHeight + 10 < el.scrollHeight) {
            overflow = getComputedStyle(el, "").getPropertyValue("overflow-y");
            if (overflow === "scroll" || overflow === "auto") {
                return setCache(elems, el);
            }
        }
    } while (el = el.parentNode);
}


/***********************************************
 * HELPERS
 ***********************************************/

function addEvent(type, fn, bubble) {
    window.addEventListener(type, fn, (bubble||false));
}

function removeEvent(type, fn, bubble) {
    window.removeEventListener(type, fn, (bubble||false));  
}

function isNodeName(el, tag) {
    return (el.nodeName||"").toLowerCase() === tag.toLowerCase();
}

function directionCheck(x, y) {
    x = (x > 0) ? 1 : -1;
    y = (y > 0) ? 1 : -1;
    if (direction.x !== x || direction.y !== y) {
        direction.x = x;
        direction.y = y;
        que = [];
        lastScroll = 0;
    }
}

var deltaBufferTimer;

function isTouchpad(deltaY) {
    if (!deltaY) return;
    deltaY = Math.abs(deltaY)
    deltaBuffer.push(deltaY);
    deltaBuffer.shift();
    clearTimeout(deltaBufferTimer);

    var allEquals    = (deltaBuffer[0] == deltaBuffer[1] && 
                        deltaBuffer[1] == deltaBuffer[2]);
    var allDivisable = (isDivisible(deltaBuffer[0], 120) &&
                        isDivisible(deltaBuffer[1], 120) &&
                        isDivisible(deltaBuffer[2], 120));
    return !(allEquals || allDivisable);
} 

function isDivisible(n, divisor) {
    return (Math.floor(n / divisor) == n / divisor);
}

var requestFrame = (function () {
      return  window.requestAnimationFrame       || 
              window.webkitRequestAnimationFrame || 
              function (callback, element, delay) {
                  window.setTimeout(callback, delay || (1000/60));
              };
})();


/***********************************************
 * PULSE
 ***********************************************/
 
/**
 * Viscous fluid with a pulse for part and decay for the rest.
 * - Applies a fixed force over an interval (a damped acceleration), and
 * - Lets the exponential bleed away the velocity over a longer interval
 * - Michael Herf, http://stereopsis.com/stopping/
 */
function pulse_(x) {
    var val, start, expx;
    // test
    x = x * options.pulseScale;
    if (x < 1) { // acceleartion
        val = x - (1 - Math.exp(-x));
    } else {     // tail
        // the previous animation ended here:
        start = Math.exp(-1);
        // simple viscous drag
        x -= 1;
        expx = 1 - Math.exp(-x);
        val = start + (expx * (1 - start));
    }
    return val * options.pulseNormalize;
}

function pulse(x) {
    if (x >= 1) return 1;
    if (x <= 0) return 0;

    if (options.pulseNormalize == 1) {
        options.pulseNormalize /= pulse_(1);
    }
    return pulse_(x);
}

var isChrome = /chrome/i.test(window.navigator.userAgent);
var isMouseWheelSupported = 'onmousewheel' in document; 

if (isMouseWheelSupported && isChrome) {
	addEvent("mousedown", mousedown);
	addEvent("mousewheel", wheel);
	addEvent("load", init);
};

})();
//]]></script>
<script language='javascript' type='text/javascript'>(function () {
    var typist;
    typist = document.querySelector('#typist-element');
    new Typist(typist, {
                letterInterval: 60,
                textInterval: 3000
    });
}.call(this));
</script>
<!-- Min JS-->
<script language='javascript' type='text/javascript'>
    (function() {
      var a = document.getElementById(&#39;title1&#39;);
                                      var b = document.getElementById(&#39;title2&#39;);
                                      b.innerHTML = a.innerHTML;
                                      a.parentNode.removeChild(a)
      })();
    (function() {
      var a = document.getElementById(&#39;blog-pager&#39;);
                                      var b = document.getElementById(&#39;pager&#39;);
                                      b.innerHTML = a.innerHTML;
                                      a.parentNode.removeChild(a)
      })();
  </script>
<script language='javascript' type='text/javascript'>
    (function() {
      var a = document.getElementById(&#39;title4&#39;);
                                      var b = document.getElementById(&#39;title3&#39;);
                                      b.innerHTML = a.innerHTML;
                                      a.parentNode.removeChild(a)
      })();
    (function() {
      var a = document.getElementById(&#39;blog-pager&#39;);
                                      var b = document.getElementById(&#39;pager2&#39;);
                                      b.innerHTML = a.innerHTML;
                                      a.parentNode.removeChild(a)
      })();
  </script>
<!-- Min JS / End-->
<script language='javascript' type='text/javascript'>

$(&#39;.blog-pager a&#39;).attr(&#39;href&#39;, function() {
return this.href + &#39;#portfolio&#39;;

});

</script>

</body>
</html>
