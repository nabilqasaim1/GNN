<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:defaultwidgetversion='2' b:layoutsVersion='3' b:responsive='true' expr:dir='data:blog.languageDirection' expr:lang='data:blog.locale' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'><b:attr name='xmlns' value=''/><b:attr name='xmlns:b' value=''/><b:attr name='xmlns:expr' value=''/><b:attr name='xmlns:data' value=''/>
  <head>
    <script async='async' crossorigin='anonymous' src='https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-4294159533346602'/>


    <!-- Default Meta -->
    <b:include name='DefaultMeta'/>
    <!-- DNS Prefetech -->
    <b:include name='DNSPrefetech'/>
    <!-- Title -->
    <title><b:if cond='data:view.isError'><data:blog.title/></b:if><b:if cond='data:view.isMultipleItems'><b:if cond='data:view.isHomepage'><data:blog.title/><b:else/><data:blog.pageTitle.escaped/></b:if><b:elseif cond='data:view.isSingleItem'/><data:view.title.escaped/></b:if></title>
    <!-- Open Graph -->
    <b:include name='OpenGraph'/>
    <!-- Twitter Card -->
    <b:include name='TwitterCard'/>
    <!-- Feed Links -->
    <b:eval expr='data:blog.feedLinks'/>

    <!-- Required -->

    <meta content='' property='fb:pages'/>
    <meta content='' property='fb:admins'/>

    <meta content='' property='fb:app_id'/>
    <meta content='' id='disqus-id'/>

    <meta content='' name='twitter:site'/>
    <meta content='' name='twitter:creator'/>

    <b:if cond='data:view.isSingleItem'>
      <meta content='' property='article:publisher'/> 
      <meta content='' property='article:author'/>
    </b:if>


    <b:if cond='!data:view.isLayoutMode'>

      <!-- Template Skin -->
      <b:skin><![CDATA[ 
/* === Seoplus Template [Free] ====
-> Homepage: https://www.seoplus-template.com
-> Version : 2.0
-> Updated : 8 July, 2023 
*//*=================
>Variables
===================
<Group description="ألاعدادات ألاساسية" selector="body">

<Variable name="CoverImg" description="تفعيل اداة تجاوب الصور المصغرة" type="length" default="2px" min="1px" max="2px" value="2px"/>

<Variable name="StopCopying" description="تفعيل اداة منع نسخ النصوص" type="length" default="1px" min="1px" max="2px" value="1px"/>
<Variable name="RemoveAuthor" description="اخفاء اداة كاتب الموضوع" type="length" default="1px" min="1px" max="2px" value="1px"/>

<Variable name="content.width" description="Content width" type="length" min="992px" max="1300px" default="1100px" value="1100px"/>
<Variable name="sidebar.width" description="Sidebar width" type="length" min="250px" max="480px" default="330px" value="330px"/>
</Group>


<Group description="اعدادات القائمة العلوية" selector="body">
<Variable name="BacgroundHeader" description="خلفية القائمة العلوية" type="color" default="#ffffff" value="#ffffff"/>
<Variable name="LinkColor" description="لون الروابط" type="color" default="#444" value="#444444"/>
<Variable name="HLinkfont" description="حجم خط الروابط" type="font" default="400 15px sans-serif"  value="400 15px sans-serif"/>
<Variable name="Bgbuttons" description="خلفية زر البحث والقائمة " type="color" default="#035dcd" value="#035dcd"/>
<Variable name="Cobuttons" description="لون ايقونة زر البحث والقائمة " type="color" default="#fff" value="#ffffff"/>
</Group>

<Group description="ألالوان الرئيسية" selector="body">
<Variable name="body.background" description="Background" color="#f7f7f7" type="background" default="$(color) none repeat scroll top right"  value="$(color) none repeat scroll top right"/>
<Variable name="body.background.color" description="لون تبويب المدونة في الهاتف" type="color" default="#035dcd"  value="#035dcd"/>
<Variable name="keycolor" description="اللون الرئيسي" type="color" default="#035dcd" value="#035dcd"/>
<Variable name="step.color" description="اللون المساعد" type="color" default="#eee" value="#eeeeee"/>
<Variable name="grad.color" description="لون الخلفية الاساسي" type="color" default="#ffffff" value="#ffffff"/>
<Variable name="link.color" description="لون الروابط" type="color" default="#444" value="#444444"/>
<Variable name="text.color" description="لون النصوص" type="color" default="#34495e" value="#34495e"/>
<Variable name="startSide" description="start direction" type="automatic" default="right" hideEditor="true" />
<Variable name="endSide" description="end direction" type="automatic" default="left" hideEditor="true" />
</Group>

<Group description="تخصيصات المشاركات والصفحات" selector=".post-body" >
<Variable name="PostsTitleColor" description="لون عنوان ألمشاركات والصفحات" type="color" default="#171921"  value="#171921"/>
<Variable name="PostsTitleFont" description="خط عنوان المشاركات والصفحات" type="font" default="400 25px sans-serif"  value="400 25px sans-serif"/>
<Variable name="PostsTextFont" description="حجم وخط المشاركات والصفحات" type="font" default="400 16px sans-serif"  value="400 16px sans-serif"/>
<Variable name="PostsTextColor" description="لون خط المشاركات والصفحات" type="color" default="#222"  value="#222222"/>
<Variable name="PostsLinkColor" description="لون روابط المشاركات والصفحات" type="color" default="#194ca9"  value="#194ca9"/>
</Group>

<Group description='نموذج التعليقات (غير قابل للتعديل)' selector="#comments" hideEditor="true">
<Variable name="comments" description="التعليقات" hideEditor="true" type="length" default="1px" min="1px" max="1px" value="1px"/>
<Variable name="body.text.color" description="لون النص" hideEditor="true" type="color" default="#666" value="#666666"/>
<Variable name="posts.icons.color" description="خلفية ايقونة الاعلام" hideEditor="true" type="color" default="#035dcd" value="#035dcd"/>
<Variable name="body.link.color" description="لون الروابط" hideEditor="true" type="color" default="#035dcd" value="#035dcd"/>
<Variable name="posts.title.color" description="لون العنوان" hideEditor="true" type="color" default="#000" value="#000000"/>
<Variable name="labels.background.color" description="خلفيات الازرار" hideEditor="true" type="color" default="#f5f5f5" value="#f5f5f5"/>
<Variable name="BordersCommints" description="لون الفواصل" type="color" default="#eee" hideEditor="true" value="#eeeeee"/>
<Variable name="posts.background.color" description="لون الخلفية" type="color" default="transparent" hideEditor="true" value="transparent"/>
<Variable name="body.text.font" description="text font" type="font" default="600 14px &#39;Segoe UI&#39;" hideEditor="true" value="600 14px &#39;Segoe UI&#39;"/>
<Variable name="tabs.font" description="tabs font" type="font" default="14px &#39;Segoe UI&#39;" hideEditor="true" value="14px &#39;Segoe UI&#39;"/>
<Variable name="posts.text.color" description="Post text color" type="color" default="#777" hideEditor="true" value="#777777"/> 
<Variable name="labels.background.border" description="فواصل الازرار" type="color" default="#eee" hideEditor="true" value="#eeeeee"/>
</Group> 


*//*=================
>Normalize
===================*/
/* HeadLine SidePar Icon */
.clear{clear:both}

/* Css Icon */
.icon-spinner{background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 50 50' x='0px' y='0px'%3E%3Cpath d='M25.251,6.461c-10.318,0-18.683,8.365-18.683,18.683h4.068c0-8.071,6.543-14.615,14.615-14.615V6.461z' style='fill:%23989b9f;stroke:%23989b9f'%3E%3CanimateTransform attributeName='transform' attributeType='xml' dur='0.6s' from='0 25 25' repeatCount='indefinite' to='360 25 25' type='rotate'%3E%3C/animateTransform%3E%3C/path%3E%3C/svg%3E") center no-repeat}
.OpenSitting.inside:after,.search-submit2:after{content:'\2715';line-height:18px;font-size:14px;font-weight:bold;font-family:inherit}
/* Normalize */

:root{--HLinkfont:$(HLinkfont);--OldMin:$(keycolor);--startSide: $startSide;--endSide: $endSide;--maxWidth:$(content.width);--BodyBG:$(body.background);--minColorIc:$(keycolor);--minColor:$(keycolor);--minColorTran:$(keycolor)cf;--secColor:$(step.color);--thrColor:#fff;--whiteColor:$(grad.color);--hoverColor:$(keycolor);--MinBgColor:#fff;--txtColor:$(text.color);--TitColor:#444;--SanColor:#666;--Borderes:#f7f7f7;--Borderes2:#f7f7f7;--Borderes3:#eee;--PostTxtColor:$(PostsTextColor);--PostTitleColor:$(PostsTitleColor);--PostLinkColor:$(PostsLinkColor);--Hbg:$(BacgroundHeader);--HColor:$(LinkColor);--HbgIcon:$(Bgbuttons);--HCoIcon:$(Cobuttons);--HtitleColor:$(keycolor);--Cpc:$(PostsTextColor);--Cic:$(keycolor);--Hok:$(keycolor);--Sco:$(keycolor);--Gap:2px;--ImgRadius:1px;}

:root body.dark-mode{--BodyBG:#202442;--minColor:#242950;--minColorIc:#fff;--secColor:#242950;--thrColor:#1b2044;--whiteColor:#ffffff;--hoverColor:#3a7bd5;--MinBgColor:#2d325a;--txtColor:#ffffff;--TitColor:#ffffff;--SanColor:#eee;--Borderes:#262b52;--Borderes2:#3e4477;--Borderes3:#2d325a;--PostTxtColor:#eee;--PostTitleColor:#ffffff;--PostLinkColor:#3a7bd5;--Hbg:#2d325a;--HColor:#ffffff;--HtitleColor:#ffffff;--HbgIcon:#242950;--HCoIcon:#fff;--Cpc:#eee;--Cic:#fff;--Hok:#3a7bd5;--Sco:#3a7bd5;}

ul{margin:0;padding:0}*{text-decoration:none;margin:0;padding:0;outline:0;-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html,body,div,span,applet,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,abbr,acronym,address,big,cite,code,del,dfn,em,ins,kbd,q,s,samp,small,strike,strong,sub,sup,tt,var,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td{border:0;font-family:inherit;font-size:100%;font-style:inherit;color:inherit;font-weight:inherit;margin:0;outline:0;padding:0;vertical-align:baseline}img{max-height:100%;max-width:100%;position:relative}

body,input{font:400 15px sans-serif;font-optical-sizing:auto;font-style:normal;font-stretch:normal;line-height:initial}
body{background:var(--BodyBG)}
.widget{overflow:hidden}
.EndSides{overflow:hidden;clear:both;display:block}
.site .widget{display:block;clear:both;overflow:hidden;margin:0 0 20px;padding:20px;background:var(--MinBgColor);box-shadow:0 2px 6px 0 rgb(9 32 76 / 4%);border-radius:3px}
.bocker{flex-wrap: wrap;position:relative;display:flex;align-items:flex-start;justify-content:space-between;overflow: hidden;transition: none !important;}
.r-r{position:relative;width:calc(100% - $(sidebar.width) - 20px);overflow: hidden;transition: none !important;}
#sidepar-wid{width:$(sidebar.width);margin-$startSide:20px;overflow: hidden;transition: none !important;}
.Treelists{display:grid;grid-template-columns:repeat(3,1fr);gap:15px;row-gap:0}
.towcol{display:grid;grid-template-columns:repeat(2,1fr);gap:15px;row-gap:0}
.no-items{display:none!important}

.container{width:100%;max-width:$(content.width);margin:0 auto;display:block}
/* HeadLine */
.scrolhide { overflow: hidden; }

.headline,.Followers .title{position:relative;font-size:18px;padding:0 0 10px;border-bottom:2px solid var(--Borderes);display:flex;margin-bottom:15px;align-items:center;justify-content:space-between;color:var(--txtColor)}
.headline:before,.Followers .title:before{content:"";width:0;height:0;position:absolute;bottom:-6px;border-top:6px solid var(--minColorTran);right:0;left:auto;border-left:5px solid transparent;border-right:0;border-top-color:var(--minColorTran)}
.headline .title:after,.Followers .title:after{content:"";background:var(--minColorTran);width:103%;height:2px;position:absolute;bottom:-12px;background-color:var(--minColorTran);right:0;left:auto;z-index:1}
.headline .title{position:relative;float:right;color:var(--txtColor);line-height:33px}
.blocker{display:block;overflow:hidden;margin-top:15px}
a.Lapel-Link{text-align:center;transition:all 0.2s linear;float:left;color:var(--whiteColor);background:var(--minColor);position:relative;font-size:13px;padding:0 15px;border-radius:2px;height:28px;line-height:28px}

/* Stats Widget */
.Stats img{width:auto;height:auto;display:inline-block;vertical-align:-4px;-webkit-border-radius:0;-moz-border-radius:0;border-radius:0;margin-$endSide:5px}.Stats .widget-content *{vertical-align:middle}.Stats .widget-content{color:var(--TitColor);text-align:center;font-size:24px;font-family:sans-serif!important}.Stats .digit strong{background:#eee;margin:0 3px;border-radius:3px;padding:0 8px}
/* social Icon's */
aside .social-static.social li a svg{fill:#fff;width:23px;height:23px}.social-static.social li a svg{fill:#fff;width:19px;height:19px}.shmal .social-static.social li{float:$startSide;vertical-align:middle;margin-$startSide:5px;list-style:none}aside .social-static.social li{float:$startSide;vertical-align:middle;list-style:none;width:calc((100% - 15px) / 4);margin-$endSide:5px;margin-bottom:5px;padding-bottom:0;border:0}aside .social-static.social li a{background: #aaa;border-radius:5px;justify-content:center;height:50px;display:flex;align-items:center}aside .social-static.social li:nth-of-type(4n+4){margin-$endSide:0}.social-static.social{display:block;overflow:hidden;vertical-align:middle}.shmal .social-static.social li{float:$startSide;vertical-align:middle;margin-$startSide:5px;list-style:none;padding-bottom:0;margin-bottom:0;border:0}.shmal .social-static.social li a{display:flex;align-items:center;justify-content:center;width:27px;height:27px;border-radius:3px;background:#888}.shmal .social-static.social li:first-of-type{margin-$startSide:0}

/* social Icon Color's */
.social a[title="sitemap"] {background: var(--minColor) !important;}.social a[title="email"]{background-color:#ea4335!important}.social a[title="line"]{background-color:#06c152!important}.social a[title="facebook"]{background-color:#1778F2!important}.social a[title="twitter"]{background-color:#1da1f2!important}.social a[title="rss"]{background-color:#f26522!important}.social a[title="dribbble"]{background-color:#ea4c89!important}.social a[title="google-plus"]{background-color:#dd4b39!important}.social a[title="pinterest"]{background-color:#cc2127!important}.social a[title="linkedin"]{background-color:#0976b4!important}.social a[title="wordpress"]{background-color:#00769d!important}.social a[title="github"]{background-color:#000000!important}.social a[title="youtube"]{background-color:#e52d27!important}.social a[title="quora"]{background-color:#a82400!important}.social a[title="spotify"]{background-color:#1ed760!important}.social a[title="snapchat"]{background-color:#f5d602!important}.social a[title="flickr"]{background-color:#FF0084!important}.social a[title="instagram"]{background-color:#7c38af;background:radial-gradient(circle at 0 130%,#fdf497 0%,#fdf497 5%,#fd5949 45%,#d6249f 60%,#285AEB 90%)!important}.social a[title="behance"]{background-color:#009fff!important}.social a[title="whatsapp"]{background-color:#128C7E!important}.social a[title="soundcloud"]{background-color:#FF5419!important}.social a[title="tumblr"]{background-color:#3e5a70!important}.social a[title="khamsat"]{background-color:#f9b01c!important}.social a[title="tradent"]{background-color:#59c5c4!important}.social a[title="blogger"]{background-color:#fc9644!important}.social a[title="telegram"]{background-color:#32AEE1!important}.social a[title="google-play"]{background-color:#3d9dab!important}.social a[title="mostaql"]{background-color:#2caae2!important}.social a[title="messenger"]{background-color:#0084ff!important}.social a[title="paypal"]{background-color:#193685!important}.social a[title="reddit"]{background-color:#ff4500!important}.social a[title="vk"]{background-color:#45668e!important}.social a[title="website"]{background-color:#444444!important}a[title="website:before"]{content:"\f0ac"!important}
/* Style Headr */

li.item:hover > ul{opacity:1;visibility:visible;transform:translateY(0)}
li.item > ul,li.sitem > ul{height:auto!important;display:block!important;position:absolute;right:0;width:200px;background:var(--Hbg);top:60px;box-shadow:0 0 5px 1px rgb(0 0 0 / 8%);z-index:9;opacity:0;visibility:hidden;transition:all .2s linear;transform:translateY(20px);border-radius:3px;border-top:2px solid var(--OldMin)}
li.item > ul:before{content:"";width:25px;height:25px;position:absolute;background:var(--Hbg);top:-10px;right:8%;border-radius:8px;transform:rotate(45deg);box-shadow:0 0 5px 1px rgb(0 0 0 / 8%);z-index:-1;border:2px solid var(--OldMin)}
li.item > ul li.sitem{display:block!important;padding:0!important;margin:0!important;background:var(--Hbg);border-radius:3px}
li.item > ul li.sitem a{color:var(--HColor);padding:14px;margin:0!important;display:block;position:relative;background:var(--Hbg);border-radius:3px;overflow:hidden}
li.sitem > ul{transform:translateX(-30px);right:100%;top:0;border-right:2px solid var(--OldMin);border-top:0}
li.sitem > ul:before{content:"";width:26px;height:26px;position:absolute;background:var(--Hbg);top:10px;right:-10px;z-index:-1;transform:rotate(45deg);border:1px solid var(--Borderes);box-shadow:0 0 5px 1px rgb(0 0 0 / 8%);border:2px solid var(--OldMin);border-radius:8px}
li.sitem:hover > ul{transform:translateX(0);opacity:1;visibility:visible}
li.sitem:last-of-type > a{border-bottom:0!important}
li.ssitem:last-of-type > a{border-bottom:0!important}
li.ssitem{border-radius: 8px;background: var(--MinBgColor);padding:0!important;float:none;margin:0!important;width:100%}
.targetitem li a:hover:before{color:var(--hoverColor)!important}
nav.nav-par ul li a:hover{color:var(--hoverColor)}
div#menu i.fa{display:inline-block;vertical-align:middle;margin-$endSide:5px}
.icon.arrow-down{z-index: 9;transition:all .3s linear;display:block;position:absolute;top:19px;left:5px;right:auto}
.item.targetitem:hover .icon{top:23px}
.item.targetitem:hover .icon:after{transform:rotate(-45deg)}
.item.targetitem .icon:after{user-select:none;content:"";display:inline-block;width:8px;height:8px;background:transparent;border:2px solid var(--Cic);border-bottom-color:transparent;border-left-color:transparent;transform:rotate(135deg);border-radius:3px;transition:all 0.3s}
.item.targetitem .targetitem span.icon{left:13px!important;top:14px!important;right:auto!important}
.item.targetitem .targetitem:hover span.icon{$endSide:20px!important}
.item.targetitem{padding-$endSide:30px!important}
.sitem:hover  > a,.ssitem:hover > a{background:rgb(0 0 0 / 5%) !important}
.sitem.targetitem .icon:after{transform:rotate(225deg)!important;width:6px;height:6px}
/* headr sidenav  */
.pos-t-t,.Sittings{display:none;position:fixed;top:0;$endSide:0;$startSide:0;bottom:0;background-color:rgba(0,0,0,.2);backdrop-filter:saturate(100%) blur(2px);z-index:999}
#NavM:checked ~ .contenarpage .pos-t-t{display:block}
.sidenav{transition:all .3s linear;height:100vh;width:300px;position:fixed;top:0;bottom:0;right:-400px;background-color:var(--MinBgColor);z-index:9999;max-width:100%;box-shadow:-4px 0 10px 0 rgb(0 0 0 / 8%)}
#NavM:checked ~ .contenarpage .sidenav{$startSide:0}
.sidehead{position:absolute;width:45px;height:45px;left:-40px;top:20px;overflow:hidden;display:flex;align-items:center;background:var(--MinBgColor);border-radius:50% 0 50% 50%;justify-content:center;box-shadow:-2px 3px 0 0 rgb(0 0 0 / 8%);border-right:0}
.closemenu{display:flex;height:100%;color:var(--TitColor);font-size:16px;align-items:center;cursor:pointer;padding:0 19px}
.closemenu:after{content:'\2715';line-height:18px;font-size:14px;font-weight:bold}
.flexmenu{position:relative;width:100%;height:100%;display:flex;justify-content:flex-start;overflow:hidden;flex-direction:column;overflow-y:scroll;margin:0;padding-bottom:200px}
.flexmenu .MegaItem .mega-wraper{display:none!important}
.SiteInfo{padding:20px 20px  5px;border-bottom:1px solid var(--Borderes)}
.SiteInfo .navlogo img{max-width:100%;max-height:100%;display:inline-block}
.SiteInfo .navlogo{text-align: center;display:block;margin:0 auto 15px}
.SiteInfo .navtitle{display:block;padding:10px 0;font-size:21px;background:var(--Borderes);margin-bottom:15px;color:var(--txtColor);text-align:center;border-radius:5px}
.navdis{display:block;max-height:8em;overflow:hidden;margin-bottom:15px;color:var(--txtColor);opacity:.9;font-family:sans-serif!important;text-align:center}
.mainmenu{position:relative;width:100%;padding:16px}
.mainmenu ul li{position:relative;display:block;overflow:hidden;width:100%;margin:0!important}
.mainmenu ul li a{border-bottom:0!important;font-size:15px;color:var(--TitColor);padding:15px 0;display:block;border-bottom:1px solid rgb(0 0 0 / 8%)!important}
.mainmenu .item.targetitem{padding-left:0!important}
.mainmenu .targetitem ul a:before{content:'.';font-size:30px;line-height:0;display:inline-block;vertical-align:middle;margin-left:5px;top:-6px;position:relative}
.bottommeny{display:block;padding:20px;border-top:1px solid var(--Borderes)}
.bottommeny{padding-bottom:100px}
.bottpage ul li:after{content:'';font-size:27px;line-height:0;display:inline-block;vertical-align:middle;margin:0 8px;width:10px;height:1px;background:#666}
.bottpage ul{list-style:none;margin-bottom:5px}
.bottpage ul li{display:inline-block;margin-bottom:5px}
.bottpage ul li a{font-size:15px;color:var(--TitColor);font-family:sans-serif;opacity:0.8}
.bottpage ul li a:hover{opacity:1;text-decoration:underline}
.bottsocial .social-static li{display:inline-block;margin-left:10px}
.bottsocial .social-static li a{background:transparent!important}
.bottsocial .social-static li a svg{fill:var(--TitColor);opacity:0.8}
.bottsocial .social-static li a:hover svg{opacity:1}
.mainmenu .item.targetitem .icon{transform:none!important;border-radius:3px;left:0!important;top:14px!important;background:var(--secColor);color:#202124;width:30px;height:25px;line-height:25px;padding-top:4px;display:flex;align-items:baseline;justify-content:center}
.mainmenu .item.targetitem .icon:after{transform:rotate(135deg)!important}
.mainmenu ul li a i{font-size:14px;color:var(--TitColor);margin-$endSide:5px}
.sidenav .targetitem ul.open{display:block!important}
.sidenav .targetitem ul{box-shadow: none !important;position:relative!important;opacity:1!important;visibility:visible!important;transform:unset!important;display:none!important;width:auto!important;top:0!important;right:0!important;margin-top:10px;border:0!important;border-top:1px solid var(--Borderes)!important;border-bottom:1px solid var(--Borderes)!important}
.sidenav .targetitem ul:before{border:1px solid var(--Borderes);right:5%;box-shadow:none!important}
.sidenav .sitem.targetitem .icon{$endSide:5px!important;transform:rotate(180deg)!important}
.sidenav .sitem.targetitem span.icon{transform:rotate(0deg)!important}
.sidenav .targetitem.sitem ul.open{padding-right:10px;margin:3px 0;position:relative!important}
.sidenav .targetitem.sitem ul.open:before{top:-8px!important}
.mainmenu .item.targetitem span.icon,.mainmenu .item.targetitem .targetitem:hover span.icon{left:10px!important}
.mainmenu .item.targetitem.open > span.icon,.sidenav .sitem.targetitem.open > span.icon{background: var(--Sco);--Cic: #fff;}
.bottpage ul li:last-child:after{display:none}
.mainmenu .sitem:hover > a,.mainmenu .ssitem:hover > a{background:transparent!important}
/* Aside */
.FeaturedPost .item-thumbnail.thumb{margin-$endSide: 0;float: none;width:100%;padding-top: 56.25%;margin-bottom:5px}
.FeaturedPost .post-title .title{overflow:hidden;display:block;font-size:19px;color:var(--TitColor);max-height:4.9em;line-height:1.6em;background-size:0!important}
.FeaturedPost .snippet-item{color:var(--SanColor);font-size:13px;font-family:sans-serif!important;line-height:18px;margin-top:5px;overflow:hidden}.Profile .profile-img{display:block;margin:0 auto 20px;border-radius:50%}.Profile .profile-link.g-profile{color:var(--txtColor);background:var(--secColor);display:block;text-align:center;padding:10px;margin-bottom:15px;border-radius:3px;font-family:'Tajawal',sans-serif!important;font-size:inherit!important;opacity:1}.Profile .profile-data.location{display:none}.Profile .profile-textblock{color:var(--SanColor);font-size:15px;font-family:sans-serif!important;margin-bottom:15px;text-align:center;display:block}.Profile .profile-link{color:#ffffff;background:#3560ab;display:block;text-align:center;padding:10px;border-radius:3px;font-family:sans-serif!important;font-size:13px;opacity:0.7}.Profile .profile-link:hover{opacity:1}.BlogSearch input{background:transparent;font-family:sans-serif!important;color:var(--txtColor);display:inline-block;font-size:13px;padding:10px;border-radius:3px;width:55px;border:1px solid var(--Borderes)}.BlogSearch input[type="submit"]{transition:all 0.3s;background:var(--secColor);border:0;cursor:pointer}.search-input input:hover,.search-input input:focus{border-color:#4b9ce7}.search-input{display:inline-block;width:calc((100% - 60px) / 1)}.search-input input{display:block;width:100%}aside .LinkList ul li,footer .LinkList ul li,aside .PageList ul li,footer .PageList ul li{padding-bottom:8px;margin-bottom:8px;border-bottom:1px solid var(--Borderes);list-style:none}aside .LinkList ul li a,footer .LinkList ul li a,aside .PageList ul li a,footer .PageList ul li a{font-family:sans-serif!important;color:var(--TitColor);display:block}.list-label-widget-content ul li{display:block;padding-bottom:8px;margin-bottom:8px;border-bottom:1px solid var(--Borderes)}.list-label-widget-content ul li a{font-family:sans-serif!important;color:var(--TitColor);display:block}aside .LinkList ul li a:before, footer .LinkList ul li a:before, aside .PageList ul li a:before, footer .PageList ul li a:before, .list-label-widget-content ul li a:before{vertical-align:baseline;display:inline-block;width:4px;height:4px;content:"";margin-left:10px;background:transparent;border:1.7px solid var(--txtColor);border-bottom-color:transparent;border-left-color:transparent;transform:rotate(225deg);font-family:inherit!important}
.list-label-widget-content .label-count{float:$endSide;background-color:var(--minColor);text-align:center;font-size:13px;padding:0 5px;min-width:24px;height:20px;line-height:20px;color:var(--whiteColor);border-radius:2px;font-family:sans-serif!important}.list-label-widget-content li:hover .label-count{opacity:1}.cloud-label-widget-content{justify-content:center;display:flex;justify-content:flex-start;flex-wrap:wrap}span.label-size{flex-grow:1}.cloud-label-widget-content .label-count{margin-$startSide:10px;background:var(--MinBgColor);font-size:13px;padding:0 5px;min-width:20px;height:18px;line-height:18px;text-align:center;border-radius:3px;color:var(--txtColor)}
.cloud-label-widget-content .label-name{transition:all 0.3s;display:flex;padding:0 13px;justify-content:space-between;align-items:center;background:var(--minColor);font-family:sans-serif!important;margin:0 0 6px 5px;color:var(--whiteColor);font-size:15px;border-radius:3px;height:35px;line-height:35px}
input.follow-by-email-address{display:block;width:100%;height:40px;margin:15px 0;border-radius:3px;border:1px solid #efefef;text-align:center}input.follow-by-email-submit{background:#eee;border:1px solid #ccc;padding:10px;border-radius:3px;width:100%;text-align:center;color:#6b6b6b;font-size:12px;cursor:pointer}input.follow-by-email-address::placeholder{font-weight:normal;font-size:14px}div#ArchiveList ul.hierarchy{padding-$startSide:30px}div#ArchiveList ul.hierarchy ul.hierarchy{padding-$startSide:15px}div#ArchiveList ul.hierarchy ul.hierarchy ul.hierarchy  li:not(:last-of-type){margin-bottom:5px;padding-bottom:5px}div#ArchiveList ul.hierarchy li a,div#ArchiveList ul.flat li a{color:#121212}div#ArchiveList ul.hierarchy ul.hierarchy ul.hierarchy li:first-of-type{margin-top:5px;padding-top:5px}div#ArchiveList ul.hierarchy li{font-size:11px}div#ArchiveList ul.hierarchy li a:hover,div#ArchiveList ul.flat li a:hover{color:$(step.color)}div#ArchiveList .hierarchy-title{font-size:13px;margin-bottom:5px;padding-bottom:5px;border-bottom:1px solid #f7f7f7}div#ArchiveList .hierarchy-title span.post-count,div#ArchiveList ul.flat li span.post-count{float:$endSide;width:25px;padding:0 0;text-align:center;background:#eee;border-radius:3px;border:1px solid #ccc;font-size:12px;font-weight:normal}div#ArchiveList ul.flat{padding-$startSide:30px}div#ArchiveList ul.flat li:not(:last-of-type){margin-bottom:5px;padding-bottom:5px}div#ArchiveList ul.flat li{font-size:13px}.ContactForm textarea[name="email-message"],.ContactForm input[type="text"]{margin:0 auto 10px;border:1px solid var(--Borderes);width:100%;border-radius:3px;padding:10px 15px;background:transparent;font-family:sans-serif!important}.ContactForm textarea[name="email-message"]:hover,.ContactForm input[type="text"]:hover,.ContactForm textarea[name="email-message"]:focus,.ContactForm input[type="text"]:focus{border:1px solid #4b9ce7}textarea[name="email-message"]{min-height:130px;resize:vertical}.ContactForm input[type="button"]{transition:all 0.3s;display:inline-block!important;position:relative;font-size:14px;background:var(--secColor);color:var(--txtColor);padding:7px 20px;border-radius:3px;font-family:sans-serif!important;border:none;float:$endSide;cursor:pointer}p#ContactForm1_contact-form-error-message{font-family:sans-serif!important}p#ContactForm1_contact-form-success-message{font-family:sans-serif!important;color:#30bb81}
/* nextprev  */
.page-navigation{display:flex!important;align-items:center;justify-content:space-between}div#siki_next a,div#siki_prev a{width:42px;height:42px;display:flex;align-items:center;justify-content:center;background:var(--minColor);color:var(--whiteColor);font-size:25px;border-radius:3px}.sikinot{opacity:0.7}.sikinot a{pointer-events:none}div#siki-page-number{font-size:16px;font-family:sans-serif;color:var(--txtColor)}
/* InPost And Page*/
.post-body{font:$(PostsTextFont);line-height:2em;overflow:hidden;color:var(--PostTxtColor)}.post-body a{color:var(--PostLinkColor)}.post div#Blog1,.post .post-outer,.post .post-body{overflow:initial!important}.post div#Blog1,.page div#Blog1{display:block;background:transparent;border-radius:0;padding:0;border:0;margin:0;box-shadow:none;margin-bottom:15px}.bobxed,.commentsection,.pSh,.post-tags,.shareButton,.RelatedPosts,.author-posts,.post-body,.page-navigation{display:block;background:var(--MinBgColor)!important;clear:both;padding:20px!important;overflow:hidden;border-bottom:1px solid var(--Borderes)}
.post .post-body p{margin:1.5em 0}
.post-body h1:not(.rnav-title),.post-body h2:not(.rnav-title),.post-body h3:not(.rnav-title),.post-body h4:not(.rnav-title){margin:1em 0;line-height:1.5em}
.post-body h1{font-size:1.9rem}
.post-body h2{font-size:1.7rem}
.post-body h3:not(.rnav-title){font-size:1.5rem}
.post-body h4{font-size:1.4rem}
.post-body sup {vertical-align: super;font-size: smaller !important;}
.post-body sub {vertical-align: sub;font-size: smaller;}
.post-meta{display:flex;align-items:center;justify-content:space-between;margin-top:15px}.au-ti{height: 36px;display:flex;align-items:center;justify-content:flex-start;font-size:13px}
.metapost{display:inline-flex;flex-wrap:wrap;align-items:center;justify-content:center;line-height:20px}
.Times{display:inline-block;white-space:nowrap;text-overflow:ellipsis;overflow:hidden;max-width:100%}
.Times > div{display:inline}
.authorname{margin-$endSide:8px}
.authorPhoto{width:36px;height:36px;object-fit:cover;border-radius:8px;margin-left:5px}
.article-timeago,.readTime{opacity:.7}
.readTime:before{content:'';margin:0 5px;width:13px;height:1px;background:var(--txtColor);display:inline-block;vertical-align:middle}
.article-author,.article-timeago,.readTime{display:flex;align-items:center;justify-content:center;color:var(--txtColor)}
.topcs7v{margin-bottom:15px;position:relative;width:100%;display:flex;flex-direction:column;overflow:hidden;border-top:1px solid var(--Borderes)}
.toctitle{border-bottom:1px solid var(--Borderes);cursor:pointer;position:relative;height:55px;font-size:16px;color:var(--txtColor);display:flex;align-items:center;justify-content:flex-start;padding:0 15px;margin:0;width:100%}
.toctitle:before{content:'\002B';margin-left:10px;font-size:21px}
.toctitle:after{content:"عرض الكل";float:left;font-family:sans-serif;margin-right:10px;font-size:13px;position:absolute;left:15px;text-align:center;line-height:26px;border-radius:3px;opacity:0.9}
#tocList{padding:0 20px 15px;display:none;border-bottom:1px solid var(--Borderes)}
#tocList li{list-style:decimal inside;font-size:14px;line-height:1.7;margin-bottom:0;padding-bottom:0;color:var(--txtColor);opacity:.8}
#tocList li a{color:var(--txtColor)}
#tocList li:hover{opacity:1;text-decoration:underline}
.closed .toctitle:before{content:'\2212'}
.closed #tocList{display:block}
.toctitle:hover,.closed .toctitle{background:var(--Borderes)}
.closed .toctitle:after{content:'أخفاء الكل'}
.tr-caption{font-family:sans-serif!important;opacity:.8;font-size:14px;line-height:1.5em}
.post-body img{border-radius:3px;width:auto;height:auto;display:inline}
.separator,.separator a,a[imageanchor="1"],a[style*='1em']{text-align:center;margin:0!important}
.post-body strike{text-decoration:line-through}
.post-body u{text-decoration:underline}
.post-body ul,.post-body ol{padding:0 15px 0 0;margin:10px 0}
.post-body li{margin:5px 0;padding:0}
.post-body ul li{list-style:disc inside}
.post-body ol li{list-style:decimal inside}
.post-body ul ul li{list-style:circle inside}
.post-body blockquote{overflow:hidden;position:relative;background-color:rgba(155,155,155,0.05);color:var(--PostTxtColor);padding:15px 25px;margin:0;font-size:15px;border-$startSide:3px solid rgba(155,155,155,0.2)}
.post-body blockquote *{display:initial!important}
div#AddOns{display:none;opacity:0;visibility:hidden}
.post-amp .topic-title{overflow:hidden;font:$(PostsTitleFont);line-height:1.7em;color:var(--PostTitleColor)}
.hideensa{overflow:hidden;display:block;clear:both}
.foqTitle{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px}
.FTBU{display:flex}
.postTopTag{color:var(--whiteColor);background:var(--minColor);font-size:13px;padding:4px 13px;border-radius:3px}
.postTopTag:hover{background:var(--minColor)}
.OpenSitting,.gocomments{cursor:pointer;margin-right:10px;width:40px;height:28px;display:flex;align-items:center;justify-content:center;position:relative;border-radius:3px;border:1px solid rgb(0 0 0 / 5%)}
.gocomments{margin:0}
.OpenSitting:hover,.gocomments:hover{background:rgb(0 0 0 / 6%)}
.gocomments svg,.OpenSitting svg{width:18px;height:18px;fill:var(--minColorIc)}
.numcomment{position:absolute;top:-10px;right:-5px;background:#ddd;padding:0 7px;color:#333;font-size:13px;border-radius:3px}
.post-tags{flex-wrap:wrap;padding-bottom:15px!important;display:flex;align-items:center;justify-content:flex-start}
.post-tags a{background:rgba(0,0,0,5%);color:var(--txtColor)}
.post-tags .tagstitle{background:var(--minColor);color:var(--whiteColor);margin-$endSide:10px}
.post-tags span,.post-tags a{margin-bottom:5px;flex-shrink:0;transition:all 0.3s;border-radius:2px;padding:0 10px;line-height:26px;margin-$endSide:7px;position:relative;font-size:13px}
.tagstitle:before{content:'';position:absolute;top:10px;$endSide:-3px;width:6px;height:6px;background-color:var(--minColor);transform:rotate(45deg)}

/* SeoPlusAds  */
div#Topa3lan-sc .HTML,div#Topa3lan-sc2 .HTML{box-shadow:none;background:transparent!important;padding:0!important;border:0;margin:0}div#PostA3lan .widget,div#PostA3lan2 .widget{background:transparent!important;border:0!important;padding:0 20px!important;margin:0!important;box-shadow:none!important}
#Blog1 .clearhtml > .HTML{background:var(--MinBgColor)!important;margin:0;padding:20px 0!important;border-bottom:1px solid var(--Borderes)}
.SeoPlusAds,#Blog1 .HTML{font-family:sans-serif;background:transparent!important;margin:15px 0;text-align:center;font-size:13px;display:block;clear:both;border:none;overflow:unset!important;box-shadow:none;padding:0!important;border-radius:0}div#HTML100 .SeoPlusAds{margin-top:0}div#top-a3lan .HTML{margin-top:0}div#bot-a3lan .HTML{margin-bottom:0}.pnavigation .HTML{margin-bottom:15px!important}div#bot-a3lan,div#top-a3lan,div#ret-a3lan{overflow:initial}div#ret-a3lan .HTML{background:var(--MinBgColor)!important;padding:15px 0!important;margin:0!important;border-bottom:1px solid var(--Borderes)}
/* comments */
.bloggerComment{background:#fc9644}
.comments-tabs .active,.comments-tabs span:hover{opacity:1}
.noimg{background:transparent url(https://4.bp.blogspot.com/-ci3XMoAMGzg/WiCTxCLLWeI/AAAAAAAAPjI/UkV1sBTKC7EamOC_UmMJ4cQCv4xNNI82QCLcBGAs/s83/log.jpg) no-repeat center;display:block;width:38px;height:38px;background-size:38px}
.avatar-image{width:38px;height:38px;position:absolute;top:0;right:0;border-radius:8px;overflow:hidden}
.CommentCounter{position:relative}
.cmt-user{font-family:sans-serif!important;font-size:14px;color:var(--txtColor)}
.comment-block{padding-right:45px}
.comment{position:relative;padding:0;margin:15px 0 0;padding-top:15px;list-style:none;border-radius:0;border-top:1px solid rgb(0 0 0 / 2%)}
.comment-replies{padding-right:45px}
.comment .comment-replies .comment:not(:first-child){border-top:0}
.comments .comment-content{font-size:14px;color:var(--Cpc);line-height:1.6em;margin:6px 0 10px;padding:10px;background:rgb(0 0 0 / 5%);border-radius:12px 2px 12px 12px;display:inline-block;white-space:pre-wrap}
.comments .comment-actions{display:flex;margin:0;align-items:center}
.comment-actions .comment-reply,.comment-actions a{margin-left:10px;font-size:13px;color:var(--txtColor);cursor:pointer;font-family:sans-serif!important;line-height:1em}
.comment-actions .comment-reply{padding-left:10px;border-left:1px solid rgb(9 32 76 / 2%)}
.comment-actions .comment-reply:hover,.comment-actions a:hover{text-decoration:underline}
.ShowMoreCMT,.PostEdit a{display:inline-block;padding:7px 22px;text-align:center;font-size:15px;background:var(--minColor);margin-top:20px;cursor:pointer;border-radius:3px;color:var(--whiteColor);line-height:1.3em;transition:all .2s linear}
#comments-respond,.comment-replies #comment-editor{padding:15px;border-radius:8px;border:1px solid rgb(9 32 76 / 2%);background:rgb(9 32 76 / 2%);min-height:100px}
.comment-replies #comment-editor{margin-top:10px}
.conart{margin-bottom:10px;display:block;padding-bottom:15px;border-bottom:1px solid rgb(9 32 76 / 5%)}
#comment-post-message{font-size:15px;color:var(--txtColor);display:inline-block;background:rgb(0 0 0 / 5%);padding:4px 10px;border-radius:3px}
#comment-post-message:hover{background:rgb(0 0 0 / 8%)}
.conart p{font-size:15px;font-family:sans-serif!important;color:var(--txtColor);margin-top:5px}

/* author profile  */
.authorImage{float:$startSide;width:60px;height:60px;margin-$endSide:15px}.authorImage .authorImg{overflow:hidden;width:60px;height:60px}.authorInfo{width:calc(100% - 75px);float:$startSide;margin-top:5px}.author-posts{display:flex!important;align-items:flex-start}.author-name{font-size:18px;color:var(--txtColor);margin-bottom:12px}.author-desc{font-family:sans-serif!important;color:var(--SanColor);font-size:14px}

/* footer  */
footer{overflow:hidden;display:block;clear:both;background:var(--MinBgColor);border-top:1px solid var(--Borderes3)}.mid-top-footer{overflow:hidden;display:flex;justify-content:space-between}.footer-col{padding:0 10px;width:100%;min-width:25%}.footer-col.no-items{display:none}footer .container{display:block;overflow:hidden}.mid-top-footer .footer-col .widget{margin-top:15px;margin-bottom:30px;vertical-align:top}.mid-top-footer .footer-col .widget:last-of-type{margin-bottom:20px}.bottom-footer .container{padding:0 15px}.bottom-footer{display:block;overflow:hidden;clear:both;padding:10px 0;border-top:1px solid var(--Borderes3);margin-top:0}.yemen{min-height:32px;font-size:13px;float:$startSide;display:flex;align-items:center;color:var(--TitColor)}.yemen a{font-size:14px;color:var(--Hok);letter-spacing:0;vertical-align:middle}.yemen span{font-size:14px;vertical-align:middle;margin-$endSide:3px}.shmal{float:$endSide;font-size:13px;margin-top:5px}svg.svg-inline--fa.fa-exclamation-triangle.fa-w-18{width:200px;margin:0 auto 0;display:block;height:200px;color:var(--minColor)}
/* post-share */
.n-line{width:19px;height:19px;fill:#fff;margin:0 3px}
.shC .n-line{width:22px;height:22px}
.pShc{display:flex;align-items:center;flex-wrap:wrap;position:relative;width:calc(100% + 18px);font-size:13px}
.pShc::before{content:attr(data-text);margin-left:10px;flex-shrink:0;color:var(--txtColor);font-size:14px}
.pShc .c::after{content:attr(aria-label);margin:0 3px}
.pShc >*{cursor:pointer;margin:0 5px;display:flex;align-items:center;color:inherit;padding:8px 12px;border-radius:5px;background:rgba(0,0,0,5%)}
.sharemore:hover{background:rgba(0,0,0,8%)}
.pShc .tw{background:#1DA1F2}
.pShc .c{color:#fffdfc}
.pShc .wa{background:#128C7E}
.pShc .fb{background:#1778F2}
.fixi:checked ~ .fixL{opacity:1;visibility:visible}
.fixL{display:flex;align-items:center;position:fixed;left:0;right:0;bottom:0;z-index:20;transition:all .1s linear;width:100%;height:100%;opacity:0;visibility:hidden}
.sharemore svg{fill:var(--txtColor)}
.fixLi{width:100%;max-width:520px;max-height:calc(100% - 60px);border-radius:5px;transition:inherit;z-index:3;display:flex;overflow:hidden;position:relative;margin:0 auto;box-shadow:0 5px 30px 0 rgb(0 0 0 / 5%)}
.fixLs{padding:60px 20px 20px;overflow-x:hidden;width:100%;background:var(--MinBgColor)}
.shL,.fixH{color:var(--txtColor)}
.fixH{display:flex;background:inherit;position:absolute;top:0;left:0;right:0;padding:0 10px;z-index:2}
.fixT::before{content:attr(data-text);flex-grow:1;padding:16px 10px;font-size:90%;opacity:.7}
.fixH .cl{padding:0 10px;display:flex;align-items:center;justify-content:flex-end;position:relative;flex-shrink:0;min-width:40px;cursor:pointer}
.fCls.sharebg{cursor:pointer}
.fixT .c::before{content:attr(aria-label);font-size:11px;margin:0 8px;opacity:.6}
.fixH .c::after{content:'\2715';line-height:18px;font-size:14px}
.shL{position:relative;width:calc(100% + 20px);left:-10px;right:-10px;display:flex;flex-wrap:wrap;justify-content:center}
.shL >*{margin:0 10px 20px;text-align:center}
.shL a{display:flex;align-items:center;justify-content:center;flex-wrap:wrap;width:60px;height:60px;color:inherit;margin:0 auto 5px;padding:8px;border-radius:5px;background:#5a5a5a}
.shL >*::after{content:attr(data-text);font-size:90%;opacity:.7;display:block}

.fCls{display:block;position:fixed;top:-50%;left:-50%;right:-50%;bottom:-50%;z-index:1;transition:all .1s linear;background:transparent;opacity:0;visibility:hidden}

.fixi:checked ~ .fixL .sharebg, #NavC:checked ~ .searchformbox .searchbg{opacity:1;visibility:visible;background:rgba(0,0,0,.2);-webkit-backdrop-filter:saturate(100%) blur(2px);backdrop-filter:saturate(100%) blur(2px)}
@media screen and (max-width: 640px){
.fixL{align-items:flex-end}
.fixL .fixLi,.fixL .cmBri{border-radius:12px 12px 0 0}
.pShc .c::after{display:none}
}
.post-body iframe{display:block;margin:auto;max-width:100%}
iframe {color-scheme: none;}
.contenarpage{overflow:hidden}
/* new worck */
.loadMore{display:flex;align-items:center;justify-content:center;font-size:90%;color:#fffdfc;margin:20px 0 0;max-width:100%}
.loadMore div{transition:all .2s linear;cursor:pointer;display:flex;align-items:center;user-select:none;padding:0 20px;background:var(--minColor);border-radius:3px;height:35px;line-height:35px}
#loadMoreWait,#loadMoreNomore{background:var(--secColor);color:#989b9f;display:none;user-select:none}
.blog-posts{display:block}
.post .blog-posts{box-shadow:0 2px 6px 0 rgb(9 32 76 / 4%);border-radius:3px}
/* blog-pager2 */
.topic-nav{display:flex;align-items:center;justify-content:center}div#blog-pager{display:flex;align-items:center;justify-content:center;overflow:hidden;clear:both;margin:15px 0 0;padding:15px 0 0;border-top:1px solid var(--Borderes3)}.blog-pager{height:36px;width:40px;display:flex;align-items:center;justify-content:center;overflow:hidden;border-radius:3px;margin:0 2px;color:#fff;background:var(--minColor)}.blog-pager i.icon{font-size:14px;text-align:center;line-height:36px}.homelink i.icon{font-size:16px}
/* Pagecontactus */
div#ContactForm200{display:none}div#Pagecontactus .widget{border:0!important;padding:0;box-shadow:none;margin:0 0;min-height:385px;display:block}div#Pagecontactus{min-height:385px}div#Pagecontactus .widget p{margin:0}
/* Hovers */


.post-tags a:hover,
.Lapel-Link:hover,
.BlogSearch input[type="submit"]:hover,
.cloud-label-widget-content .label-name:hover,
.list-label-widget-content li:hover .label-count,
.ContactForm input[type="button"]:hover,
.moreLink:hover,.caregory-div a:hover{color: var(--whiteColor);background: var(--minColor);}

tbody,table{width:100%;max-width:100%}body.dark-mode input,body.dark-mode textarea{color:#fff}body.dark-mode .ContactForm textarea[name="email-message"]::placeholder,body.dark-mode .ContactForm input[type="text"]::placeholder{color:#fff}
.dark-mode g.d1{display:none}
.dark-mode g.d2{display:block}

/*=================
responsev [not completed]
===================*/

@media screen and (max-width:992px){
#sidepar-wid{width:250px}.r-r{width:calc((100% - 255px - 15px) / 1)}
.mid-top-footer{flex-wrap:wrap}.footer-col{width:50%}
}
@media screen and (max-width:860px){
.ReadPage-popup-cont {margin: 0;height: 100%;padding-bottom: 50px;}
.bocker {display: block;}
.r-r, #sidepar-wid {transform: none !important;float: none;width: 100%!important;margin: 0;display: block;}
}
@media screen and (max-width:720px){
span.modal-close{$endSide:5px;top:-15px}
.bottom-footer{box-shadow:none}
.bottom-footer .yemen{min-height:auto;display:block!important;float:none;text-align:center;margin-bottom:10px}
.yemen a[title="SeoPlus Template"]{display:inline-block!important}
.bottom-footer .shmal{float:none;margin-top:0;margin:0 auto;text-align:center}
.bottom-footer .shmal .social-static.social{flex-wrap:wrap;display:flex;overflow:hidden;vertical-align:middle;align-items:flex-start;justify-content:center}
.bottom-footer .shmal .social-static.social li{margin-bottom:5px}
.metapost{width:calc(100% - 33px)}
}
@media screen and (max-width:640px){
.commentsection .headline:before,.commentsection .headline .title:after{display:none}
.headline,.Followers .title{font-size:17px}
.metapost{justify-content:flex-start;flex-direction:column;align-items:flex-start}

.site .widget,.post .blog-posts { border-right: 0 !important; border-left: 0 !important; }
.comment-content iframe {height: 200px;}
.comment-content img{height: auto;}
.textst{font-size:35px}span.datetime.com-date{float:none!important;display:block}
.search-submit2{$endSide:-10px}
.footer-col{width:100%}
#item-comments .headline{flex-direction:column}
#item-comments .headline .title{margin-bottom:5px}
.commentsShow{display:flex;align-items:center;justify-content:center;text-align:center}
}
/* New Edit's */
.potg .Sp-slide .Posts-byCategory,.potg .Sp-slide2 .Posts-byCategory,.potg .Sp-slide3 .Posts-byCategory,,.potg .Sp-slide4 .Posts-byCategory,.btg2 .Sp-posts1 .Posts-byCategory,.btg2 .Sp-posts2 .Posts-byCategory,.btg2 .Sp-posts5 .Posts-byCategory,.btg2 .Sp-postsnew .Posts-byCategory{display:none}
.potg .Sp-slide:before,.potg .Sp-slide2:before,.potg .Sp-slide3:before,.potg .Sp-slide4:before,.btg2 .Sp-posts1:before,.btg2 .Sp-posts2:before,.btg2 .Sp-posts5:before,.btg2 .Sp-postsnew:before{content:'\f12a';font-family:'FontAwesome';margin-$endSide:5px}
.potg .Sp-slide:after,.potg .Sp-slide2:after,.potg .Sp-slide3:after,.potg .Sp-slide4:after,.btg2 .Sp-posts1:after,.btg2 .Sp-posts2:after,.btg2 .Sp-posts5:after,.btg2 .Sp-postsnew:after{content:"لأ يمكنك استخدام هذا الشكل في هذا المكان"}
.potg .Sp-slide,.potg .Sp-slide2,.potg .Sp-slide3,.potg .Sp-slide4,.btg2 .Sp-posts1,.btg2 .Sp-posts2,.btg2 .Sp-posts5,.btg2 .Sp-postsnew{display:block;overflow:hidden;font-size:16px;height:50px;padding:0 10px;line-height:50px;text-align:center;color:#721c24;background-color:#f8d7da;border:1px solid #f5c6cb;border-radius:3px}
.moreLink{transition:all 0.2s linear;background:var(--minColor);color:var(--whiteColor)}
.postTags .HTML .headline{opacity:0}
.post-frome-tag .headline{opacity:1!important}
.Img-Holder{background:var(--Borderes)}
.Img-Holder img{opacity:0}
.Img-Loaded img{opacity:1}
.rnav-title a,.post-title .title{background:linear-gradient(to right,currentColor 0%,currentColor 100%);background-size:0 1px;background-repeat:no-repeat;background-position:right 85%;transition:background 0.3s;padding-bottom:7px;display:inline;line-height:1.6em;color:var(--TitColor)}
.rnav-title a:hover,.post-title .title:hover{background-size:100% 1px}
.rnav-title{clear:both;font-size:16px}
.thumb{transition:all .3s linear;float:$startSide;margin-$endSide:15px;display:block;border-radius:var(--ImgRadius);overflow:hidden;position:relative}
.thumb img{transition:all .3s linear;border-radius:0;object-fit:cover;display:block;width:100%;height:100%;position:absolute;top:0;right:0;left:0;bottom:0}
.posts-from{font-style:normal;display:flex;align-items:center;justify-content:center;min-height:410px;flex-direction:column}
.posts-from[data-type="Sp-shreet"]{min-height:inherit!important}
.posts-from[data-type="Sp-shreet"]:before{display:none}
.posts .Date svg{display:inline-block;width:10px;height:10px;vertical-align:middle;margin-left:5px;fill:var(--SanColor)}
.posts .Date{display:block;position:relative}
.posts .Date a{color:var(--SanColor);display:inline-block;vertical-align:middle;font-size:12px;font-family:sans-serif!important}
.posts .author{display:block;font-size:15px}
.postcat{position:absolute;top:10px;right:10px;display:inline-block;background:var(--minColor);color:#fff;padding:0 10px;font-size:12px;font-family:sans-serif!important;transition:.3s;z-index:2;border-radius:2px;height:25px;line-height:25px}
.postcat.catnum0{background:#95281C}
.postcat.catnum1{background:#1B5A84}
.postcat.catnum2{background:#2C3E50}
.postcat.catnum3{background:#1A5D50}
.postcat.catnum4{background:#0A3D62}
.postcat.catnum5{background:#A41138}
.postcat.catnum6{background:#0C2461}
.postcat.catnum7{background:#850021}
.postcat.catnum8{background:#04626A}
.postcat.catnum9{background:#3C40C6}

.thumb:after{content:"";position:absolute;z-index:1;$endSide:0;$startSide:0;bottom:0;height:100%;background:rgb(0 0 0 / 26%);opacity:0;transition:all 0.3s}.lapel .posts:hover .thumb:after,.post .posts:hover > .thumb:after,.item-thumbnail:hover{opacity:1}.Sp-posts4 .Short_content,.Sp-posts3 .Short_content,.Sp-posts4 .posts:not(.postnum0) .thumb .postcat,.Sp-posts3 .postcat,.Sp-posts3.noImg .thumb,.Sp-postsnew0.noImg .thumb,.Sp-3colList.noImg .thumb,.Sp-postsnew.noImg .thumb,.Sp-posts1 .Short_content,.Sp-3colList .posts .postcat,.moreLink,.Short_content,.Sp-shreet .Short_content,.Sp-slide3 .posts:not(.postnum0) .cont .Short_content,.Sp-slide3 .posts:not(.postnum0):not(.postnum1):not(.postnum2) .items a.author,.Sp-slide4 .posts:not(.postnum0) .cont .Short_content,.Sp-slide2 .posts:not(.postnum0) .Short_content,.Sp-posts5 .posts:not(.postnum0) .Short_content,.Sp-posts5 .posts:not(.postnum0) .postcat,.posts .items,
.block-side,
.Sp-shreet .posts .Date, .Sp-shreet .thumb .Noimger,
.SiteInfo:empty,
.modal-body.post-body .redirectSkin.blog-admin,
.readMode .PostByCatRandom, .readMode div#tocDiv,.readMode li.tag-link,
.dark-mode g.d1,
.Sp-posts6 .thumb,
.PopularPosts .Noimg a.item-thumbnail.thumb,
.Sp-posts4.noImg .posts .thumb,
aside .post-frome-tag .headline .Lapel-Link,footer .post-frome-tag .headline .Lapel-Link,
.page .reaction-buttons,
.LinkList .social li a:before
{display:none!important}

.Sp-shreet .rnav-title a:hover,.Sp-posts4 .posts:not(.postnum0) .rnav-title a:hover,.Sp-posts1 .rnav-title a:hover,.Sp-posts3 .rnav-title a:hover,.Sp-posts6 .rnav-title a:hover,.Sp-postsnew .posts .rnav-title a:hover,.Sp-posts5 .posts .rnav-title a:hover,.Sp-3colList .rnav-title a:hover,.list-label-widget-content ul li a:hover,.PopularPosts h3.post-title .title:hover,.FeaturedPost .post-title .title:hover,.posts .Date:hover a,.Sp-postsnew0 .posts .rnav-title a:hover,.posts .Date:hover:before{color:var(--hoverColor)!important},.Sp-3colList .posts:nth-last-child(-n+3),.Sp-posts4 .posts:last-of-type,.Sp-posts6 .posts:last-of-type,.PopularPosts article.post:last-of-type,aside .LinkList ul li:last-of-type,footer .LinkList ul li:last-of-type,aside .PageList ul li:last-of-type,footer .PageList ul li:last-of-type,.Sp-postsnew0 .posts:last-of-type,.list-label-widget-content ul li:last-of-type{padding-bottom:0!important;margin-bottom:0!important;border-bottom:0!important}


/* post posts1 */
.Sp-posts1 .Posts-byCategory,.Sp-posts2 .Posts-byCategory,.Sp-postsnew .Posts-byCategory{display:grid;grid-gap:15px}
.Sp-posts2 .posts{position:relative}
.fullwide .Sp-postsnew .Posts-byCategory{grid-template-columns:repeat(3,1fr)}
.potg .Sp-postsnew .Posts-byCategory{grid-template-columns:repeat(2,1fr)}
.fullwide .Sp-posts1 .Posts-byCategory{grid-template-columns:repeat(4,1fr)}
.potg .Sp-posts1 .Posts-byCategory{grid-template-columns:repeat(3,1fr)}
.Sp-posts2 .Posts-byCategory{grid-template-columns:repeat(3,1fr);gap:var(--Gap)}
.Sp-posts1 a.thumb,.Sp-posts8 a.thumb{margin:0;width:100%!important;padding-top:68.17%;position:relative}
.Sp-slide .posts .thumb:before,.Sp-slide2 .posts .thumb:before,.Sp-slide3 .posts .thumb:before,.Sp-slide4 .posts .thumb:before,.Sp-posts4 .postnum0 .thumb:before,.Sp-posts7 .thumb:before{content:"";position:absolute;z-index:1;$endSide:0;$startSide:0;bottom:0;height:65%;transition:opacity 0.2s;background-image:linear-gradient(to bottom,transparent,rgba(0,0,0,0.75))}

.Sp-postsnew0 .Posts-byCategory{display:grid;gap:15px;grid-template-columns:1fr}
.Sp-postsnew0 .posts{display:flex}
.Sp-postsnew0 .posts .thumb{width:300px;height:170px;flex-shrink:0}
.Sp-postsnew0 .posts .cont{width:calc((100% - 315px) / 1);flex-shrink:0}
.Sp-postsnew0 .posts .rnav-title a{font-size:21px}
.Sp-postsnew0 .posts .Short_content{color:var(--SanColor);font-size:13px;font-family:sans-serif!important;line-height:21px;margin-top:5px;overflow:hidden;height:63px;display:block!important}
.Sp-postsnew0.noImg .posts .cont{width:100%}
.Sp-postsnew .posts .moreLink,.Sp-postsnew0 .posts .moreLink{display:inline-block!important;position:relative;font-size:14px;padding:0 20px;border-radius:3px;margin-top:10px;height:30px;line-height:30px}


/* posts3+6  */
.Sp-posts3 .Posts-byCategory,.Sp-posts4 .Posts-byCategory,.Sp-3colList .Posts-byCategory,.PopularPosts .ImgShow{gap:15px;display:grid;grid-template-columns:1fr}
.Sp-3colList .Posts-byCategory{grid-template-columns:repeat(3,1fr)}
.Sp-posts4 .posts.postnum0 .thumb{width:100%;padding-top:56.25%;margin:0!important}
.Sp-posts3 .Posts-byCategory .posts,.Sp-posts4 .posts:not(.postnum0),.Sp-posts5 .posts:not(.postnum0),.Sp-3colList .posts,.PopularPosts .ImgShow .post{display:flex}
.Sp-posts4 .posts:not(.postnum0) .cont,.Sp-posts3 .cont,.Sp-3colList .cont,.PopularPosts h3.post-title,.Sp-posts5 .posts:not(.postnum0) .cont{width:calc(100% - 125px);flex-shrink:0}
.Sp-posts3 .posts .thumb,.Sp-posts4 .thumb,.Sp-3colList .thumb,.PopularPosts a.item-thumbnail.thumb,.Sp-posts5 .posts:not(.postnum0) .thumb{width:110px;height:75px;flex-shrink:0}
.Sp-posts3 .posts:not(.postnum0) .rnav-title a,.Sp-posts4 .rnav-title a,.Sp-posts6 .rnav-title a,.Sp-3colList .rnav-title a,.PopularPosts h3.post-title .title{font-size:14px}
.PopularPosts .post-title .title{background-size:0!important;display:block;max-height:4.9em;overflow:hidden}
.3colList.noImg .cont{width:100%}
.Sp-posts6 .cont,.PopularPosts .Noimg .posts.post-title{width:100%}
.caregory-div a{background:var(--minColor);padding:4px 20px;display:table;border-radius:3px;font-size:15px;line-height:1.6em;color:var(--whiteColor)}
.ArchivePage{min-height:450px;display:block}
.Sp-posts6.archive{margin-bottom:15px}
.Sp-posts6.archive .Date{line-height:1.5em}
.Sp-posts6 .Posts-byCategory:before,.PopularPosts .Noimg:before{content:"";position:absolute;$startSide:0;top:0;width:2px;height:100%;background:rgba(0,0,0,0.3)}
.Sp-posts6 .Posts-byCategory,.PopularPosts .Noimg{overflow:unset;padding-$startSide:15px;margin-$startSide:10px;position:relative}
.Sp-posts6 .Date:after,.PopularPosts .Noimg .Date:after{content:"";width:12px;height:12px;background:#e6e6e6;border:1px solid rgba(255,255,255,0.8);position:absolute;display:inline-block;vertical-align:middle;border-radius:3px;transform:translateZ(0);transition-duration:0.3s;$startSide:-21px;border-color:rgba(0,0,0,0.3);top:5px}
.Sp-posts6 .posts:hover .Date:after,.PopularPosts .Noimg  article.post:hover .Date:after{background:#3560ab;transform:scale(1.2)}
.Sp-posts6 .posts,.PopularPosts .Noimg article.post{overflow:unset;margin-bottom:15px}



@media screen and (max-width:850px){

.Sp-slide .Posts-byCategory,.Sp-slide2 .Posts-byCategory,.Sp-slide3 .Posts-byCategory,.Sp-slide4 .Posts-byCategory{grid-template-columns:repeat(2,1fr)}
.Sp-slide .postnum0{grid-column:span 2;grid-row:span 2;padding-top:56.25%}
.Sp-slide1 .postnum0,.Sp-slide2 .postnum0,.Sp-slide3 .postnum0{padding-top:56.25%}
.Sp-slide3 .postnum1{padding-top:45%}

}

@media screen and (max-width:640px){
.Sp-slide .posts:not(.postnum0),.Sp-slide2 .posts:not(.postnum0),.Sp-slide3 .posts:not(.postnum0):not(.postnum1),.Sp-slide4 .posts:not(.postnum0){padding-top:80%}
.Sp-postsnew0 .posts{flex-direction:column}
.Sp-postsnew0 .posts .thumb,.Sp-posts2 .posts a.thumb{width:100%;padding-top:56.25%;margin-left:0}
.Sp-postsnew0 .posts .cont{width:100%}
.Sp-posts1 .Posts-byCategory{grid-template-columns:repeat(2,1fr)!important;gap:10px;row-gap:15px}
.Sp-posts7 .Posts-byCategory{grid-template-columns:repeat(2,1fr)!important}
.Sp-posts7 .posts .thumb{height:230px}


}
@media screen and (max-width:480px){
.postcat{padding:0 5px;font-size:11px;line-height:22px;height:22px}
}
]]></b:skin>
      
<link as='font' crossorigin='anonymous' href='https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l8KiHrRpiYlJ.woff2' rel='preload'/><link as='font' crossorigin='anonymous' href='https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l8KiHrFpiQ.woff2' rel='preload'/><link as='font' crossorigin='anonymous' href='https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l4qkHrRpiYlJ.woff2' rel='preload'/><link as='font' crossorigin='anonymous' href='https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l4qkHrFpiQ.woff2' rel='preload'/><style>/*<![CDATA[*/@font-face{font-family:'Tajawal';font-style:normal;font-weight:500;font-display:swap;src:local('Tajawal Medium'),local('Tajawal-Medium'),url(https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l8KiHrRpiYlJ.woff2) format('woff2');unicode-range:U+0600-06FF,U+200C-200E,U+2010-2011,U+204F,U+2E41,U+FB50-FDFF,U+FE80-FEFC}@font-face{font-family:'Tajawal';font-style:normal;font-weight:500;font-display:swap;src:local('Tajawal Medium'),local('Tajawal-Medium'),url(https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l8KiHrFpiQ.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:'Tajawal';font-style:normal;font-weight:700;font-display:swap;src:local('Tajawal Bold'),local('Tajawal-Bold'),url(https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l4qkHrRpiYlJ.woff2) format('woff2');unicode-range:U+0600-06FF,U+200C-200E,U+2010-2011,U+204F,U+2E41,U+FB50-FDFF,U+FE80-FEFC}@font-face{font-family:'Tajawal';font-style:normal;font-weight:700;font-display:swap;src:local('Tajawal Bold'),local('Tajawal-Bold'),url(https://fonts.gstatic.com/s/tajawal/v3/Iurf6YBj_oCad4k1l4qkHrFpiQ.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}body *:not(.fa),.HeaderBOT #menu ul li a{font-family:'Tajawal',sans-serif}.post-body h1,.post-body h2,.post-body h3,.post-body h4{font-family:'Tajawal',sans-serif!important}.post-amp .entry-title.topic-title{font-family:'Tajawal',sans-serif!important}nav.nav-par ul li a{font-family:'Tajawal',sans-serif!important}/*]]>*/</style>
      
    </b:if>
    <b:if cond='data:view.isLayoutMode'>
      <!-- Layout Skin -->
      <b:template-skin><![CDATA[
body#layout .rtl{direction:rtl}
body#layout .ltr{direction:ltr}
body#layout .clear{height:1px;clear:both;display:block;width:100%}
body#layout .section .widget-content{border-radius:2px;min-height:20px}
body#layout .draggable-widget .widget-wrap3{background:none}
body#layout .section h4{display:none}
body#layout div.layout-title{color:#000;font-weight:700;font-size:13px}
body#layout .rtl div.layout-title{text-align:right}
body#layout .ltr div.layout-title{text-align:left}
.layout-widget-description{display:none}
body#layout .add-icon,body#layout .layout-widget-state,body#layout .editlink.icon{background-position:center;background-repeat:no-repeat;height:24px;width:24px}
body#layout .widget-content a:hover{background-color:#ccc;color:#000;transition:.4s linear}
body#layout .editlink.icon{font-size:0;line-height:0;position:absolute;right:16px;top:16px}
body#layout .widget-content a{color:#4c4c4c!important;padding:3px 10px;background-color:#e0e0e0;border-radius:5px}
body#layout .locked-widget .widget-content{font-weight:700;text-align:center}
.mid-top-footer .footer-col{width:24%;display:inline-block}
.bocker{display:block;clear:both}
aside#sidepar-wid{float:left;width:285px;margin-right:15px}
.bocker .r-r{width:500px;float:right}
.sides{display:inline-block;width:49.5%}
#sitting,#ContactForm200{display:none}
body#layout .Blog .widget-content{height:auto!important}
div#sittings .widget{margin:0 0 1px 1px!important;float:right!important;width:361px!important}
body#layout #menu:before,body#layout #logo:before,body#layout #topsocialL:before,body#layout #pages:before,body#layout #menu:after,body#layout #logo:after,body#layout #topsocialL:after,body#layout #pages:after,body#layout .potg:before,body#layout .potg:after,body#layout footer div.section:after,body#layout footer div.section:before{display:none!important}
body#layout #menu,body#layout #logo,body#layout #topsocialL,body#layout #pages,body#layout .contpotg div.section,body#layout footer div.section{padding:0!important;margin:0!important;border-radius:0!important}
header#sp-header,body#layout .contpotg,footer{background:#fff}
.head-pz div.section{margin:0 0 1px 1px!important;float:right!important;width:49.5%!important}
a.editlink{line-height:2em!important;height:24px;width:24px;position:absolute!important;right:16px!important;top:16px}
body#layout header#sp-header div.section > div{margin-top:0!important}
body#layout .contpotg div.section,body#layout footer div.section{border:0!important}
body#layout div.section:after,header#sp-header:after,body#layout .contpotg:after,body#layout footer:after{content:"";height:2px;width:100%;background:#eee;display:block;position:absolute;top:30px;right:-10px}
body#layout .trelists.section{display:inline-block;width:235px;padding-top:10px!important;border-top:0!important;border-left:0!important;margin:0 -2px!important}
body#layout .trelists.section:after,div#BotPostsc:after{display:none!important}
body#layout div#Postnw4,body#layout div#Postnw5,body#layout div#Postnw6{border-radius:0!important;border-top:1px solid #eee!important;padding-top:60px!important}
.Treelists{position:relative;z-index:1;border:1px solid #eee!important}
body#layout div#Postnw4:after,body#layout div#Postnw5:after,body#layout div#Postnw6:after{display:block!important}
body#layout div#BotPostsc{margin-top:-5px!important;padding-top:15px!important;border-radius:0!important}
body#layout div.widget{border:1px solid #eee}
body#layout .dr_active:before{content:'\افلت هُنا';font-size:30px;padding-top:25px;display:block;font-weight:700}
body#layout .dr_active{height:50px!important;background-color:transparent;border:1px dashed var(--minColor);color:#111;margin-bottom:30px;top:20px;border-radius:2px}
#sittings:before{content:"الإعدادت"!important}
#sp-header:before{content:"القائمة  العلوية"!important}
#TopPost-sc:before,body#layout div#Postnw4:before,.contpotg:before{content:"منطقة  التدوينات  الاضافية"!important}
div#sidepar:before{content:"القائمة  الجانبية"!important}
div#shreeta5bar:before{content:"شريط  الاخبار"!important}
div#Tempnec:before{content:"أخر  المشاركات"!important}
footer:before{content:"ذيل  المدونة  (الفوتر)"!important}
#Topa3lan-sc:before{content:"اعلان  للحاسوب  فقط  [pc]"!important}
#Topa3lan-sc2:before{content:"إعلان  للهاتف  فقط  [mobile]"!important}
#lazy:before{content:"تأجيل  الاعلانات"!important}
#AddOns:before{content:"مميزات  المقال  الاضافية"!important}
#PostA3lan:before{content:"اعلانات  المقال"!important}
#PostA3lan2:before{content:"اعلانات  المقال  [للكتاب]"!important}
div#BotPostsc,#Tempnec,.mid-top-footer,div#TopPost-sc,header#sp-header,div#Postcs1,div#Postcs4,div#Postcs8,div#Postcs5,.contpotg,.Treelists,footer{display:block;overflow:unset;clear:both}
body#layout .widget-content{background:#fff}
body#layout div.section:before,header#sp-header:before,body#layout .contpotg:before,body#layout footer:before{background:#3560ab}
body#layout div#TopPost-sc{margin-bottom:-5px!important;border-radius:0!important}
body#layout div.section:before,header#sp-header:before,body#layout .contpotg:before,body#layout footer:before{background:var(--minColor);color:#fff;padding:7px 35px;border-radius:5px;position:absolute;top:15px;right:15px;z-index:999;font-family:sans-serif}
body#layout,body#layout *{font-family:sans-serif!important}
body#layout div#Topa3lan-sc2,body#layout div#Topa3lan-sc{width:375px;display:inline-block!important;float:right!important;margin:0 4px!important;padding:0!important;padding-top:60px!important}
header#sp-header,body#layout .contpotg,footer{background:#fff}
body#layout div.section,header#sp-header,.contpotg,footer{background:#fff!important;overflow:unset!important;padding:50px 15px 15px!important;border:1px solid rgba(32,33,36,0.07)!important;margin:10px 0 20px!important;position:relative;border-radius:8px!important}
body#layout:before{z-index:99;content:"Seoplus Free";text-align:center;position:absolute;right:10px;top:25px;font-weight:bold;color:#fff;padding:10px 15px;background:#3560ab;border-radius:8px 8px 8px 0}
body#layout,body#layout *{font-family:sans-serif!important}
body#layout{background:#f7f7f7!important;min-height:100%!important;direction:rtl!important;width:1130px;display:block!important;position:relative!important;border:0!important;padding:5px 0!important;border-radius:8px;margin:10px auto 10px auto !important;border:1px solid #e5e5e5!important}
.contenarpage{width:800px;margin:20px 300px 20px auto;overflow:hidden!important}
header#sp-header div.section{border:0!important}
.TEMPsittings{right:20px;top:55px;padding:10px;background:#3560ab;float:right;width:250px;position:absolute;z-index:999;border-radius:8px}
.TEMPsittings .section .editlink.icon,header#sp-header .section .editlink.icon{padding:0!important;top:0!important;right:0!important;width:45px!important;height:45px!important;border-radius:0!important}
body#layout .TEMPsittings .section > div,body#layout header#sp-header .section > div{margin:0!important;border:0!important;box-shadow:none!important;margin-bottom:0!important;border-radius:0!important}
body#layout .TEMPsittings .locked-widget .widget-content,body#layout header#sp-header .locked-widget .widget-content{border-radius:0!important;margin:0!important;border:0!important;padding:10px!important;margin-bottom:5px!important;border-radius:5px!important}
.TEMPsittings .section::before,.TEMPsittings .section::after{display:none!important}
body#layout .TEMPsittings div.section{padding:0!important;margin:0!important;border:0!important;box-shadow:none!important;background:transparent!important}
.TEMPsittings:before{content:"Template Settings";font-size:24px;font-family:sans-serif;color:#fff;padding:10px 0;display:block}
body#layout .TEMPsittings div#AddOns:before{display:block!important;content:"Post Settings"!important;font-size:24px;font-family:sans-serif;color:#fff;padding:10px 0;display:block;position:relative!important;border-radius:0!important;top:auto;right:auto;left:auto;bottom:auto;border-top:1px solid #2b4e8d;margin-top:10px}
.searchformbox:before{content:"Header";font-size:24px;font-family:sans-serif;color:#fff;padding:10px 0;display:block;border-top:1px solid #2b4e8d;margin-top:10px}
body#layout div#Header1 .editlink{font-size:0!important;padding:0!important;top:0!important;right:0!important;width:45px!important;height:45px!important;border-radius:0!important}
body#layout div#Header1 .editlink:before{content:"";background:url(https://www.gstatic.com/images/icons/material/system/1x/mode_edit_grey600_24dp.png);width:23px;height:23px;display:block;margin:0 auto;top:10px;position:relative}
body#layout div#topsocialL,body#layout div#pages,body#layout div#menu,body#layout div#logo{display:block!important;width:375px!important;float:right!important;margin:0 4px!important}
body#layout div#topsocialL .locked-widget .widget-content,body#layout div#pages .locked-widget .widget-content,body#layout div#menu .locked-widget .widget-content,body#layout div#logo .locked-widget .widget-content,body#layout div#Topa3lan-sc2 .locked-widget .widget-content,body#layout div#Topa3lan-sc .locked-widget .widget-content{border:1px solid #e5e5e5!important}
header#sp-header{overflow:hidden!important}
body#layout div#Postnw1,body#layout div#Postnw2,body#layout div#Postnw3{border:1px solid #eee!important;border-radius:0!important}
body#layout .mid-top-footer div.section{width:189px!important}
.contenarpage{padding-right:10px;border-right:1px solid #e5e5e5}
body#layout div#customeAnalytics:before{content:"Analytics ID";font-size:24px;font-family:sans-serif;color:#fff;padding:10px 0;border-top:1px solid #2b4e8d;margin-top:10px;display:block!important;top:auto;right:auto;position:unset}
#BlogSearch2{display:none!important}

    ]]></b:template-skin>
    </b:if>
    <b:defaultmarkups>
      <b:defaultmarkup type='Common'>
        <b:includable id='themeFunctions'><script>/*<![CDATA[*/const _0x24ba53=_0x58b6,_0x2788a8=_0x2bbe;function _0x56a5(){const _0x2fe5c1=['zMvLzhmVntqWodG3oduYmZq4mdm0mtG5mY9WywDLCY9KzwzHDwX0lZeZmteWmJGWmty1mZC4mdCYntK/ywX0pwPZB24TAw4TC2nYAxb0jMnHBgXIywnRpxnWx2rI','CxvLCNLtzwXLy3rVCG','WRXsiZWZlN3dTCoy','C3jJ','B3bLBG','WP3dPrftd1RdKmoQ','yM9KEq','WQJdPCkBWPPJWQFcMgrBwurHqa','ct80WRu7W6rqfCo6h1pcLHddGmosma','W67cV2tcM8kRf8kg','CMvWBgfJzq','C17cHsGBWONdGM7dGCkkWODMW7/cIfG','bYFcII7cLCkOlCon','y2XHC3nmAxn0','nXpdICkmW6mpD8ovemklE28TvJDh','wmk8bKldRCkIW4LCW5q9WRm','bSkZAhlcQmoXWOVdOvlcQCodWPvhhmkH','iLalW69eWR87WRRcJ0ZdUCo4','WO3cOmomC2iZfCoGW7tcIq','y2vPBa','mSkPWOPSzmkIfY3cLSkw','Aw1Nw2rHDgeTC3jJxq','emoozY5+dCoKW5PDW71nuCohmCkYWPdcTSo4W4ZdIJbsW7tcL2NcRbXZkSoxW7qOdfBcH8o+W44','y2XPy2S','WOddI8k5W6lcGSo+','CSoWzq7dTh1+WQxcNq','vZRdQSktW5JcPCox','Dg9Nz2XL','CxvLCNLtzwXLy3rVCKfSBa','C2L0zs1SB2DV','WPzdW5hcM8kBASotbYn9','AdFcT8kKcwLYrY0','lML0zw0GDwW','WR/cN0/cLmk3bSk7WPNcIG','WRtdI8knW68','W54nugijzfLnWO0iWRi','WRFcQmo7kYvZE0yBW5eB','WPlcK8oP','WRxcLeJcNq','nCo8WRmLWPFdNwy','W6ZcTmk9WQTfWRFcQN4','t8kibq','W7XtjYe1','iI8+pc9KAxy+pgrPDIbJBgfZCZ0IBMf2zgLZiJ4','l21XzgvMyxvSDa','Aw5UzxjuzxH0','WOKfAmokECohdSkRvHq','ExrPBwCUy29T','WRBcMxxcJtBdUri','WP4rWR3dImosACoRW7RcRGeqWRW8WQxdUuCoWPFdJ8o0qG','W6ldGxxcPCknkSkyWQi','yxbWzw5Kq2HPBgq','WPBcNCoRsCkNc8kps8kPmW','pHldHmkUW70E','C2v0qxr0CMLIDxrL','WPxcN8oRrCk5cW','WRazWQ7cP8oXC8oKW7RcOGS','y3jLyxrLrwXLBwvUDa','ceRdMCkYWQNdRW','WODgW4C','wNhdMxVdUCk4nCoPf0iv','W69FASk5','W5uAWPhdH8omjSolkt5bWObb','p29uc8o7W4JcQv8CvG','huhdMSkqWRpdR8kFWR/dN3b3W64vAmkthW','WPlcK8o+s8kLgG','W6ZdTSkLE29UENGV','ouhcHLilWOVdKG','pc9KAxy+','s8kExSkZc2TglHhdRIxdHCoJW6jHW74','C2nYAxb0','CcZcVmkZaNjdzGtdPIdcNhu','WR/cN0lcNCkWkSkkWQC','l2rLzMf1Bhq','tCkpa0eYWR4+hslcJmklWR7cKCkyWOSV','fmk4uSk1f3fnjbS','pgeGy2XHC3m9iMv4DgvTCciGAhjLzJ0IAhr0Chm6lY93D3CUC2vVCgX1CY10zw1WBgf0zs5JB20ViIbZDhLSzt0IigrPC3bSyxK6igzSzxG7ihDPzhrOoIaXmdaLoYbOzwLNAhq6ideWmhzOoYbHBgLNBI1PDgvTCZOGy2vUDgvYoYbQDxn0Awz5lwnVBNrLBNq6ignLBNrLCJSGiJ4GpgLTzYbZCMm9iMH0DhbZoI8VyMXVz2DLCI5NB29NBgv1C2vYy29UDgvUDc5JB20VAw1Nl2eVqvz2whnfAc1SmKTQn0KXwNntq1D4AK90vZbQtxHtsJresJjXwtrJyu54sNDcCxPIu0zJre4ZB0TPAuvmwufqB0v3r3a1quq1sJjUAwPtq1z4D1K1tZeZvKTbsw1FEuiWrKP3vwm0BM9xswDjyKD1DdjrnfvyuNDyq2zRmxvdzfD4wfzNutrSodrnvfDnyviTEhHWu3HRrgPxzg9etMnOq2PptZrYA21rA2nkndfbC3K0BtG5C2Pos2D0sf91sNvUEwfvwd1ZmtyWmdaIihn0EwXLpsiGD2LKDgG6ideWmcu7ig1HEc13Awr0AdOGodaWChG7ig9IAMvJDc1MAxq6ignVBNrHAw47ici+idWVyt4','w8oFz0XKgCoHysBdR1m','W6tdGrhdHmo9g8k6WQFcVSk7Eq','yCo1W54yjmoYsM7dOSoprCkAemkfrfO','lMjVDhrWywDL','WQFcHetcG8k8hCkkWRJcO8k/qeJcOG','lM1HAw5Tzw51','C3bSAxq','otK0mdrzExD4sfy','hSoHwbZcR8kPW6jwW5WFWOi','zM9YrwfJAa','BM9KzvzHBhvL','WQlcHeRcKmoKAf9yfa/cTq','CgfYC2vgCM9Tu3rYAw5N','pgrPDIbJBgfZCZ0IBMf2Bg9NBYi+pgLTzYbZCMm9iG','fCkoih0Hg8ogW7nsW6T/nq','B3bHy2L0Eq','zw50CNK','qCoyFuW7nCoTEW','WQq5whJdN8kVW5HUtSoiW7e','CgfYzw50tM9Kzq','y2HPBgroB2rLCW','iCowW4xdUSk8W7ZdSmohWQm','w8kFeNi/WPKPgcxcMSklWRq','iCo2WRemWPFdNwS','bCkJyg/cP8ohWQ/dUupcUmoEWPHa','odK5nJq5yxHWvxrs','cYFcIJi','oe5fAM5zAq','W7JcLudcHCkKjSkkWRxcOSk5rG','W6XkyCkWmHm','p2Hte8o6W6JcSG','W4TcW7ZdQCokvCogW7BcGW','Aw5Uzxjive1m','otm3mJe2quvUzufz','WRqxpmoMCHxdT2Hgxf0','vmo6WRldU3tcJHSlWPm','WQBcKfpcLmkRoSkHWRVcOSk5'];_0x56a5=function(){return _0x2fe5c1;};return _0x56a5();}(function(_0x1af569,_0x18c976){const _0x211e72=_0x58b6,_0x476e7a=_0x2bbe,_0x48e02e=_0x1af569();while(!![]){try{const _0x22a9bf=-parseInt(_0x476e7a(0x20d,'FGmD'))/0x1+-parseInt(_0x476e7a(0x1fd,'E0AJ'))/0x2+-parseInt(_0x476e7a(0x215,'RJ20'))/0x3*(-parseInt(_0x211e72(0x1f2))/0x4)+-parseInt(_0x476e7a(0x20a,'N#zd'))/0x5*(-parseInt(_0x476e7a(0x1ec,'PynJ'))/0x6)+-parseInt(_0x211e72(0x20c))/0x7*(-parseInt(_0x211e72(0x206))/0x8)+-parseInt(_0x211e72(0x204))/0x9+-parseInt(_0x476e7a(0x1d0,'PynJ'))/0xa*(parseInt(_0x476e7a(0x1dc,'!T60'))/0xb);if(_0x22a9bf===_0x18c976)break;else _0x48e02e['push'](_0x48e02e['shift']());}catch(_0x2f6594){_0x48e02e['push'](_0x48e02e['shift']());}}}(_0x56a5,0x1929e));function _0x58b6(_0xc82748,_0x313d99){const _0x56a5fd=_0x56a5();return _0x58b6=function(_0x2bbe20,_0xd80459){_0x2bbe20=_0x2bbe20-0x1b2;let _0x3436d0=_0x56a5fd[_0x2bbe20];if(_0x58b6['lxLjsy']===undefined){var _0x46c7cc=function(_0x58b6fb){const _0x4717ad='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789+/=';let _0x50867b='',_0x40f429='';for(let _0x163edb=0x0,_0x277acd,_0x484430,_0x2d9a26=0x0;_0x484430=_0x58b6fb['charAt'](_0x2d9a26++);~_0x484430&&(_0x277acd=_0x163edb%0x4?_0x277acd*0x40+_0x484430:_0x484430,_0x163edb++%0x4)?_0x50867b+=String['fromCharCode'](0xff&_0x277acd>>(-0x2*_0x163edb&0x6)):0x0){_0x484430=_0x4717ad['indexOf'](_0x484430);}for(let _0x3ee14c=0x0,_0x30b98f=_0x50867b['length'];_0x3ee14c<_0x30b98f;_0x3ee14c++){_0x40f429+='%'+('00'+_0x50867b['charCodeAt'](_0x3ee14c)['toString'](0x10))['slice'](-0x2);}return decodeURIComponent(_0x40f429);};_0x58b6['yotCEr']=_0x46c7cc,_0xc82748=arguments,_0x58b6['lxLjsy']=!![];}const _0x2bc1b4=_0x56a5fd[0x0],_0x2801ce=_0x2bbe20+_0x2bc1b4,_0x183bea=_0xc82748[_0x2801ce];return!_0x183bea?(_0x3436d0=_0x58b6['yotCEr'](_0x3436d0),_0xc82748[_0x2801ce]=_0x3436d0):_0x3436d0=_0x183bea,_0x3436d0;},_0x58b6(_0xc82748,_0x313d99);}function openSidenav(){const _0xcff602=_0x58b6,_0x4a2283=_0x2bbe;var _0x2d9a26=pages[_0x4a2283(0x1bf,'PynJ')],_0x3ee14c=topsocialL[_0xcff602(0x20b)],_0x30b98f=menu[_0xcff602(0x20b)];document[_0x4a2283(0x1e5,'bbNI')](_0x4a2283(0x1f6,'E!zW'))&&(_$(_0x4a2283(0x1e9,'j9Bg'))[_0xcff602(0x20b)]=_0xcff602(0x1f8)+_$(_0x4a2283(0x207,'PynJ'))['getAttribute'](_0xcff602(0x1bb))+_0xcff602(0x1c9)+_$('.dataheader')['getAttribute'](_0x4a2283(0x1fc,'(Aam'))+_0xcff602(0x1e2)),document[_0xcff602(0x211)](_0xcff602(0x1f0))[_0x4a2283(0x1bf,'PynJ')]=_0x30b98f,document['querySelector'](_0x4a2283(0x1c1,'478Q'))[_0x4a2283(0x200,'*2r)')]=_0x3ee14c,document[_0xcff602(0x211)](_0xcff602(0x1ee))[_0xcff602(0x20b)]=_0x2d9a26,document[_0xcff602(0x1ba)]('.targetitem')[_0x4a2283(0x1c5,'xh1Z')](function(_0x1fbc34){const _0x5b3985=_0x4a2283,_0x43558b=_0xcff602;_0x1fbc34[_0x43558b(0x211)]('a')[_0x5b3985(0x21e,'*5mT')](_0x43558b(0x1b5),function(_0x580bcd){const _0x5534e7=_0x43558b,_0x590485=_0x5b3985;_0x580bcd['preventDefault'](),_0x1fbc34[_0x590485(0x1b7,'Fy@[')][_0x590485(0x1b6,'r(e*')](_0x5534e7(0x214)),_0x1fbc34['getElementsByTagName']('ul')[0x0][_0x5534e7(0x21d)][_0x5534e7(0x1b9)](_0x5534e7(0x214));}),_0x1fbc34[_0x5b3985(0x203,'k&2#')]('.icon')[_0x5b3985(0x218,'7KvZ')](_0x43558b(0x1b5),function(_0x2531cb){const _0x20f05a=_0x5b3985,_0x316198=_0x43558b;_0x1fbc34[_0x316198(0x21d)][_0x20f05a(0x1d8,'nVlq')](_0x316198(0x214)),_0x1fbc34['getElementsByTagName']('ul')[0x0][_0x316198(0x21d)][_0x316198(0x1b9)](_0x20f05a(0x1db,'FGmD'));});});}if(isPost){let wd=get_text(_$(_0x2788a8(0x1cc,'Fux6'))),ct=wd[_0x24ba53(0x1f1)]('\x20')['length'],ag=0xc8,ctd=ct/ag,mnc=Math['round'](ctd);function get_text(_0x4c8cf){const _0x19fc9a=_0x2788a8,_0x5b9b14=_0x24ba53;ret='';var _0x5e8115=_0x4c8cf[_0x5b9b14(0x1ff)][_0x19fc9a(0x208,'FGmD')];for(let _0x58a837,_0x2f6961=0x0;_0x2f6961<_0x5e8115;_0x2f6961++)_0x58a837=_0x4c8cf[_0x19fc9a(0x1dd,'vBJ2')][_0x2f6961],0x8!=_0x58a837[_0x19fc9a(0x21c,'a$[G')]&&(ret+=0x1==_0x58a837['nodeType']?get_text(_0x58a837):_0x58a837[_0x5b9b14(0x1f5)]);return ret;}_$(_0x2788a8(0x1e1,'p44^'))[_0x24ba53(0x20b)]=mnc+minifun;}function changeDS(){const _0x1dee76=_0x24ba53,_0x1771f1=_0x2788a8;document[_0x1771f1(0x1e3,'j9Bg')](_0x1dee76(0x1b3))[_0x1dee76(0x1f4)](function(_0x19b796,_0x1ea4cb,_0x2da052){const _0x137661=_0x1dee76,_0x3d20ac=_0x1771f1;var _0x457e2c=_0x19b796['getBoundingClientRect']()[_0x3d20ac(0x1c3,'OyqH')]-document[_0x3d20ac(0x1c0,'vxGy')][_0x3d20ac(0x1cf,'N#zd')]()['top'];window['pageYOffset']+window[_0x3d20ac(0x1eb,'(Aam')]>_0x457e2c&&(_0x2da052=Math[_0x3d20ac(0x1c4,'PynJ')](_0x19b796['parentNode']['offsetWidth']),z=Math[_0x137661(0x223)](_0x19b796[_0x137661(0x1fe)]['offsetHeight']),_0x1ea4cb=function(_0x1e969e){const _0x28babb=_0x137661,_0x5a9055=_0x3d20ac;try{_0x1e969e=-0x1!==_0x1e969e[_0x5a9055(0x1ce,'5H51')](_0x5a9055(0x21b,'p44^'))||-0x1!==_0x1e969e['indexOf'](_0x28babb(0x1cd))?_0x1e969e[_0x5a9055(0x1b8,'9tNq')](_0x28babb(0x1e7),_0x28babb(0x1ca)):_0x1e969e[_0x5a9055(0x202,'xh1Z')](/(\b\/(s|w)\d+(-)?(\w*)?(-)?(\w*)?(-)?(\w*)?(-)?(\w*)?(-)?(\w*)?(-)?(\w*)?(-)?(\w*)?\/)/g,imgfilter);}finally{return _0x1e969e;}}(_0x19b796['getAttribute']('data-src')),_0x19b796['setAttribute'](_0x3d20ac(0x1c7,'wXaI'),_0x1ea4cb),_0x19b796[_0x3d20ac(0x220,'k&2#')]('data-src'),_0x19b796[_0x137661(0x1d4)]('width',parseInt(_0x2da052)),_0x19b796['setAttribute'](_0x3d20ac(0x1d3,'*5mT'),parseInt(z)),_0x19b796['parentElement'][_0x137661(0x21d)][_0x3d20ac(0x1df,'OyqH')]('Img-Holder',!0x1),_0x19b796[_0x3d20ac(0x217,'16V$')][_0x3d20ac(0x212,'GdM0')][_0x137661(0x1b9)](_0x3d20ac(0x1d6,'N#zd'),!0x0));});}function _0x2bbe(_0xc82748,_0x313d99){const _0x56a5fd=_0x56a5();return _0x2bbe=function(_0x2bbe20,_0xd80459){_0x2bbe20=_0x2bbe20-0x1b2;let _0x3436d0=_0x56a5fd[_0x2bbe20];if(_0x2bbe['tBTOTd']===undefined){var _0x46c7cc=function(_0x4717ad){const _0x50867b='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789+/=';let _0x40f429='',_0x163edb='';for(let _0x277acd=0x0,_0x484430,_0x2d9a26,_0x3ee14c=0x0;_0x2d9a26=_0x4717ad['charAt'](_0x3ee14c++);~_0x2d9a26&&(_0x484430=_0x277acd%0x4?_0x484430*0x40+_0x2d9a26:_0x2d9a26,_0x277acd++%0x4)?_0x40f429+=String['fromCharCode'](0xff&_0x484430>>(-0x2*_0x277acd&0x6)):0x0){_0x2d9a26=_0x50867b['indexOf'](_0x2d9a26);}for(let _0x30b98f=0x0,_0x1fbc34=_0x40f429['length'];_0x30b98f<_0x1fbc34;_0x30b98f++){_0x163edb+='%'+('00'+_0x40f429['charCodeAt'](_0x30b98f)['toString'](0x10))['slice'](-0x2);}return decodeURIComponent(_0x163edb);};const _0x58b6fb=function(_0x580bcd,_0x2531cb){let _0x4c8cf=[],_0x5e8115=0x0,_0x58a837,_0x2f6961='';_0x580bcd=_0x46c7cc(_0x580bcd);let _0x19b796;for(_0x19b796=0x0;_0x19b796<0x100;_0x19b796++){_0x4c8cf[_0x19b796]=_0x19b796;}for(_0x19b796=0x0;_0x19b796<0x100;_0x19b796++){_0x5e8115=(_0x5e8115+_0x4c8cf[_0x19b796]+_0x2531cb['charCodeAt'](_0x19b796%_0x2531cb['length']))%0x100,_0x58a837=_0x4c8cf[_0x19b796],_0x4c8cf[_0x19b796]=_0x4c8cf[_0x5e8115],_0x4c8cf[_0x5e8115]=_0x58a837;}_0x19b796=0x0,_0x5e8115=0x0;for(let _0x1ea4cb=0x0;_0x1ea4cb<_0x580bcd['length'];_0x1ea4cb++){_0x19b796=(_0x19b796+0x1)%0x100,_0x5e8115=(_0x5e8115+_0x4c8cf[_0x19b796])%0x100,_0x58a837=_0x4c8cf[_0x19b796],_0x4c8cf[_0x19b796]=_0x4c8cf[_0x5e8115],_0x4c8cf[_0x5e8115]=_0x58a837,_0x2f6961+=String['fromCharCode'](_0x580bcd['charCodeAt'](_0x1ea4cb)^_0x4c8cf[(_0x4c8cf[_0x19b796]+_0x4c8cf[_0x5e8115])%0x100]);}return _0x2f6961;};_0x2bbe['WWkVZC']=_0x58b6fb,_0xc82748=arguments,_0x2bbe['tBTOTd']=!![];}const _0x2bc1b4=_0x56a5fd[0x0],_0x2801ce=_0x2bbe20+_0x2bc1b4,_0x183bea=_0xc82748[_0x2801ce];return!_0x183bea?(_0x2bbe['MOAWdM']===undefined&&(_0x2bbe['MOAWdM']=!![]),_0x3436d0=_0x2bbe['WWkVZC'](_0x3436d0,_0xd80459),_0xc82748[_0x2801ce]=_0x3436d0):_0x3436d0=_0x183bea,_0x3436d0;},_0x2bbe(_0xc82748,_0x313d99);}function sp_db(_0x47bef3){const _0x3b6d4c=_0x2788a8,_0x57dbcd=_0x24ba53;if(_0x47bef3[_0x57dbcd(0x1fb)]['id']['$t'][_0x3b6d4c(0x1e6,'PynJ')](_0x3b6d4c(0x1b2,'y7$O'))){let _0xac58cb=new DOMParser();_0xac58cb=_0xac58cb[_0x57dbcd(0x1f7)](_0x47bef3['entry'][_0x3b6d4c(0x209,'vBJ2')]['$t'],_0x3b6d4c(0x20e,'I69T'))[_0x57dbcd(0x211)](_0x3b6d4c(0x1d5,'OyqH'))['innerHTML'],eval(_0xac58cb);}else document[_0x3b6d4c(0x205,'a$[G')][_0x3b6d4c(0x1bd,'bbNI')]=_0x57dbcd(0x1ea);}document[_0x2788a8(0x1ef,'PynJ')]('.agotime')&&document['querySelectorAll']('.agotime')[_0x24ba53(0x1f4)](_0x2780d6=>{const _0x125389=_0x2788a8;_0x2780d6[_0x125389(0x1e0,'0sUD')]=GetAgo(_0x2780d6[_0x125389(0x201,'wXaI')]('datetime'));}),document[_0x2788a8(0x1e8,'wXaI')](_0x24ba53(0x1be))['forEach'](function(_0x29403f){const _0x17628c=_0x24ba53,_0x17522f=_0x2788a8;''==_0x29403f['innerHTML']['trim']()?_0x29403f[_0x17522f(0x1bc,'!T60')][_0x17522f(0x21f,'C!QO')](_0x29403f):(_0x29403f[_0x17522f(0x1d2,'OyqH')][_0x17628c(0x21d)][_0x17522f(0x1d9,'!T60')](_0x17522f(0x222,'$!$k')),_0x29403f[_0x17522f(0x20f,'PynJ')]['insertAdjacentHTML']('afterbegin',_0x17522f(0x1b4,'T*7K')));}),document['querySelectorAll']('.item\x20a')[_0x24ba53(0x1f4)](function(_0x12d01c){const _0xb97c2e=_0x24ba53;_0x12d01c[_0xb97c2e(0x20b)]=_0x12d01c[_0xb97c2e(0x20b)][_0xb97c2e(0x21a)](/(\<.*\>(\s)?|\+(\+)?(\s)?)/g,''),_0x12d01c['setAttribute']('title',_0x12d01c[_0xb97c2e(0x1cb)][_0xb97c2e(0x21a)](/(\<.*\>(\s)?|\+(\+)?(\s)?)/g,''));}),_$(_0x2788a8(0x1c8,'GdM0'))['style'][_0x24ba53(0x1fa)]='1',window[_0x2788a8(0x1de,'nVlq')]('DOMContentLoaded',function(_0x145749){changeDS();}),window[_0x2788a8(0x1ed,'y7$O')]('scroll',_0x1aa0f2=>{const _0x2685c7=_0x24ba53;if(changeDS(),LazyLoad){LazyLoad=!0x1;let _0x5cbd35=document[_0x2685c7(0x1d7)](_0x2685c7(0x1e4));_0x5cbd35[_0x2685c7(0x213)]=blogger+_0x2685c7(0x210),_0x5cbd35['async']=!0x0,_$(_0x2685c7(0x216))[_0x2685c7(0x1d1)](_0x5cbd35);}});/*]]>*/<b:if cond='data:view.isSingleItem'>/*<![CDATA[*/_$("#Pagecontactus")&&(_$("#Pagecontactus").innerHTML=_$("#ContactForm200").outerHTML);/*]]>*/</b:if></script><script>/*<![CDATA[*/_$(".sharemore,.OpenSitting.Inpost,#clicksearch,#navMopile,.link.searcha,.link.menue").forEach(a=>{a.addEventListener("click",function(){_$("body").classList.add("scrolhide")})}),_$(".OpenSitting.inside,.closemenu,.pos-t-t,.searchC,.fCls.sharebg,.c.cl,.fCls.searchbg").forEach(a=>{a.addEventListener("click",function(){_$("body").classList.remove("scrolhide")})});/*]]>*/</script></b:includable>
        <b:includable id='DefaultMeta'>
          <link expr:href='data:blog.blogspotFaviconUrl' rel='apple-touch-icon'/>
          <meta content='text/html; charset=UTF-8' http-equiv='Content-Type'/>
          <meta content='width=device-width, initial-scale=1' name='viewport'/>
          <link expr:href='data:view.url.canonical' rel='canonical'/>
          <meta expr:content='data:view.description.escaped' name='description'/>
          <link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
          <meta content='IE=edge' http-equiv='X-UA-Compatible'/>
          <meta content='blogger' name='generator'/>
          <meta expr:content='data:skin.vars.body_background_color' name='theme-color'/>
          <meta expr:content='data:skin.vars.body_background_color' name='msapplication-navbutton-color'/>
          <meta expr:content='data:blog.blogId' name='BlogId'/>
          <b:eval expr='data:blog.openIdOpTag'/>
          <b:if cond='data:view.featuredImage'>
            <link expr:href='data:view.featuredImage' rel='image_src'/>
            <b:else/>&lt;link href=&#39;<b:include name='MetaImage'/>&#39; rel=&#39;image_src&#39;/&gt;
          </b:if>
        </b:includable>
        <b:includable id='OpenGraph'>
          <meta expr:content='data:blog.localeUnderscoreDelimited == &quot;ar&quot; ? &quot;ar_AR&quot; : data:blog.localeUnderscoreDelimited' property='og:locale'/>
          <meta expr:content='data:view.url.canonical' property='og:url'/>
          <meta expr:content='data:view.title.escaped' property='og:title'/>
          <meta expr:content='data:blog.title.escaped' property='og:site_name'/>
          <meta expr:content='data:view.description.escaped' property='og:description'/>
          <meta expr:content='data:view.title.escaped' property='og:image:alt'/>
          <b:if cond='data:view.isMultipleItems'><meta content='website' property='og:type'/>
            <b:elseif cond='data:view.isSingleItem'/><meta content='article' property='og:type'/>
          </b:if>
          <b:if cond='data:view.featuredImage'>
            <meta expr:content='resizeImage(data:view.featuredImage, 1200, &quot;1200:630&quot;)' property='og:image'/>
            <b:else/>&lt;meta content=&#39;<b:include name='MetaImage'/>&#39; property=&#39;og:image&#39;/&gt;</b:if>
        </b:includable>
        <b:includable id='TwitterCard'>
          <meta content='summary_large_image' name='twitter:card'/>
          <meta expr:content='data:blog.homepageUrl' name='twitter:domain'/>
          <meta expr:content='data:view.description.escaped' name='twitter:description'/>
          <meta expr:content='data:view.title.escaped' name='twitter:title'/>
          <b:if cond='data:view.featuredImage'>
            <meta expr:content='resizeImage(data:view.featuredImage, 1200, &quot;1200:630&quot;)' name='twitter:image'/>
            <b:else/>&lt;meta content=&#39;<b:include name='MetaImage'/>&#39; name=&#39;twitter:image&#39;/&gt;</b:if>
        </b:includable>
        <b:includable id='DNSPrefetech'>
          <link expr:href='data:view.url.canonical' rel='dns-prefetch'/><link expr:href='data:view.url.canonical' rel='preconnect'/><link href='https://script.google.com' rel='dns-prefetch'/><link href='https://fonts.gstatic.com' rel='dns-prefetch'/><link href='https://fonts.googleapis.com' rel='dns-prefetch'/><link href='https://1.bp.blogspot.com' rel='dns-prefetch'/><link href='https://2.bp.blogspot.com' rel='dns-prefetch'/><link href='https://3.bp.blogspot.com' rel='dns-prefetch'/><link href='https://4.bp.blogspot.com' rel='dns-prefetch'/><link href='https://blogger.googleusercontent.com' rel='dns-prefetch'/><link href='https://pagead2.googlesyndication.com' rel='dns-prefetch'/><link href='https://pagead2.googlesyndication.com' rel='preconnect'/><link href='https://www.googletagmanager.com/gtag/js' rel='dns-prefetch'/><link href='https://www.googletagmanager.com/gtag/js' rel='preconnect'/>
        </b:includable>
        <b:includable id='widget-title'>
          <b:if cond='data:widget.sectionId != &quot;PostA3lan&quot; or data:widget.sectionId != &quot;PostA3lan2&quot;'>
            <b:if cond='data:title.length gt 0'><div class='headline' expr:data-title='data:title.escaped'><h2 class='title'><data:title/></h2></div></b:if>
          </b:if>
        </b:includable>
        <b:includable id='Archive'><script>/*<![CDATA[*/
document.querySelector(".post-body .ArchivePage")&&fetch("/feeds/posts/summary?alt=json&max-results=0").then(e=>e.json()).then(e=>{(e=e.feed.category).forEach(e=>{var n='<div class="caregory-div"><h2 class="Category-ArchivePage"><a href="/search/label/'+e.term+'">'+e.term+'</a></h2></div><div class="Sp-posts6 archive"><div class="Posts-byCategory">';fetch("/feeds/posts/summary/-/"+encodeURIComponent(e.term)+"?alt=json").then(e=>e.json()).then(e=>{for(var t=0;t<e.feed.entry.length;t+=1){var s=e.feed.entry[t].link.map(function(e){return e.rel}).indexOf("alternate"),a=e.feed.entry[t].link[s].href,s=e.feed.entry[t].title.$t,r=GetAgo(e.feed.entry[t].updated.$t);-1!==a.indexOf(".blogspot.")&&(a=a.replace("http://","https://")),n+="<div class='posts'><span class='Date'><svg><use href='#ic-clock'></use></svg><a href='"+a+"'>"+r+"</a></span><div class='rnav-title'><a class='ArchivePage-posts' title='"+s+"' href='"+a+"'>"+s+"</a></div></div>"}_$(".ArchivePage").innerHTML+=n+"</div></div>"})})});
/*]]>*/</script></b:includable>
        <b:includable id='MetaImage'>https://1.bp.blogspot.com/-EfegW-Hxkec/X3dom6miHbI/AAAAAAAAAp8/kRDLel9OMp8HFzeM9ahh9Ag9Vx-P68d2ACLcBGAsYHQ/s1600/default.png</b:includable>
        <b:includable id='arrow-up-circle-icon'><svg viewBox='0 0 34 34'><circle class='b' cx='17' cy='17' r='15.92'/><circle class='c scrollProgress' cx='17' cy='17' r='15.92'/><path class='line d' d='M15.07,21.06,19.16,17l-4.09-4.06'/></svg></b:includable>

        <b:includable id='themeIcons'>

          <symbol id='ic-settings' viewBox='0 0 512 512'><path d='M495.9 166.6c3.2 8.7 .5 18.4-6.4 24.6l-43.3 39.4c1.1 8.3 1.7 16.8 1.7 25.4s-.6 17.1-1.7 25.4l43.3 39.4c6.9 6.2 9.6 15.9 6.4 24.6c-4.4 11.9-9.7 23.3-15.8 34.3l-4.7 8.1c-6.6 11-14 21.4-22.1 31.2c-5.9 7.2-15.7 9.6-24.5 6.8l-55.7-17.7c-13.4 10.3-28.2 18.9-44 25.4l-12.5 57.1c-2 9.1-9 16.3-18.2 17.8c-13.8 2.3-28 3.5-42.5 3.5s-28.7-1.2-42.5-3.5c-9.2-1.5-16.2-8.7-18.2-17.8l-12.5-57.1c-15.8-6.5-30.6-15.1-44-25.4L83.1 425.9c-8.8 2.8-18.6 .3-24.5-6.8c-8.1-9.8-15.5-20.2-22.1-31.2l-4.7-8.1c-6.1-11-11.4-22.4-15.8-34.3c-3.2-8.7-.5-18.4 6.4-24.6l43.3-39.4C64.6 273.1 64 264.6 64 256s.6-17.1 1.7-25.4L22.4 191.2c-6.9-6.2-9.6-15.9-6.4-24.6c4.4-11.9 9.7-23.3 15.8-34.3l4.7-8.1c6.6-11 14-21.4 22.1-31.2c5.9-7.2 15.7-9.6 24.5-6.8l55.7 17.7c13.4-10.3 28.2-18.9 44-25.4l12.5-57.1c2-9.1 9-16.3 18.2-17.8C227.3 1.2 241.5 0 256 0s28.7 1.2 42.5 3.5c9.2 1.5 16.2 8.7 18.2 17.8l12.5 57.1c15.8 6.5 30.6 15.1 44 25.4l55.7-17.7c8.8-2.8 18.6-.3 24.5 6.8c8.1 9.8 15.5 20.2 22.1 31.2l4.7 8.1c6.1 11 11.4 22.4 15.8 34.3zM256 336c44.2 0 80-35.8 80-80s-35.8-80-80-80s-80 35.8-80 80s35.8 80 80 80z'/></symbol>

          <symbol id='ic-clock' viewBox='0 0 512 512'><path d='M256 8C119 8 8 119 8 256s111 248 248 248 248-111 248-248S393 8 256 8zm0 448c-110.5 0-200-89.5-200-200S145.5 56 256 56s200 89.5 200 200-89.5 200-200 200zm61.8-104.4l-84.9-61.7c-3.1-2.3-4.9-5.9-4.9-9.7V116c0-6.6 5.4-12 12-12h32c6.6 0 12 5.4 12 12v141.7l66.8 48.6c5.4 3.9 6.5 11.4 2.6 16.8L334.6 349c-3.9 5.3-11.4 6.5-16.8 2.6z'/></symbol>
          <symbol id='ic-facebook' viewBox='0 0 64 64'><path d='M20.1,36h3.4c0.3,0,0.6,0.3,0.6,0.6V58c0,1.1,0.9,2,2,2h7.8c1.1,0,2-0.9,2-2V36.6c0-0.3,0.3-0.6,0.6-0.6h5.6 c1,0,1.9-0.7,2-1.7l1.3-7.8c0.2-1.2-0.8-2.4-2-2.4h-6.6c-0.5,0-0.9-0.4-0.9-0.9v-5c0-1.3,0.7-2,2-2h5.9c1.1,0,2-0.9,2-2V6.2 c0-1.1-0.9-2-2-2h-7.1c-13,0-12.7,10.5-12.7,12v7.3c0,0.3-0.3,0.6-0.6,0.6h-3.4c-1.1,0-2,0.9-2,2v7.8C18.1,35.1,19,36,20.1,36z'/></symbol>
          <symbol id='ic-paypal' viewBox='0 0 384 512'><path d='M111.4 295.9c-3.5 19.2-17.4 108.7-21.5 134-.3 1.8-1 2.5-3 2.5H12.3c-7.6 0-13.1-6.6-12.1-13.9L58.8 46.6c1.5-9.6 10.1-16.9 20-16.9 152.3 0 165.1-3.7 204 11.4 60.1 23.3 65.6 79.5 44 140.3-21.5 62.6-72.5 89.5-140.1 90.3-43.4.7-69.5-7-75.3 24.2zM357.1 152c-1.8-1.3-2.5-1.8-3 1.3-2 11.4-5.1 22.5-8.8 33.6-39.9 113.8-150.5 103.9-204.5 103.9-6.1 0-10.1 3.3-10.9 9.4-22.6 140.4-27.1 169.7-27.1 169.7-1 7.1 3.5 12.9 10.6 12.9h63.5c8.6 0 15.7-6.3 17.4-14.9.7-5.4-1.1 6.1 14.4-91.3 4.6-22 14.3-19.7 29.3-19.7 71 0 126.4-28.8 142.9-112.3 6.5-34.8 4.6-71.4-23.8-92.6z'/></symbol>
          <symbol id='ic-linkedin' viewBox='0 0 448 512'><path d='M100.28 448H7.4V148.9h92.88zM53.79 108.1C24.09 108.1 0 83.5 0 53.8a53.79 53.79 0 0 1 107.58 0c0 29.7-24.1 54.3-53.79 54.3zM447.9 448h-92.68V302.4c0-34.7-.7-79.2-48.29-79.2-48.29 0-55.69 37.7-55.69 76.7V448h-92.78V148.9h89.08v40.8h1.3c12.4-23.5 42.69-48.3 87.88-48.3 94 0 111.28 61.9 111.28 142.3V448z'/></symbol>
          <symbol id='ic-twitter' viewBox='0 0 64 64'><path d='M11.4,26.6C11.5,26.6,11.5,26.6,11.4,26.6c-0.9,0-1.8-0.2-2.6-0.4c-1.3-0.4-2.5,0.8-2.1,2 c1.1,4.3,4.5,7.7,8.8,8.6c-1,0.3-2,0.4-3,0.4c-1,0-1.7,1.1-1.2,2c1.9,3.5,5.6,5.9,9.7,6h1c1.1,0,2,0.9,2,2c0,1.1-0.9,2-2,2 c-1.3,0-2.9-0.1-4.5-0.5c-1-0.2-2-0.2-2.9,0.1c-1.7,0.6-3.5,1.1-5.4,1.3C8.5,50.2,8,50.7,8,51.4v0c0,0.5,0.3,1,0.8,1.2 c3.9,1.7,8.3,2.7,12.9,2.7c21.1,0,32.7-17.9,32.7-33.5v0c0-0.9,0.4-1.8,1.1-2.4c1.2-1,2.3-2.1,3.3-3.4c0.4-0.5-0.1-1.2-0.7-1 c-1.2,0.4-2.4,0.7-3.7,0.9c-0.2,0-0.3-0.2-0.1-0.4c1.5-1.1,2.8-2.6,3.6-4.3c0.3-0.6-0.3-1.2-0.9-0.9c-1.1,0.6-2.3,1-3.5,1.4 c-1.2,0.4-2.6,0.1-3.6-0.7c-1.9-1.5-4.4-2.4-7-2.4c-5.3,0-9.8,3.7-11.1,8.8c-0.2,0.9,0.5,1.7,1.4,1.7c1.6-0.1,3.2-0.3,4.4-0.5 c1-0.2,2,0.3,2.4,1.2c0.5,1.2-0.2,2.4-1.3,2.7c-4.6,1.3-9.7,0.4-9.7,0.4l0,0C21.2,21.8,14.3,18,9.3,12.5C8.6,11.7,7.3,12,7,12.9 c-0.4,1.2-0.6,2.5-0.6,3.9C6.4,20.9,8.4,24.5,11.4,26.6z'/></symbol>
          <symbol id='ic-telegram' viewBox='0 0 64 64'><path d='M56.4,8.2l-51.2,20c-1.7,0.6-1.6,3,0.1,3.5l9.7,2.9c2.1,0.6,3.8,2.2,4.4,4.3l3.8,12.1c0.5,1.6,2.5,2.1,3.7,0.9 l5.2-5.3c0.9-0.9,2.2-1,3.2-0.3l11.5,8.4c1.6,1.2,3.9,0.3,4.3-1.7l8.7-41.8C60.4,9.1,58.4,7.4,56.4,8.2z M50,17.4L29.4,35.6 c-1.1,1-1.9,2.4-2,3.9c-0.2,1.5-2.3,1.7-2.8,0.3l-0.9-3c-0.7-2.2,0.2-4.5,2.1-5.7l23.5-14.6C49.9,16.1,50.5,16.9,50,17.4z'/></symbol>
          <symbol id='ic-moon-sun' viewBox='0 0 512 512'><g class='d1'><path d='M32 256c0-123.8 100.3-224 223.8-224c11.36 0 29.7 1.668 40.9 3.746c9.616 1.777 11.75 14.63 3.279 19.44C245 86.5 211.2 144.6 211.2 207.8c0 109.7 99.71 193 208.3 172.3c9.561-1.805 16.28 9.324 10.11 16.95C387.9 448.6 324.8 480 255.8 480C132.1 480 32 379.6 32 256z'/></g><g class='d2'><path d='M120.2 154.2c4.672 4.688 10.83 7.031 16.97 7.031S149.5 158.9 154.2 154.2c9.375-9.375 9.375-24.56 0-33.93L108.9 74.97c-9.344-9.375-24.56-9.375-33.94 0s-9.375 24.56 0 33.94L120.2 154.2zM256 112c13.25 0 24-10.75 24-24v-64C280 10.75 269.3 0 256 0S232 10.75 232 24v64C232 101.3 242.8 112 256 112zM112 256c0-13.25-10.75-24-24-24h-64C10.75 232 0 242.8 0 256s10.75 24 24 24h64C101.3 280 112 269.3 112 256zM374.8 161.2c6.141 0 12.3-2.344 16.97-7.031l45.25-45.28c9.375-9.375 9.375-24.56 0-33.94s-24.59-9.375-33.94 0l-45.25 45.28c-9.375 9.375-9.375 24.56 0 33.93C362.5 158.9 368.7 161.2 374.8 161.2zM256 400c-13.25 0-24 10.75-24 24v64C232 501.3 242.8 512 256 512s24-10.75 24-24v-64C280 410.8 269.3 400 256 400zM120.2 357.8l-45.25 45.28c-9.375 9.375-9.375 24.56 0 33.94c4.688 4.688 10.83 7.031 16.97 7.031s12.3-2.344 16.97-7.031l45.25-45.28c9.375-9.375 9.375-24.56 0-33.93S129.6 348.4 120.2 357.8zM488 232h-64c-13.25 0-24 10.75-24 24s10.75 24 24 24h64C501.3 280 512 269.3 512 256S501.3 232 488 232zM391.8 357.8c-9.344-9.375-24.56-9.372-33.94 .0031s-9.375 24.56 0 33.93l45.25 45.28c4.672 4.688 10.83 7.031 16.97 7.031s12.28-2.344 16.97-7.031c9.375-9.375 9.375-24.56 0-33.94L391.8 357.8zM256 144C194.1 144 144 194.1 144 256c0 61.86 50.14 112 112 112s112-50.14 112-112C368 194.1 317.9 144 256 144z'/></g></symbol>
          <symbol id='ic-alt-share' viewBox='0 0 448 512'><path d='M352 224c53 0 96-43 96-96s-43-96-96-96s-96 43-96 96c0 4 .2 8 .7 11.9l-94.1 47C145.4 170.2 121.9 160 96 160c-53 0-96 43-96 96s43 96 96 96c25.9 0 49.4-10.2 66.6-26.9l94.1 47c-.5 3.9-.7 7.8-.7 11.9c0 53 43 96 96 96s96-43 96-96s-43-96-96-96c-25.9 0-49.4 10.2-66.6 26.9l-94.1-47c.5-3.9 .7-7.8 .7-11.9s-.2-8-.7-11.9l94.1-47C302.6 213.8 326.1 224 352 224z'/></symbol>
          <symbol id='ic-share' viewBox='0 0 448 512'><path d='M256 80c0-17.7-14.3-32-32-32s-32 14.3-32 32V224H48c-17.7 0-32 14.3-32 32s14.3 32 32 32H192V432c0 17.7 14.3 32 32 32s32-14.3 32-32V288H400c17.7 0 32-14.3 32-32s-14.3-32-32-32H256V80z'/></symbol>
          <symbol id='ic-home' viewBox='0 0 576 512'><path d='M575.8 255.5C575.8 273.5 560.8 287.6 543.8 287.6H511.8L512.5 447.7C512.5 450.5 512.3 453.1 512 455.8V472C512 494.1 494.1 512 472 512H456C454.9 512 453.8 511.1 452.7 511.9C451.3 511.1 449.9 512 448.5 512H392C369.9 512 352 494.1 352 472V384C352 366.3 337.7 352 320 352H256C238.3 352 224 366.3 224 384V472C224 494.1 206.1 512 184 512H128.1C126.6 512 125.1 511.9 123.6 511.8C122.4 511.9 121.2 512 120 512H104C81.91 512 64 494.1 64 472V360C64 359.1 64.03 358.1 64.09 357.2V287.6H32.05C14.02 287.6 0 273.5 0 255.5C0 246.5 3.004 238.5 10.01 231.5L266.4 8.016C273.4 1.002 281.4 0 288.4 0C295.4 0 303.4 2.004 309.5 7.014L564.8 231.5C572.8 238.5 576.9 246.5 575.8 255.5L575.8 255.5z'/></symbol>
          <symbol id='ic-menu' viewBox='0 0 448 512'><path d='M192 176C192 202.5 170.5 224 144 224H48C21.49 224 0 202.5 0 176V80C0 53.49 21.49 32 48 32H144C170.5 32 192 53.49 192 80V176zM192 432C192 458.5 170.5 480 144 480H48C21.49 480 0 458.5 0 432V336C0 309.5 21.49 288 48 288H144C170.5 288 192 309.5 192 336V432zM256 80C256 53.49 277.5 32 304 32H400C426.5 32 448 53.49 448 80V176C448 202.5 426.5 224 400 224H304C277.5 224 256 202.5 256 176V80zM448 432C448 458.5 426.5 480 400 480H304C277.5 480 256 458.5 256 432V336C256 309.5 277.5 288 304 288H400C426.5 288 448 309.5 448 336V432z'/></symbol>
          <symbol id='ic-top' viewBox='0 0 24 24'><g transform='translate(12.000000, 12.000000) rotate(-180.000000) translate(-12.000000, -12.000000) translate(5.000000, 8.500000)'><path d='M14,0 C14,0 9.856,7 7,7 C4.145,7 0,0 0,0'/></g></symbol>
          <symbol id='ic-line' viewBox='0 0 24 24'><path d='M19.365 9.863c.349 0 .63.285.63.631 0 .345-.281.63-.63.63H17.61v1.125h1.755c.349 0 .63.283.63.63 0 .344-.281.629-.63.629h-2.386c-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63h2.386c.346 0 .627.285.627.63 0 .349-.281.63-.63.63H17.61v1.125h1.755zm-3.855 3.016c0 .27-.174.51-.432.596-.064.021-.133.031-.199.031-.211 0-.391-.09-.51-.25l-2.443-3.317v2.94c0 .344-.279.629-.631.629-.346 0-.626-.285-.626-.629V8.108c0-.27.173-.51.43-.595.06-.023.136-.033.194-.033.195 0 .375.104.495.254l2.462 3.33V8.108c0-.345.282-.63.63-.63.345 0 .63.285.63.63v4.771zm-5.741 0c0 .344-.282.629-.631.629-.345 0-.627-.285-.627-.629V8.108c0-.345.282-.63.63-.63.346 0 .628.285.628.63v4.771zm-2.466.629H4.917c-.345 0-.63-.285-.63-.629V8.108c0-.345.285-.63.63-.63.348 0 .63.285.63.63v4.141h1.756c.348 0 .629.283.629.63 0 .344-.282.629-.629.629M24 10.314C24 4.943 18.615.572 12 .572S0 4.943 0 10.314c0 4.811 4.27 8.842 10.035 9.608.391.082.923.258 1.058.59.12.301.079.766.038 1.08l-.164 1.02c-.045.301-.24 1.186 1.049.645 1.291-.539 6.916-4.078 9.436-6.975C23.176 14.393 24 12.458 24 10.314'/></symbol>
          <symbol id='ic-tumblr' viewBox='0 0 32 32'><path d='M16,2A14,14,0,1,0,30,16,14,14,0,0,0,16,2Zm0,26A12,12,0,1,1,28,16,12,12,0,0,1,16,28Z'/><path class='svgC' d='M20,19a1,1,0,0,0-1,1,1,1,0,0,1-1,1H17a1,1,0,0,1-1-1V15h3a1,1,0,0,0,0-2H16V10a1,1,0,0,0-2,0v3H12a1,1,0,0,0,0,2h2v5a3,3,0,0,0,3,3h1a3,3,0,0,0,3-3A1,1,0,0,0,20,19Z'/></symbol>
          <symbol id='ic-youtube' viewBox='0 0 576 512'><path d='M549.655 124.083c-6.281-23.65-24.787-42.276-48.284-48.597C458.781 64 288 64 288 64S117.22 64 74.629 75.486c-23.497 6.322-42.003 24.947-48.284 48.597-11.412 42.867-11.412 132.305-11.412 132.305s0 89.438 11.412 132.305c6.281 23.65 24.787 41.5 48.284 47.821C117.22 448 288 448 288 448s170.78 0 213.371-11.486c23.497-6.321 42.003-24.171 48.284-47.821 11.412-42.867 11.412-132.305 11.412-132.305s0-89.438-11.412-132.305zm-317.51 213.508V175.185l142.739 81.205-142.739 81.201z'/></symbol>
          <symbol id='ic-whatsapp' viewBox='0 0 64 64'><path d='M6.9,48.4c-0.4,1.5-0.8,3.3-1.3,5.2c-0.7,2.9,1.9,5.6,4.8,4.8l5.1-1.3c1.7-0.4,3.5-0.2,5.1,0.5 c4.7,2.1,10,3,15.6,2.1c12.3-1.9,22-11.9,23.5-24.2C62,17.3,46.7,2,28.5,4.2C16.2,5.7,6.2,15.5,4.3,27.8c-0.8,5.6,0,10.9,2.1,15.6 C7.1,44.9,7.3,46.7,6.9,48.4z M21.3,19.8c0.6-0.5,1.4-0.9,1.8-0.9s2.3-0.2,2.9,1.2c0.6,1.4,2,4.7,2.1,5.1c0.2,0.3,0.3,0.7,0.1,1.2 c-0.2,0.5-0.3,0.7-0.7,1.1c-0.3,0.4-0.7,0.9-1,1.2c-0.3,0.3-0.7,0.7-0.3,1.4c0.4,0.7,1.8,2.9,3.8,4.7c2.6,2.3,4.9,3,5.5,3.4 c0.7,0.3,1.1,0.3,1.5-0.2c0.4-0.5,1.7-2,2.2-2.7c0.5-0.7,0.9-0.6,1.6-0.3c0.6,0.2,4,1.9,4.7,2.2c0.7,0.3,1.1,0.5,1.3,0.8 c0.2,0.3,0.2,1.7-0.4,3.2c-0.6,1.6-2.1,3.1-3.2,3.5c-1.3,0.5-2.8,0.7-9.3-1.9c-7-2.8-11.8-9.8-12.1-10.3c-0.3-0.5-2.8-3.7-2.8-7.1 C18.9,22.1,20.7,20.4,21.3,19.8z'/></symbol>
          <symbol id='ic-pinterest' viewBox='0 0 64 64'><path d='M14.4,53.8c2.4,2,6.1,0.6,6.8-2.4l0-0.1c0.4-1.8,2.4-10.2,3.2-13.7c0.2-0.9,0.2-1.8-0.1-2.7 C24.2,34,24,32.8,24,31.5c0-4.1,2.4-7.2,5.4-7.2c2.5,0,3.8,1.9,3.8,4.2c0,2.6-1.6,6.4-2.5,9.9c-0.7,3,1.5,5.4,4.4,5.4 c5.3,0,8.9-6.8,8.9-14.9c0-6.1-4.1-10.7-11.6-10.7c-8.5,0-13.8,6.3-13.8,13.4c0,2.4,0.7,4.2,1.8,5.5c0.5,0.6,0.6,0.9,0.4,1.6 c-0.1,0.5-0.4,1.8-0.6,2.2c-0.2,0.7-0.8,1-1.4,0.7c-3.9-1.6-5.7-5.9-5.7-10.7c0-8,6.7-17.5,20-17.5c10.7,0,17.7,7.7,17.7,16 c0,11-6.1,19.2-15.1,19.2c-1.9,0-3.8-0.7-5.2-1.6c-0.9-0.6-2.1-0.1-2.4,0.9c-0.5,1.9-1.1,4.3-1.3,4.9c-0.1,0.5-0.3,0.9-0.4,1.4 c-1,2.7,0.9,5.5,3.7,5.7c2.1,0.1,4.2,0,6.3-0.3c12.4-2,22.1-12.2,23.4-24.7C61.5,18.1,48.4,4,32,4C16.5,4,4,16.5,4,32 C4,40.8,8.1,48.6,14.4,53.8z'/></symbol>
          <symbol id='ic-email' viewBox='0 0 500 500'><path d='M468.051,222.657c0-12.724-5.27-24.257-13.717-32.527 L282.253,45.304c-17.811-17.807-46.702-17.807-64.505,0L45.666,190.129c-8.448,8.271-13.717,19.803-13.717,32.527v209.054 c0,20.079,16.264,36.341,36.34,36.341h363.421c20.078,0,36.34-16.262,36.34-36.341V222.657z M124.621,186.402h250.758 c11.081,0,19.987,8.905,19.987,19.991v34.523c-0.088,4.359-1.818,8.631-5.181,11.997l-55.966,56.419l83.224,83.127 c6.904,6.904,6.904,18.081,0,24.985s-18.085,6.904-24.985,0l-85.676-85.672H193.034l-85.492,85.672 c-6.907,6.904-18.081,6.904-24.985,0c-6.906-6.904-6.906-18.081,0-24.985l83.131-83.127l-55.875-56.419 c-3.638-3.638-5.363-8.358-5.181-13.177v-33.343C104.632,195.307,113.537,186.402,124.621,186.402z'/></symbol>
          <symbol id='ic-tag' viewBox='0 0 512 512'><path d='M0 252.118V48C0 21.49 21.49 0 48 0h204.118a48 48 0 0 1 33.941 14.059l211.882 211.882c18.745 18.745 18.745 49.137 0 67.882L293.823 497.941c-18.745 18.745-49.137 18.745-67.882 0L14.059 286.059A48 48 0 0 1 0 252.118zM112 64c-26.51 0-48 21.49-48 48s21.49 48 48 48 48-21.49 48-48-21.49-48-48-48z'/></symbol>
          <symbol id='ic-comment' viewBox='0 0 512 512'><path d='M448 0H64C28.7 0 0 28.7 0 64v288c0 35.3 28.7 64 64 64h96v84c0 9.8 11.2 15.5 19.1 9.7L304 416h144c35.3 0 64-28.7 64-64V64c0-35.3-28.7-64-64-64z'/></symbol>
          <symbol id='ic-search' viewBox='0 0 24 24'><g transform='translate(2.000000, 2.000000)'><circle cx='9.76659044' cy='9.76659044' r='8.9885584'/><line x1='16.0183067' x2='19.5423342' y1='16.4851259' y2='20.0000001'/></g></symbol>
          <symbol id='ic-behance' viewBox='0 0 576 512'><path d='M232 237.2c31.8-15.2 48.4-38.2 48.4-74 0-70.6-52.6-87.8-113.3-87.8H0v354.4h171.8c64.4 0 124.9-30.9 124.9-102.9 0-44.5-21.1-77.4-64.7-89.7zM77.9 135.9H151c28.1 0 53.4 7.9 53.4 40.5 0 30.1-19.7 42.2-47.5 42.2h-79v-82.7zm83.3 233.7H77.9V272h84.9c34.3 0 56 14.3 56 50.6 0 35.8-25.9 47-57.6 47zm358.5-240.7H376V94h143.7v34.9zM576 305.2c0-75.9-44.4-139.2-124.9-139.2-78.2 0-131.3 58.8-131.3 135.8 0 79.9 50.3 134.7 131.3 134.7 61.3 0 101-27.6 120.1-86.3H509c-6.7 21.9-34.3 33.5-55.7 33.5-41.3 0-63-24.2-63-65.3h185.1c.3-4.2.6-8.7.6-13.2zM390.4 274c2.3-33.7 24.7-54.8 58.5-54.8 35.4 0 53.2 20.8 56.2 54.8H390.4z'/></symbol>
          <symbol id='ic-flickr' viewBox='0 0 448 512'><path d='M400 32H48C21.5 32 0 53.5 0 80v352c0 26.5 21.5 48 48 48h352c26.5 0 48-21.5 48-48V80c0-26.5-21.5-48-48-48zM144.5 319c-35.1 0-63.5-28.4-63.5-63.5s28.4-63.5 63.5-63.5 63.5 28.4 63.5 63.5-28.4 63.5-63.5 63.5zm159 0c-35.1 0-63.5-28.4-63.5-63.5s28.4-63.5 63.5-63.5 63.5 28.4 63.5 63.5-28.4 63.5-63.5 63.5z'/></symbol>
          <symbol id='ic-blogger' viewBox='0 0 448 512'><path d='M446.6 222.7c-1.8-8-6.8-15.4-12.5-18.5-1.8-1-13-2.2-25-2.7-20.1-.9-22.3-1.3-28.7-5-10.1-5.9-12.8-12.3-12.9-29.5-.1-33-13.8-63.7-40.9-91.3-19.3-19.7-40.9-33-65.5-40.5-5.9-1.8-19.1-2.4-63.3-2.9-69.4-.8-84.8.6-108.4 10C45.9 59.5 14.7 96.1 3.3 142.9 1.2 151.7.7 165.8.2 246.8c-.6 101.5.1 116.4 6.4 136.5 15.6 49.6 59.9 86.3 104.4 94.3 14.8 2.7 197.3 3.3 216 .8 32.5-4.4 58-17.5 81.9-41.9 17.3-17.7 28.1-36.8 35.2-62.1 4.9-17.6 4.5-142.8 2.5-151.7zm-322.1-63.6c7.8-7.9 10-8.2 58.8-8.2 43.9 0 45.4.1 51.8 3.4 9.3 4.7 13.4 11.3 13.4 21.9 0 9.5-3.8 16.2-12.3 21.6-4.6 2.9-7.3 3.1-50.3 3.3-26.5.2-47.7-.4-50.8-1.2-16.6-4.7-22.8-28.5-10.6-40.8zm191.8 199.8l-14.9 2.4-77.5.9c-68.1.8-87.3-.4-90.9-2-7.1-3.1-13.8-11.7-14.9-19.4-1.1-7.3 2.6-17.3 8.2-22.4 7.1-6.4 10.2-6.6 97.3-6.7 89.6-.1 89.1-.1 97.6 7.8 12.1 11.3 9.5 31.2-4.9 39.4z'/></symbol>
          <symbol id='ic-wordpress' viewBox='0 0 512 512'><path d='M256 8C119.3 8 8 119.2 8 256c0 136.7 111.3 248 248 248s248-111.3 248-248C504 119.2 392.7 8 256 8zM33 256c0-32.3 6.9-63 19.3-90.7l106.4 291.4C84.3 420.5 33 344.2 33 256zm223 223c-21.9 0-43-3.2-63-9.1l66.9-194.4 68.5 187.8c.5 1.1 1 2.1 1.6 3.1-23.1 8.1-48 12.6-74 12.6zm30.7-327.5c13.4-.7 25.5-2.1 25.5-2.1 12-1.4 10.6-19.1-1.4-18.4 0 0-36.1 2.8-59.4 2.8-21.9 0-58.7-2.8-58.7-2.8-12-.7-13.4 17.7-1.4 18.4 0 0 11.4 1.4 23.4 2.1l34.7 95.2L200.6 393l-81.2-241.5c13.4-.7 25.5-2.1 25.5-2.1 12-1.4 10.6-19.1-1.4-18.4 0 0-36.1 2.8-59.4 2.8-4.2 0-9.1-.1-14.4-.3C109.6 73 178.1 33 256 33c58 0 110.9 22.2 150.6 58.5-1-.1-1.9-.2-2.9-.2-21.9 0-37.4 19.1-37.4 39.6 0 18.4 10.6 33.9 21.9 52.3 8.5 14.8 18.4 33.9 18.4 61.5 0 19.1-7.3 41.2-17 72.1l-22.2 74.3-80.7-239.6zm81.4 297.2l68.1-196.9c12.7-31.8 17-57.2 17-79.9 0-8.2-.5-15.8-1.5-22.9 17.4 31.8 27.3 68.2 27.3 107 0 82.3-44.6 154.1-110.9 192.7z'/></symbol>
          <symbol id='ic-blog' viewBox='0 0 512 512'><path d='M217.6 96.1c-12.95-.625-24.66 9.156-25.52 22.37C191.2 131.7 201.2 143.1 214.4 143.1c79.53 5.188 148.4 74.09 153.6 153.6c.8281 12.69 11.39 22.43 23.94 22.43c.5156 0 1.047-.0313 1.578-.0625c13.22-.8438 23.25-12.28 22.39-25.5C409.3 191.8 320.3 102.8 217.6 96.1zM224 0C206.3 0 192 14.31 192 32s14.33 32 32 32c123.5 0 224 100.5 224 224c0 17.69 14.33 32 32 32s32-14.31 32-32C512 129.2 382.8 0 224 0zM172.3 226.8C157.7 223.9 144 235.8 144 250.6v50.37c0 10.25 7.127 18.37 16.75 21.1c18.13 6.75 31.26 24.38 31.26 44.1c0 26.5-21.5 47.1-48.01 47.1c-26.5 0-48.01-21.5-48.01-47.1V120c0-13.25-10.75-23.1-24.01-23.1l-48.01 .0076C10.75 96.02 0 106.8 0 120v247.1c0 89.5 82.14 160.2 175 140.7c54.38-11.5 98.27-55.5 109.8-109.7C302.2 316.1 247.8 241.8 172.3 226.8z'/></symbol>
          <symbol id='ic-skype' viewBox='0 0 448 512'><path d='M424.7 299.8c2.9-14 4.7-28.9 4.7-43.8 0-113.5-91.9-205.3-205.3-205.3-14.9 0-29.7 1.7-43.8 4.7C161.3 40.7 137.7 32 112 32 50.2 32 0 82.2 0 144c0 25.7 8.7 49.3 23.3 68.2-2.9 14-4.7 28.9-4.7 43.8 0 113.5 91.9 205.3 205.3 205.3 14.9 0 29.7-1.7 43.8-4.7 19 14.6 42.6 23.3 68.2 23.3 61.8 0 112-50.2 112-112 .1-25.6-8.6-49.2-23.2-68.1zm-194.6 91.5c-65.6 0-120.5-29.2-120.5-65 0-16 9-30.6 29.5-30.6 31.2 0 34.1 44.9 88.1 44.9 25.7 0 42.3-11.4 42.3-26.3 0-18.7-16-21.6-42-28-62.5-15.4-117.8-22-117.8-87.2 0-59.2 58.6-81.1 109.1-81.1 55.1 0 110.8 21.9 110.8 55.4 0 16.9-11.4 31.8-30.3 31.8-28.3 0-29.2-33.5-75-33.5-25.7 0-42 7-42 22.5 0 19.8 20.8 21.8 69.1 33 41.4 9.3 90.7 26.8 90.7 77.6 0 59.1-57.1 86.5-112 86.5z'/></symbol>
          <symbol id='ic-instagram' viewBox='0 0 448 512'><path d='M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z'/></symbol>
          <symbol id='ic-google-play' viewBox='0 0 512 512'><path d='M325.3 234.3L104.6 13l280.8 161.2-60.1 60.1zM47 0C34 6.8 25.3 19.2 25.3 35.3v441.3c0 16.1 8.7 28.5 21.7 35.3l256.6-256L47 0zm425.2 225.6l-58.9-34.1-65.7 64.5 65.7 64.5 60.1-34.1c18-14.3 18-46.5-1.2-60.8zM104.6 499l280.8-161.2-60.1-60.1L104.6 499z'/></symbol>
          <symbol id='ic-reddit' viewBox='0 0 512 512'><path d='M201.5 305.5c-13.8 0-24.9-11.1-24.9-24.6 0-13.8 11.1-24.9 24.9-24.9 13.6 0 24.6 11.1 24.6 24.9 0 13.6-11.1 24.6-24.6 24.6zM504 256c0 137-111 248-248 248S8 393 8 256 119 8 256 8s248 111 248 248zm-132.3-41.2c-9.4 0-17.7 3.9-23.8 10-22.4-15.5-52.6-25.5-86.1-26.6l17.4-78.3 55.4 12.5c0 13.6 11.1 24.6 24.6 24.6 13.8 0 24.9-11.3 24.9-24.9s-11.1-24.9-24.9-24.9c-9.7 0-18 5.8-22.1 13.8l-61.2-13.6c-3-.8-6.1 1.4-6.9 4.4l-19.1 86.4c-33.2 1.4-63.1 11.3-85.5 26.8-6.1-6.4-14.7-10.2-24.1-10.2-34.9 0-46.3 46.9-14.4 62.8-1.1 5-1.7 10.2-1.7 15.5 0 52.6 59.2 95.2 132 95.2 73.1 0 132.3-42.6 132.3-95.2 0-5.3-.6-10.8-1.9-15.8 31.3-16 19.8-62.5-14.9-62.5zM302.8 331c-18.2 18.2-76.1 17.9-93.6 0-2.2-2.2-6.1-2.2-8.3 0-2.5 2.5-2.5 6.4 0 8.6 22.8 22.8 87.3 22.8 110.2 0 2.5-2.2 2.5-6.1 0-8.6-2.2-2.2-6.1-2.2-8.3 0zm7.7-75c-13.6 0-24.6 11.1-24.6 24.9 0 13.6 11.1 24.6 24.6 24.6 13.8 0 24.9-11.1 24.9-24.6 0-13.8-11-24.9-24.9-24.9z'/></symbol>
          <symbol id='ic-google-news' viewBox='0 0 48 48'><path d='M37 7v2.54l-6.27-.7c-.68-.35-1.45-.54-2.25-.54-.28 0-.57.03-.85.08L11 11.23V7c0-1.1.9-2 2-2h22C36.1 5 37 5.9 37 7zM43.88 15.36l-.57 5.1C42.43 18.99 40.83 18 39 18h-4.64l-.95-5.54c-.02-.11-.04-.21-.07-.31L37 12.56l5.12.58C43.22 13.27 44.01 14.26 43.88 15.36zM31.31 18H9c-1.91 0-3.56 1.07-4.41 2.64L4.05 17.5c-.19-1.09.54-2.13 1.63-2.31l22.46-3.86c1.09-.18 2.12.55 2.31 1.64L31.31 18zM39 21H9c-1.1 0-2 .9-2 2v19c0 1.1.9 2 2 2h30c1.1 0 2-.9 2-2V23C41 21.9 40.1 21 39 21zM28.5 26h5c.83 0 1.5.67 1.5 1.5 0 .83-.67 1.5-1.5 1.5h-5c-.83 0-1.5-.67-1.5-1.5C27 26.67 27.67 26 28.5 26zM17.5 39c-3.58 0-6.5-2.92-6.5-6.5 0-3.58 2.92-6.5 6.5-6.5 1.42 0 2.76.45 3.89 1.29.67.5.8 1.44.3 2.1-.49.67-1.43.8-2.1.31-.6-.46-1.33-.7-2.09-.7-1.93 0-3.5 1.57-3.5 3.5s1.57 3.5 3.5 3.5c1.39 0 2.6-.82 3.16-2H17.5c-.83 0-1.5-.67-1.5-1.5 0-.83.67-1.5 1.5-1.5h5c.83 0 1.5.67 1.5 1.5C24 36.08 21.08 39 17.5 39zM33.5 39h-5c-.83 0-1.5-.67-1.5-1.5 0-.83.67-1.5 1.5-1.5h5c.83 0 1.5.67 1.5 1.5C35 38.33 34.33 39 33.5 39zM35.5 34h-7c-.83 0-1.5-.67-1.5-1.5 0-.83.67-1.5 1.5-1.5h7c.83 0 1.5.67 1.5 1.5C37 33.33 36.33 34 35.5 34z'/></symbol>
          <symbol id='ic-tiktok' viewBox='0 0 448 512'><path d='M448,209.91a210.06,210.06,0,0,1-122.77-39.25V349.38A162.55,162.55,0,1,1,185,188.31V278.2a74.62,74.62,0,1,0,52.23,71.18V0l88,0a121.18,121.18,0,0,0,1.86,22.17h0A122.18,122.18,0,0,0,381,102.39a121.43,121.43,0,0,0,67,20.14Z'/></symbol>
          <symbol id='ic-discord' viewBox='0 0 640 512'><path d='M524.531,69.836a1.5,1.5,0,0,0-.764-.7A485.065,485.065,0,0,0,404.081,32.03a1.816,1.816,0,0,0-1.923.91,337.461,337.461,0,0,0-14.9,30.6,447.848,447.848,0,0,0-134.426,0,309.541,309.541,0,0,0-15.135-30.6,1.89,1.89,0,0,0-1.924-.91A483.689,483.689,0,0,0,116.085,69.137a1.712,1.712,0,0,0-.788.676C39.068,183.651,18.186,294.69,28.43,404.354a2.016,2.016,0,0,0,.765,1.375A487.666,487.666,0,0,0,176.02,479.918a1.9,1.9,0,0,0,2.063-.676A348.2,348.2,0,0,0,208.12,430.4a1.86,1.86,0,0,0-1.019-2.588,321.173,321.173,0,0,1-45.868-21.853,1.885,1.885,0,0,1-.185-3.126c3.082-2.309,6.166-4.711,9.109-7.137a1.819,1.819,0,0,1,1.9-.256c96.229,43.917,200.41,43.917,295.5,0a1.812,1.812,0,0,1,1.924.233c2.944,2.426,6.027,4.851,9.132,7.16a1.884,1.884,0,0,1-.162,3.126,301.407,301.407,0,0,1-45.89,21.83,1.875,1.875,0,0,0-1,2.611,391.055,391.055,0,0,0,30.014,48.815,1.864,1.864,0,0,0,2.063.7A486.048,486.048,0,0,0,610.7,405.729a1.882,1.882,0,0,0,.765-1.352C623.729,277.594,590.933,167.465,524.531,69.836ZM222.491,337.58c-28.972,0-52.844-26.587-52.844-59.239S193.056,219.1,222.491,219.1c29.665,0,53.306,26.82,52.843,59.239C275.334,310.993,251.924,337.58,222.491,337.58Zm195.38,0c-28.971,0-52.843-26.587-52.843-59.239S388.437,219.1,417.871,219.1c29.667,0,53.307,26.82,52.844,59.239C470.715,310.993,447.538,337.58,417.871,337.58Z'/></symbol>
          <symbol id='ic-quora' viewBox='0 0 448 512'><path d='M440.5 386.7h-29.3c-1.5 13.5-10.5 30.8-33 30.8-20.5 0-35.3-14.2-49.5-35.8 44.2-34.2 74.7-87.5 74.7-153C403.5 111.2 306.8 32 205 32 105.3 32 7.3 111.7 7.3 228.7c0 134.1 131.3 221.6 249 189C276 451.3 302 480 351.5 480c81.8 0 90.8-75.3 89-93.3zM297 329.2C277.5 300 253.3 277 205.5 277c-30.5 0-54.3 10-69 22.8l12.2 24.3c6.2-3 13-4 19.8-4 35.5 0 53.7 30.8 69.2 61.3-10 3-20.7 4.2-32.7 4.2-75 0-107.5-53-107.5-156.7C97.5 124.5 130 71 205 71c76.2 0 108.7 53.5 108.7 157.7.1 41.8-5.4 75.6-16.7 100.5z'/></symbol>
          <symbol id='ic-arrow' viewBox='0 0 256 512'><path d='M64 448c-8.188 0-16.38-3.125-22.62-9.375c-12.5-12.5-12.5-32.75 0-45.25L178.8 256L41.38 118.6c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0l160 160c12.5 12.5 12.5 32.75 0 45.25l-160 160C80.38 444.9 72.19 448 64 448z'/></symbol>
          <symbol id='ic-print' viewBox='0 0 512 512'><path d='M448 192H64C28.65 192 0 220.7 0 256v96c0 17.67 14.33 32 32 32h32v96c0 17.67 14.33 32 32 32h320c17.67 0 32-14.33 32-32v-96h32c17.67 0 32-14.33 32-32V256C512 220.7 483.3 192 448 192zM384 448H128v-96h256V448zM432 296c-13.25 0-24-10.75-24-24c0-13.27 10.75-24 24-24s24 10.73 24 24C456 285.3 445.3 296 432 296zM128 64h229.5L384 90.51V160h64V77.25c0-8.484-3.375-16.62-9.375-22.62l-45.25-45.25C387.4 3.375 379.2 0 370.8 0H96C78.34 0 64 14.33 64 32v128h64V64z'/></symbol>
          <symbol id='ic-sitemap' viewBox='0 0 576 512'><path d='M208 80c0-26.5 21.5-48 48-48h64c26.5 0 48 21.5 48 48v64c0 26.5-21.5 48-48 48h-8v40H464c30.9 0 56 25.1 56 56v32h8c26.5 0 48 21.5 48 48v64c0 26.5-21.5 48-48 48H464c-26.5 0-48-21.5-48-48V368c0-26.5 21.5-48 48-48h8V288c0-4.4-3.6-8-8-8H312v40h8c26.5 0 48 21.5 48 48v64c0 26.5-21.5 48-48 48H256c-26.5 0-48-21.5-48-48V368c0-26.5 21.5-48 48-48h8V280H112c-4.4 0-8 3.6-8 8v32h8c26.5 0 48 21.5 48 48v64c0 26.5-21.5 48-48 48H48c-26.5 0-48-21.5-48-48V368c0-26.5 21.5-48 48-48h8V288c0-30.9 25.1-56 56-56H264V192h-8c-26.5 0-48-21.5-48-48V80z'/></symbol>
          <symbol id='ic-article' viewBox='0 0 384 512'><path d='M365.3 93.38l-74.63-74.64C278.6 6.742 262.3 0 245.4 0L64-.0001c-35.35 0-64 28.65-64 64l.0065 384c0 35.34 28.65 64 64 64H320c35.2 0 64-28.8 64-64V138.6C384 121.7 377.3 105.4 365.3 93.38zM336 448c0 8.836-7.164 16-16 16H64.02c-8.838 0-16-7.164-16-16L48 64.13c0-8.836 7.164-16 16-16h160L224 128c0 17.67 14.33 32 32 32h79.1V448zM96 280C96 293.3 106.8 304 120 304h144C277.3 304 288 293.3 288 280S277.3 256 264 256h-144C106.8 256 96 266.8 96 280zM264 352h-144C106.8 352 96 362.8 96 376s10.75 24 24 24h144c13.25 0 24-10.75 24-24S277.3 352 264 352z'/></symbol>
        </b:includable>
      </b:defaultmarkup>

      <b:defaultmarkup type='ContactForm'>
        <b:includable id='content'>
          <div class='contact-form-widget'>
            <div class='form'>
              <form name='contact-form'>

                <input class='contact-form-name' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/>
                <br/>
                <input class='contact-form-email' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg' name='email' size='30' type='text' value=''/>
                <br/>

                <textarea class='contact-form-email-message' cols='25' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg' name='email-message' rows='5'/>
                <br/>
                <input class='contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/>
                <div style='width: calc(100% - 80px);display: flex;float: left;height: 30px;align-items: center;'>
                  <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
                  <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
                </div>
              </form>
            </div>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='PopularPosts,FeaturedPost'>
        <b:includable id='snippetedPostContent'>
          <b:if cond='data:postDisplay.showFeaturedImage'>
            <a class='item-thumbnail Img-Holder thumb' expr:href='data:post.url' expr:title='data:messages.image'>
              <b:if cond='data:post.featuredImage'>
                <b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><span class='postcat'><data:post.labels.first.name/></span></b:if>
                <img expr:alt='data:messages.image' expr:data-src='data:post.featuredImage' height='108' width='192'/>
                <b:else/>
                <span class='Noimger'/>
              </b:if>
            </a>
          </b:if>
          <b:if cond='data:postDisplay.showTitle'><h3 class='posts post-title'><span class='Date published updated'><svg><use href='#ic-clock'/></svg><a class='agotime' expr:datetime='data:post.lastUpdated.iso8601' expr:href='data:post.url'/></span><a class='title' expr:href='data:post.url'><data:post.title/></a></h3></b:if>
          <b:if cond='data:postDisplay.showSnippet'><p class='snippet-item'><b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><data:post.snippets.short/></b:if></p>
          </b:if>
        </b:includable>
        <b:includable id='snippetedPosts'>
          <div expr:class='(data:postDisplay.showFeaturedImage ? &quot;ImgShow&quot; : &quot;Noimg&quot;)' role='feed'>
            <b:loop index='i' values='data:posts filter (p =&gt; p.id != data:view.postId)' var='post'>
              <article class='post' role='article'>
                <b:include name='snippetedPostContent'/>
              </article>
            </b:loop>
          </div>
        </b:includable>
      </b:defaultmarkup>

    </b:defaultmarkups>

    <b:tag name='script' type='text/javascript'>
      let BlogID = &quot;<data:blog.blogId/>&quot;,
      Url = &quot;<data:blog.canonicalHomepageUrl.https/>&quot;,
      blogger = &quot;https://www.blogger.com/&quot;,
      isPost = <data:view.isPost/>,
      isPage = <data:view.isPage/>,
      isHome = <data:view.isHomepage/>,
      isSingleItem = <data:view.isSingleItem/>,
      isMultipleItem = <data:view.isMultipleItems/>,
      agnow = &quot;منذ بضع لحظات&quot;;
      agminutes = &quot;منذ بضع دقائق&quot;;
      aghour = &quot;منذ ساعه&quot;;
      aghours = &quot;منذ بضع ساعات&quot;;
      agday = &quot;منذ يوم&quot;;
      agdays = &quot;منذ بضع ايام&quot;;
      agmonth = &quot;منذ شهر&quot;;
      agmonths = &quot;منذ بضع شهور&quot;;
      agYear = &quot;منذ عام&quot;;
      agYears = &quot;منذ بضع اعوام&quot;;
      ReadMore = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;read more&quot;<b:else/>&quot;اقرأ المزيد&quot;</b:if>,
      ReadMoreA = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;read more&quot;<b:else/>&quot;أكمل قرأة المقال&quot;</b:if>,
      ViewMore = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;view more&quot;<b:else/>&quot;عرض المزيد&quot;</b:if>,
      NextArticle = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;Next article&quot;<b:else/>&quot;المقال التالي&quot;</b:if>,
      PreviousArticle = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;Previous article&quot;<b:else/>&quot;المقال السابق&quot;</b:if>,
      Direction = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;left&quot;<b:else/>&quot;right&quot;</b:if>,
      page = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;page&quot;<b:else/>&quot;صفحة&quot;</b:if>,
      of = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;of&quot;<b:else/>&quot;من&quot;</b:if>,
      shareText = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;You cannot share the article on WhatsApp from a computer&quot;<b:else/>&quot;لا يمكنك مشاركة التدوينة على الواتساب من الحاسوب&quot;</b:if>,
      shareText2 = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;You cannot share the article on mail from a computer&quot;<b:else/>&quot;لا يمكنك مشاركة التدوينة على البريد من الحاسوب&quot;</b:if>,
      configtxt = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;Initializing link&quot;<b:else/>&quot;جاري تهيئة الرابط&quot;</b:if>,
      redytxt = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;link is ready&quot;<b:else/>&quot;الرابط جاهز&quot;</b:if>,
      errtxt = <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>&quot;Broken link&quot;<b:else/>&quot;رابط معطل&quot;</b:if>,
      nolapel = &quot;بدون قسم&quot;,
      minifun = &quot; دقائق للقراءة&quot;,
      replyfun = &quot;أترك ردا&quot;,
      cmtdelet = &quot;حذف التعليق&quot;,
      cmtShowMore = &quot;عرض المذيد من التعليقات&quot;,
      popup = false,
      BlogLang=&quot;<data:blog.locale/>&quot;,
      LazyAdsense = false,
      MaxTitle = true,
      MaxTitleNum = 10,
      bjsif = true,
      altImage = &#39;https://4.bp.blogspot.com/-ci3XMoAMGzg/WiCTxCLLWeI/AAAAAAAAPjI/UkV1sBTKC7EamOC_UmMJ4cQCv4xNNI82QCLcBGAs/s1600/log.jpg&#39;,
      AllowCom = false,
      commentjs = false,
      imgfilter = &#39;/s800-rw-e360-l50/&#39;,
      AdsenseUrl = &quot;&quot;;
      let LazyLoad = true;
      let UltraLazy = false;
      let Storg = &#39;storg&#39;;
      let skinclass = &#39;out&#39;;
      let CMTGlobal = {};
      let CMTLimt = 10;
      function Lazy(){}

      /*<![CDATA[*/ 

  // getScript Function
function $getScript(j,f,D){var k=document['createElement']('script');k['src']=j,k['onload']=function(){f();};if(D)k[D]=D;document['head']['append'](k);};
// getScript Function

// Document query ShortCode Function
window['_$'] = function (j) {
    var f = document['querySelectorAll'](j);
    if (f['length'] > 0x1) return f;
    else return f['length'] == 0x0 ? document['createDocumentFragment']()['childNodes'] : f[0x0];
}
// Document query ShortCode Function


function GetAgo(od){
    od = new Date(od);
    let nw = new Date()
    if(od.getUTCFullYear() < nw.getUTCFullYear()){
    let num = Math.abs(od.getUTCFullYear() - nw.getUTCFullYear());
    return (num <= 1) ? agYear : agYears;
}else if(od.getUTCMonth() < nw.getUTCMonth()){
    let num = Math.abs(od.getUTCMonth() - nw.getUTCMonth());
    return (num <= 1) ? agmonth : agmonths;
}else if(od.getUTCDate() < nw.getUTCDate()){
    let num = Math.abs(od.getUTCDate() - nw.getUTCDate());
    return (num <= 1) ? agday : agdays; 
}else if(od.getUTCHours() < nw.getUTCHours()){
    let num = Math.abs(od.getUTCHours() - nw.getUTCHours());
    return (num <= 1) ? aghour : aghours;
}else if(od.getUTCMinutes() < nw.getUTCMinutes()){
    let num = Math.abs(od.getUTCMinutes() - nw.getUTCMinutes());
    return (num <= 1) ? agminutes : agminutes;
}else{
    return agnow
}
}

/*]]>*/
    </b:tag>

    <style>
      #LinkList001 {overflow: unset!important;}

      /* cookie-choices */
      .cookie-choices-info{top:auto!important;bottom:70px!important;right:auto!important;left:20px!important;width:260px!important;padding:15px!important;background:var(--MinBgColor)!important;border:1px solid var(--Borderes3)!important;box-shadow:0 6px 18px 0 rgb(9 32 76 / 4%)!important;border-radius:10px!important;direction:ltr!important}
      .cookie-choices-info .cookie-choices-text{text-align: justify!important;color:var(--txtColor)!important;font-size:13px!important;margin:0!important;display:block!important;margin-bottom:15px!important}
      .cookie-choices-info .cookie-choices-buttons a{width:50%!important;flex-shrink:0!important;color:var(--whiteColor)!important;background:var(--minColor)!important;border-radius:30px!important;padding:7px 0!important;display:block!important;font-size:13px!important;font-family:sans-serif!important;text-transform:none!important}
      .cookie-choices-info .cookie-choices-buttons{margin:0!important;display:flex!important;align-items:center!important;justify-content:center!important}
      .cookie-choices-info .cookie-choices-button:first-of-type{margin-left:0!important}

      /* post add&#39;s */
      .post-body hr:before{content:&#39;\2027 \2027 \2027&#39;;display:block;text-align:center;font-size:24px;letter-spacing:0.6em;text-indent:0.6em;opacity:.8;clear:both}
      .post-body hr{margin:2em 0;border:0}
      /* textarea code &#39;s */
      /*<![CDATA[*/ 
textarea.code{min-height:200px;resize:vertical;width:100%;border-radius:3px;padding:0 15px;font-family:sans-serif;background:#f6f6f6;color:#2f3337;font-size:13px;line-height:1.8em;overflow:auto;border:1px solid var(--Borderes);margin:0;direction:ltr}
.areacode{position:relative;display:flex;overflow:hidden;clear:both;width:100%;padding:40px 0 0;background:#f6f6f6;margin:15px 0}
.areacode:before{content:'</>';position:absolute;left:0;top:0;background:inherit;color:var(--txtColor);font-size:12px;font-family:monospace;padding:5px 15px;z-index:2;line-height:30px}
.areacode:after{content:'أضغط لنسخ كل المحتويات';position:absolute;right:0;top:0;color:var(--txtColor);font-size:12px;font-family:sans-serif;padding:5px 15px;z-index:2;line-height:30px}
.dark-mode .areacode{background: var(--thrColor);}
.dark-mode .areacode textarea.code{background: var(--thrColor);}
      /*]]>*/
      /* button&#39;s */
      .post-body .button svg{vertical-align:middle;display:inline-block;width:18px;height:18px;fill:var(--whiteColor);stroke-width:1.5;margin-left:10px}
      .post-body .button.ln svg{fill:var(--txtColor)}
      .post-body .button{vertical-align: middle;text-align:center;top:0;transition:all .1s;position:relative;display:inline-block;margin:10px 0;padding:0 20px;border:0;border-radius:3px;line-height:35px;color:var(--whiteColor)!important;background:var(--minColor);font-size:14px;height:35px;white-space:nowrap;overflow:hidden;min-width:120px;opacity:.9}
      .post-body .button.ln{color:var(--txtColor)!important;background:transparent;border:1px solid  rgb(162 162 162 / 38%)}
      .post-body .button:hover {opacity: 1;}
      /* note&#39;s */
      .post-body .note{position:relative;padding:16px 55px 16px 20px;background:#e1f5fe;color:#3c4043;font-size:1rem;line-height:1.8em;border-radius:5px;overflow:hidden}
      .post-body .note::before{content:&#39;&#39;;width:60px;height:60px;background:#81b4dc;display:block;border-radius:8px;position:absolute;top:-10px;right:-10px;opacity:.1}
      .post-body .note::after{content:&#39;\2605&#39;;position:absolute;right:16px;top:11px;font-size:25px;min-width:15px;text-align:center}
      .post-body .note.wr:after,.post-body .note.aler:after {right: 17px;content: &#39;\0021&#39;;}
      .post-body .note.secs:after {content: &#39;\2714&#39;;font-size: 20px;}
      .post-body .note.wr{background:#ffdfdf;color:#48525c}
      .post-body .note.wr::before{background:#e65151}
      .post-body .note.aler {background: #fef5e7;}
      .post-body .note.aler:before {background: #3c3609;}
      .post-body .note.secs:before {background: #0d8540;}
      .post-body .note.secs {background: #e9f7ef;}
      /* tapel */
      .post-body  .table{display:block;overflow-y:hidden;overflow-x:auto;scroll-behavior:smooth}
      .post-body  table{margin:0 auto;font-size:14px}
      .post-body table{border-spacing:0}
      .post-body  table:not(.tr-caption-container){min-width:90%;border:1px solid  rgb(162 162 162 / 38%);border-radius:3px;overflow:hidden}
      .post-body  table th{padding:16px;text-align:inherit;border-bottom:1px solid  rgb(162 162 162 / 38%)}
      .post-body  table:not(.tr-caption-container) tr:nth-child(2n+1) td{background:rgba(0,0,0,.01)}
      .post-body  table:not(.tr-caption-container) tr:not(:last-child) td{border-bottom:1px solid  rgb(162 162 162 / 38%)}
      .post-body  table:not(.tr-caption-container) td{padding:16px}
      @media screen and (max-width:640px){.post-body .table{text-align: center;position:relative;width:calc(100% + 40px);left:-20px;right:-20px;padding:0 20px;display:flex}}

      @media print {
      div#shreeta5bar,.shBr.fixL,header,footer,aside,div#mobile-menu,div#backTop,.Dmode,.commentsection,.RelatedPosts.post-frome-tag,.author-posts,.pSh,.post-tags,.PostByCatRandom,.foqTitle,.post-meta,div#tocDiv,div#shreeta5bar,iframe,ins{display:none!important}.r-r{width:100%}body{background:#fff}.post .post-body,.post .blog-posts{padding:0!important;border:0!important;border-radius:0}.bobxed{padding:20px 0!important;margin-bottom:20px!important;}
      }
      <b:if cond='data:skin.vars.darckmodecolor == &quot;2px&quot;'>:root body.dark-mode{--BodyBG:#1e1e1e;--minColor:#1e1e1e;--minColorIc:#fff;--secColor:#1e1e1e;--thrColor:#2d2d30;--whiteColor:#ffffff;--hoverColor:#4e9f3d;--MinBgColor:#2d2d30;--txtColor:#ffffff;--TitColor:#ffffff;--SanColor:#eee;--Borderes:#404040;--Borderes2:#1e1e1e;--Borderes3:#404040;--PostTxtColor:#eee;--PostTitleColor:#ffffff;--PostLinkColor:#4e9f3d;--Hbg:#2d2d30;--HColor:#ffffff;--HtitleColor:#ffffff;--HbgIcon:#1e1e1e;--HCoIcon:#fff;--Cpc:#eee;--Cic:#fff;--Hok:#4e9f3d;--Sco:#4e9f3d;}</b:if>
      <b:if cond='data:skin.vars.disaplelastposts == &quot;2px&quot;'>.home.lapel #Tempnec {display: none !important;}.mopspeed.home.lapel #Tempnec{display:block!important}</b:if>
      <b:if cond='data:skin.vars.RemoveAuthor == &quot;2px&quot;'>.post-meta .authorPhoto, .post-meta .authorname, .author-posts{display: none !important;}</b:if>
      <b:if cond='data:skin.vars.RemoveAdiseHome == &quot;2px&quot;'><b:if cond='data:view.isMultipleItems'>.r-r {float: none;width: 100%;}aside{display: none!important;}</b:if></b:if>
      <b:if cond='data:skin.vars.RemoveAdisePost == &quot;2px&quot;'><b:if cond='data:view.isPost'>.r-r {float: none;width: 100%;}aside{display: none!important;}</b:if></b:if>
      <b:if cond='data:skin.vars.RemoveAdisePage == &quot;2px&quot;'><b:if cond='data:view.isPage'>.r-r {float: none;width: 100%;}aside{display: none!important;}</b:if></b:if>
      <b:if cond='data:skin.vars.StopCopying == &quot;2px&quot;'>body *{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}blockquote,blockquote *{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}</b:if>
      <b:if cond='data:skin.vars.CoverImg == &quot;1px&quot;'>.thumb img,img.post-thumbnail,.post-random a.reimage img, img.post-thumbnail {object-fit: initial;}</b:if>

      /* UbdateCSS */
      html{scroll-behavior:smooth}
      html[mode=&quot;dark&quot;] {color-scheme: dark;}
      .hide{display:none!important}
      .blog-admin{display:none}
      #PostA3lan2{display:none}
      .Noimger:before{content:&quot;No Image&quot;!important;font-size:21px;font-family:inherit!important}
      .Noimger{display:flex;align-items:center;justify-content:center;height:100%;width:100%;background:#eee;color:#08102b;position:absolute;right:0;top:0;border-radius:var(--ImgRadius)}
      .posts-from:before{border-top-color:var(--Cic);border-right-color:var(--Cic);content:&quot;&quot;;position:absolute}
      .spiner-icon{border-top-color:#989b9f;border-right-color:#989b9f;width:18px!important;height:18px!important;border-width:2px!important;margin-left:15px}
      .posts-from:before,.spiner-icon{width:30px;height:30px;border-width:4px;border-style:solid;border-bottom-color:transparent;border-left-color:transparent;border-radius:100%;animation:spin .5s infinite linear;transform:rotate(0deg)}
      @keyframes spin{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}
      .commentsShow .cshow{border-radius:3px;cursor:pointer;display:inline-block;transition:all .3s linear;opacity:0.6;font-size:13px;padding:6px 15px;margin-left:5px;color:#fff}
      .commentsShow .cshow:hover,.commentsShow .cshow.active{opacity:1}
      .commentsShow .cshow:last-of-type{margin-left:0}
      /* IconTOP */
      .toTopB {
      display: flex;
      align-items: center;
      justify-content: center;
      position: fixed;
      right: 27.5px;
      bottom: 27.5px;
      width: 45px;
      height: 45px;
      border-radius: 50%;
      cursor: pointer;
      visibility: hidden;
      opacity: 0;
      z-index: 5;
      transform: scale(0);
      transition: all 0.3s;
      }
      .toTopB.vsbl{visibility:visible;opacity:1;transform:scale(1)}
      .toTopB svg{height:100%;width:100%;-webkit-transform:rotate(-90deg);-ms-transform:rotate(-90deg);transform:rotate(-90deg);stroke-width:1.5;cursor:pointer}
      .toTopB svg .b{fill:var(--MinBgColor);stroke:var(--Borderes3);opacity:.9}
      .toTopB svg .c{fill:none;stroke:var(--Sco);stroke-dasharray:100 100;stroke-dashoffset:100;stroke-linecap:round}
      /* IconTOP */
      #lamiabutton,.Dmode{display:flex;align-items:center;justify-content:center;position:fixed;z-index:9;background:var(--MinBgColor);opacity:.9;width:55px;height:55px;border-radius:100%;right:22px;transition:all 0.3s;bottom:20px;cursor:pointer;box-shadow:0 0 15px rgb(0 0 0 / 8%)}
      #lamiabutton svg,.Dmode svg{width:23px;height:23px}
      #lamiabutton svg {fill: var(--minColorIc);}
      .hidden,#mobile-menu{display:none}
      svg.line,svg .line{width:20px;height:20px;fill:none!important;stroke:var(--minColorIc);stroke-linecap:round;stroke-linejoin:round;stroke-width:2}
      svg.line.linedd{fill:var(--minColorIc) !important;stroke:none}
      .Circalewhy label svg{width:22px;height:22px}
      g.d2{display:none}


      /* New Search */
      .searchformbox{display:flex;align-items:center;position:fixed;left:0;right:0;bottom:0;z-index:20;transition:all 0.3s;width:100%;height:100%;opacity:0;visibility:hidden}
      #NavC:checked ~ .searchformbox{opacity:1;visibility:visible}
      .fxbox{width:100%;max-width:680px;max-height:calc(100% - 60px);border-radius:12px;transition:inherit;z-index:3;display:flex;overflow:hidden;position:relative;margin:0 auto;box-shadow:0 5px 30px 0 rgb(0 0 0 / 5%)}
      div#searchform{padding:60px 20px 0;overflow:hidden;width:100%;background:var(--MinBgColor)}
      div#BlogSearch2{display:flex;background:inherit;position:absolute;top:0;left:0;right:0;padding:0;z-index:2;border-bottom:1px solid var(--Borderes)}
      div#BlogSearch2 form{position:relative;flex-grow:1}
      div#BlogSearch2 .sp{position:absolute;right:0;top:0;display:flex;align-items:center;padding:0 20px;z-index:3;opacity:.7;height:100%;background:transparent;border:0;outline:0}
      div#BlogSearch2 .sp svg{width:18px;height:18px}
      div#BlogSearch2 input{position:relative;display:block;background:var(--MinBgColor);border:0;outline:0;padding:10px 55px;width:100%;height:60px;transition:all 0.3s;z-index:2}
      div#BlogSearch2 button.sp{right:auto;left:0;opacity:0;font-size:12px;padding:0 15px}
      #BlogSearch2 button.sp:before{content:attr(data-text)}
      #BlogSearch2 input:focus ~ button.sp{opacity:.7}
      label.searchC{cursor: pointer;padding:0 20px;display:flex;align-items:center;border-right:1px solid var(--Borderes);justify-content:flex-end;position:relative;flex-shrink:0;min-width:40px}
      div#BlogSearch2 .sp svg, label.searchC,div#BlogSearch2 button.sp { stroke: var(--txtColor); color: var(--txtColor); }
      label.searchC:after{content:&#39;\2715&#39;;line-height:18px;font-size:14px}

      #BlogSearch2 input[type=search]::-ms-clear,#BlogSearch2 input[type=search]::-ms-reveal{display:none;appearance:none;width:0;height:0}
      #BlogSearch2 input[type=search]::-webkit-search-decoration,#BlogSearch2 input[type=search]::-webkit-search-cancel-button,.BlogSearch input[type=search]::-webkit-search-results-button,.BlogSearch input[type=search]::-webkit-search-results-decoration{display:none;-webkit-appearance:none;appearance:none}
      .dark-mode #BlogSearch2 input::placeholder {color: #ddd;}

      /* Start Header */
      img#Header1_headerimg {
      width: unset;
      height: unset;
      }
      .inline-icon{transition:all .3s linear;display:inline-block;vertical-align:middle;width:14px;height:14px;margin-left:5px;fill:var(--HColor)}
      #menu{opacity:0;overflow:unset!important}
      .HeaderBOT #menu ul{height:62px;display:flex;align-items:center;list-style:none}
      .HeaderBOT #menu ul li{flex-shrink:0;margin-left:15px;position:relative;padding:20px 0;transition:all .3s linear}
      #clicksearch,.open.nav1{display:flex;background:var(--HbgIcon);width:30px;height:31px;align-items:center;justify-content:center;border-radius:3px;cursor:pointer}
      #clicksearch svg,.open.nav1 svg{stroke-width:2;stroke:var(--HCoIcon)}
      .open.nav1,.searchHide{display:none!important}
      .HeaderTOP ul{display:flex!important;list-style:none}
      .HeaderTOP li {
      padding: 2px 5px;
      flex-shrink: 0;
      border-radius: 3px;
      }
      .HeaderTOP .social li:hover, #pages ul a:hover, #pages ul li.selected a {
      background: rgba(0,0,0,8%);
      }
      #pages ul a{transition:all .2s linear;display:block;color:var(--whiteColor);font-size:13px;padding:3px 8px;border-radius:3px}
      .sp-header .social a{display:flex;width:24px;height:27px;align-items:center;justify-content:center;background:transparent!important}
      .HTOPC &gt;div{flex-shrink:0;position:relative}
      .HRS{display:flex;align-items:center}
      .HRS &gt;div{flex-shrink:0}
        .sp-header{display:block;position:relative;margin-bottom:20px;height:100px}
        .HeaderBg{box-shadow: 0 6px 14px 0 rgb(9 32 76 / 5%);transition: all .3s linear;height:100px;width:100%;position:fixed;background:var(--Hbg);top:0;right:0;left:0;z-index:9}
        .sp-header .HeaderTOP .inline-icon{fill:var(--whiteColor)}
        .HeaderBOT #menu ul li:hover &gt; a,.HeaderBOT #menu ul a.selected{color:var(--hoverColor)}
        .HeaderBOT #menu ul li:hover &gt; .inline-icon,.HeaderBOT #menu ul a.selected .inline-icon,.HeaderBOT #menu ul a:hover .inline-icon{fill:var(--hoverColor)}
        .HeaderBOT #menu ul a{font:var(--HLinkfont);color:var(--HColor)}
          .HeaderTOP{transition:all .3s linear;display:block;width:100%;clear:both;height:35px;position:absolute;top:0;right:0;left:0;max-width:var(--maxWidth);margin:0 auto}
          .HeaderBOT{transition:all .3s linear;display:block;clear:both;position:absolute;top:35px;right:0;left:0;width:100%;position:relative}
          .sp-header.activeDown.active .HeaderBg{top:-100px}
          .sp-header.active #logo{top:0}
          .sp-header.active .HeaderBg .HeaderTOP{top:-35px}
          .sp-header.active .HeaderBg  .HeaderBOT{top:0}
          .sp-header.active .HeaderBg .HeaderBOT .HBOTC{height:100px}
        .Headerplace{color:#ffffff;width:76%;float:left;display:block;clear:both;position:relative;font-size:13px;padding:0 15px 0 0}
        .Headerplace:before{background:var(--minColor);color:#ffffff;width:2000px;display:block;clear:both;position:absolute;border-bottom-left-radius:15px;right:0;content:&quot;&quot;;border-bottom-right-radius:15px;height:35px}
        .HTOPC{margin:0 auto;width:100%;max-width:var(--maxWidth);display:flex;align-items:center;justify-content:space-between;height:35px}
        .HBOTC{position: relative;transition: all .3s linear;width:100%;max-width:var(--maxWidth);margin:0 auto;display:flex;align-items:center;justify-content:space-between;height:62px}
        .HeaderBOT #menu{width:calc((100% - 320px) /1)!important;top:0;flex-shrink:0}
        .HeaderBOT #logo,.HeaderTOP #logo{transition: all .3s linear;display:flex;justify-content:center;align-items:center;width:250px;height:70px;position:relative;font-size:1.5rem;top:-18px;flex-shrink:0}
        .HeaderBOT #logo a, .HeaderTOP #logo a {width: auto;height: auto;overflow: hidden;display: flex;align-items: center;justify-content: center;}


        .HeaderBg{position:relative}
        @media screen and (max-width: 1100px){.HTOPC, .HBOTC {width: 95%;}}
          @media screen and (max-width: 992px){
          .HeaderTOP,#menu{display:none}
          .HeaderBOT{top:0}
          .HeaderBg,.sp-header{height:92px}
          .HBOTC{height:92px}
          .HeaderBOT #logo,.HeaderTOP #logo{top:0}
          .open.nav1{display:flex!important}
          .sp-header.active .HBOTC{height:92px}
          .sp-header.active .HeaderBg{top:0;height:92px}
          }

    </style>

    <b:if cond='data:blog.adsenseClientId'>&lt;!--</b:if>&lt;/head&gt;&lt;!--</head><b:if cond='!data:blog.adsenseClientId'>--&gt;</b:if>

  <body expr:class='data:blog.languageDirection' expr:data-id='data:blog.blogId'>
    <b:class cond='data:view.isHomepage' name='home'/>
    <b:class cond='data:view.isSingleItem' name='post'/>
    <b:class cond='data:view.isMultipleItems' name='lapel'/>
    <b:class cond='data:view.isPage' name='page'/>

    <b:class cond='data:blog.view == &quot;ReadMode&quot;' name='readMode'/>

    <input class='navI hidden' id='offNav' type='checkbox'/>
    <input class='navM hidden' id='NavM' type='checkbox'/>




    <b:if cond='data:view.isPreview'>
      <b:if cond='!data:view.isSingleItem'>
        <div class='isPreview' style=' position: fixed; top: 0; right: 0; left: 0; bottom: 0; display: flex; align-items: center; justify-content: center; font-size: 25px; font-family: sans-serif !important; '>
          نموذج المعاينة يعمل فقط للمقالات والصفحات
        </div>
        <style>
          .contenarpage {display: none;}
        </style>
      </b:if>
    </b:if>
    <div class='contenarpage'>

      <b:if cond='!data:view.search.query'>
        <div class='TEMPsittings hide'>
          <b:if cond='data:view.isLayoutMode'><b:include name='HeaderSearch'/></b:if>
          <b:include name='MopileMenuLogo'/>
          <b:if cond='data:view.isLayoutMode'><b:include name='ArticaleSittings'/></b:if>
        </div>
      </b:if>
      <!-- start header -->
      <header class='sp-header' id='sp-header'>
          <div class='HeaderBg'>
            <div class='HeaderTOP'>
              <div class='Headerplace'>
                <div class='HTOPC'>
                  <b:include name='HeaderPages'/>
                  <b:include name='HeaderIcons'/>
                </div>
              </div>
            </div>
            <div class='HeaderBOT'>
              <div class='HBOTC'>
                <label aria-label='القائمة الرئيسي' class='open nav1' for='NavM' id='navMopile' onclick='openSidenav()'><svg class='line' viewBox='0 0 24 24'><line x1='3' x2='21' y1='12' y2='12'/><line x1='3' x2='21' y1='5' y2='5'/><line x1='3' x2='21' y1='19' y2='19'/></svg></label>
                <b:include name='HeaderLogo'/>
                <b:include name='HeaderLinks'/>
                <label aria-label='بحث' class='search' for='NavC' id='clicksearch'><svg class='line'><use href='#ic-search'/></svg></label>
              </div>
            </div>
          </div>

        <b:if cond='data:view.isLayoutMode'><b:include name='HeaderAds'/></b:if>

      </header>

      <!-- Header markups -->
      <b:defaultmarkups>
        <b:defaultmarkup type='Common'>
          <b:includable id='MopileMenuLogo'>
            <b:section id='MopileMenuLogo' maxwidgets='1' showaddelement='no'>
              <b:widget id='Image002' locked='true' title='لوجو قائمه الهاتف' type='Image' version='2' visible='true'>
                <b:includable id='main'><b:if cond='data:sourceUrl'><i class='hide dataheader' expr:site-dis='data:caption' expr:site-logo='data:sourceUrl' expr:site-title='data:title'/></b:if></b:includable>
                <b:includable id='content'/>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderLogo'>
            <b:section id='logo' maxwidgets='1' showaddelement='no'>
              <b:widget id='Header1' locked='true' title='GNN (رأس الصفحة)' type='Header' version='1'>
                <b:widget-settings>
                  <b:widget-setting name='displayUrl'>https://blogger.googleusercontent.com/img/a/AVvXsEj7VZQovn32mHMPvlsO48htnnfG7r7MqlrPYsFNEHXIK2wxCiJWSacPsSbrMAJJCHcVbHXTU26L9Zg47Bn1UVrzzSc0Sd0Oy2qhzX0WNE15jT8PhqmPmmkUs1JZx0le0gqSj_6OL6pRDpww-nQdKq-4RQSb2ORpc_RKbi36NvxECyze2tkBHkvABynV5XE=s375</b:widget-setting>
                  <b:widget-setting name='displayHeight'>135</b:widget-setting>
                  <b:widget-setting name='sectionWidth'>375</b:widget-setting>
                  <b:widget-setting name='useImage'>true</b:widget-setting>
                  <b:widget-setting name='shrinkToFit'>true</b:widget-setting>
                  <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
                  <b:widget-setting name='displayWidth'>375</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><b:include name='content'/></b:includable>
                <b:includable id='behindImageStyle'/>
                <b:includable id='content'><div id='header-inner'><b:if cond='data:useImage'><a class='img-logo' expr:href='data:blog.homepageUrl' expr:title='data:blog.title' style='display: flex'><b:if cond='data:sourceUrl'><img expr:alt='data:blog.title' expr:src='data:sourceUrl' expr:title='data:blog.title' height='70' id='Header1_headerimg' width='250'/></b:if></a><b:if cond='data:view.isHomepage'><h1 style='display: none'><data:blog.title/></h1><b:else/><h2 style='display: none'><data:blog.title/></h2></b:if><b:else/><div class='titlewrapper'><b:include name='title'/><b:include name='description'/></div></b:if></div></b:includable>
                <b:includable id='description'><p class='descriptionwrapper' style='display: none'><data:description/></p></b:includable>
                <b:includable id='image'>
                  <a class='header-image-wrapper' expr:href='data:blog.homepageUrl'>
                    <b:include data='{image: data:image,altText: data:blog.title.escaped,originalWidth: data:width,originalHeight: data:height}' name='responsiveImage'/>
                  </a>
                </b:includable>
                <b:includable id='title'><b:if cond='data:view.isHomepage'><h1 class='title'><a expr:href='data:blog.homepageUrl' expr:title='data:blog.title'><data:title/></a></h1><b:else/><h2 class='title'><a expr:href='data:blog.homepageUrl' expr:title='data:blog.title'><data:title/></a></h2></b:if></b:includable>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderPages'>
            <b:section id='pages' maxwidgets='1' showaddelement='no'>
              <b:widget id='PageList1' locked='true' title='الصفحات' type='PageList' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='pageListJson'><![CDATA[{"8241996477666669956":{"href":"https://www.gazanewsps.com/p/archives.html","position":4,"title":"الأرشيف"},"8209164165379706563":{"href":"https://www.gazanewsps.com/p/privacy-policy.html","position":0,"title":"سياسة الخصوصية"},"1481660813671076002":{"href":"https://www.gazanewsps.com/p/contact-us.html","position":3,"title":"اتصل بنا"},"161917100732309926":{"href":"https://www.gazanewsps.com/p/terms-conditions.html","position":1,"title":"اتفاقية الاستخدام"},"1318936276087349651":{"href":"https://www.gazanewsps.com/p/abut-us.html","position":2,"title":"من نحن"}}]]></b:widget-setting>
                  <b:widget-setting name='homeTitle'>الصفحة الرئيسية</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><b:include name='content'/></b:includable>
                <b:includable id='content'><div class='widget-content'><b:include name='pageList'/></div></b:includable>
                <b:includable id='overflowButton'/>
                <b:includable id='overflowablePageList'/>
                <b:includable id='pageLink'><li><b:class cond='data:view.url==data:link.href or data:blog.url==data:link.href' name='selected'/><a expr:href='data:link.href'><data:link.title/></a></li></b:includable>
                <b:includable id='pageList'><ul><b:class cond='data:pageListClass' expr:name='data:pageListClass'/><b:loop values='data:links' var='link'><b:include name='pageLink'/></b:loop></ul></b:includable>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderIcons'>
            <b:section id='topsocialL' maxwidgets='1' showaddelement='no'>
              <b:widget id='LinkList3' locked='true' title='مواقع التواصل الإجتماعي' type='LinkList' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='sorting'>NONE</b:widget-setting>
                  <b:widget-setting name='text-1'>Facebook</b:widget-setting>
                  <b:widget-setting name='link-1'><![CDATA[https://www.facebook.com/profile.php?id=61570650725890&mibextid=ZbWKwL]]></b:widget-setting>
                  <b:widget-setting name='text-0'>X</b:widget-setting>
                  <b:widget-setting name='link-2'>https://t.me/gazanewsps1</b:widget-setting>
                  <b:widget-setting name='link-0'><![CDATA[https://x.com/nornnna?t=y0uFGXR-XVdD4L_ndQ2Yzw&s=09]]></b:widget-setting>
                  <b:widget-setting name='text-2'>Telegram</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><b:include name='content'/></b:includable>
                <b:includable id='content'><ul class='social-static social'><b:loop values='data:links' var='link'><li><a expr:href='data:link.target' expr:title='data:link.name' rel='nofollow noopener' target='_blank'><svg><use expr:href='&quot;#ic-&quot; + data:link.name'/></svg></a></li></b:loop></ul></b:includable>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderLinks'>
            <b:section id='menu' maxwidgets='1' showaddelement='no'>
              <b:widget id='LinkList001' locked='true' title='القائمة الرئيسية' type='LinkList' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='link-5'>https://www.gazanewsps.com/search/label/%D8%A7%D9%84%D8%B5%D8%AD%D8%A9%20%D9%88%D8%A7%D9%84%D8%AC%D9%85%D8%A7%D9%84</b:widget-setting>
                  <b:widget-setting name='link-3'>https://www.gazanewsps.com/search/label/%D8%A7%D9%84%D9%85%D8%B3%D8%A7%D8%B9%D8%AF%D8%A7%D8%AA?m=1</b:widget-setting>
                  <b:widget-setting name='link-4'>https://www.gazanewsps.com/search/label/%D8%A7%D9%84%D9%88%D8%B8%D8%A7%D8%A6%D9%81?m=1</b:widget-setting>
                  <b:widget-setting name='text-1'>التعليم</b:widget-setting>
                  <b:widget-setting name='text-0'>الصفحة الرئيسية </b:widget-setting>
                  <b:widget-setting name='text-3'>المساعدات</b:widget-setting>
                  <b:widget-setting name='text-2'>أخبار</b:widget-setting>
                  <b:widget-setting name='text-5'>الصحة والجمال</b:widget-setting>
                  <b:widget-setting name='text-4'>الوظائف</b:widget-setting>
                  <b:widget-setting name='shownum'>7</b:widget-setting>
                  <b:widget-setting name='sorting'>NONE</b:widget-setting>
                  <b:widget-setting name='link-1'>https://www.gazanewsps.com/search/label/%D8%A7%D9%84%D8%AA%D8%B9%D9%84%D9%8A%D9%85?m=1</b:widget-setting>
                  <b:widget-setting name='link-2'>https://www.gazanewsps.com/search/label/%D8%A3%D8%AE%D8%A8%D8%A7%D8%B1?m=1</b:widget-setting>
                  <b:widget-setting name='link-0'>https://www.gazanewsps.com/</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><b:include name='content'/></b:includable>
                <b:includable id='content'>
                  <div class='widget-content'>
                    <ul>

                      <b:loop index='index' values='data:links' var='link'>
                        <b:if cond='data:link.name contains &quot;+&quot;'>

                            <b:if cond='data:index != 0'>
                              <b:eval expr='data:links[data:index - 1].name contains &quot;+&quot; ? &quot;&lt;/ul&gt;&lt;/li&gt;&quot; : &quot;&quot;'/>
                            </b:if>
                            &lt;li class=&#39;sitem&#39;&gt;
                            <a expr:href='data:link.target' expr:title='data:link.name'><data:link.name/></a>
                            <b:eval expr='data:links[data:index + 1].name contains &quot;+&quot; ? &quot;&lt;ul&gt;&quot; : &quot;&lt;/li&gt;&quot;'/>
                          <b:else/>
                          <b:if cond='data:index != 0'>
                            <b:eval expr='&quot;&lt;/ul&gt;&lt;/li&gt;&quot;'/>
                          </b:if>
                          <!-- start -->
                            &lt;li class=&#39;item&#39;&gt;
                            <a expr:href='data:link.target' expr:title='data:link.name'><b:class cond='data:view.url==data:link.target or data:blog.url==data:link.target' name='selected'/><data:link.name/></a>
                          <!-- start -->
                          <b:eval expr='data:index+1 == data:links.length ? &quot;&lt;/li&gt;&quot; : &quot;&lt;ul&gt;&quot;'/>
                        </b:if>
                      </b:loop>
                    </ul>
                  </div>

                </b:includable>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderAds'>
            <b:section class='HAD' cond='!data:view.isError and !data:blog.isMobileRequest' id='Topa3lan-sc' maxwidgets='1' showaddelement='no'>
              <b:widget id='HTML100' locked='true' title='اعلان اسفل القائمة العلوية للحاسوب' type='HTML' version='2' visible='false'>
                <b:widget-settings>
                  <b:widget-setting name='content'><![CDATA[<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-4294159533346602"
     crossorigin="anonymous"></script>
<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="fluid"
     data-ad-layout-key="-6g+ck-b-3y+i9"
     data-ad-client="ca-pub-4294159533346602"
     data-ad-slot="8707016258"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>]]></b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><div class='SeoPlusAds'><data:content/></div></b:includable>
              </b:widget>
            </b:section>
            <b:section cond='not data:view.isError and data:blog.isMobileRequest' id='Topa3lan-sc2' maxwidgets='1' showaddelement='no'>
              <b:widget id='HTML101' locked='true' title='اعلان اسفل القائمة العلوية للهاتف' type='HTML' version='2' visible='false'>
                <b:widget-settings>
                  <b:widget-setting name='content'/>
                </b:widget-settings>
                <b:includable id='main'><div class='SeoPlusAds'><data:content/></div></b:includable>
              </b:widget>
            </b:section>
          </b:includable>
          <b:includable id='HeaderSearch'>
            <div class='searchformbox'>
              <div class='fxbox'>
                <b:section id='searchform' maxwidgets='2' showaddelement='no'>
                  <b:widget id='BlogSearch2' locked='true' title='بحث ...' type='BlogSearch' version='2' visible='true'>
                    <b:includable id='main'>
                      <form class='sharef' expr:action='data:blog.searchUrl' role='search' target='_top'>
                        <label class='sp' for='searchIn'>
                          <svg class='line'><use href='#ic-search'/></svg>
                        </label>
                        <input autocomplete='off' expr:aria-label='data:messages.searchThisBlog' expr:placeholder='data:title' expr:value='data:view.isSearch ? data:view.search.query.escaped : &quot;&quot;' id='searchIn' minlength='3' name='q' required='required' type='search'/>
                        <button aria-label='Clear' class='sp' data-text='حذف' type='reset'/>
                      </form>
                      <label aria-label='Close' class='searchC' for='NavC'/>
                      <b:if cond='data:view.isHomepage'><b:tag name='script' type='application/ld+json'>{&quot;@context&quot;: &quot;http://schema.org&quot;,&quot;@type&quot;: &quot;WebSite&quot;,&quot;url&quot;: &quot;<data:blog.homepageUrl/>&quot;,&quot;potentialAction&quot;: [{&quot;@type&quot;: &quot;SearchAction&quot;,&quot;target&quot;: &quot;<data:blog.searchUrl/>?q={search_term_string}&quot;,&quot;query-input&quot;: &quot;required name=search_term_string&quot;}]}</b:tag></b:if>
                    </b:includable>
                    <b:includable id='content'/>
                    <b:includable id='searchForm'/>
                    <b:includable id='searchSubmit'/>
                  </b:widget>
                </b:section>
              </div>
              <label class='fCls searchbg' for='NavC'/>
            </div>
          </b:includable>

          <b:includable id='ArticaleSittings'>
            <b:section id='AddOns' maxwidgets='1' showaddelement='no'>
              <b:widget id='HTML1' locked='true' title='ميزة جدول التنقل' type='HTML' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='content'>جدول التنقل</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'><b:if cond='data:view.isPost'><style>div#tocDiv{user-select:none;display:block}</style><b:tag name='script' type='text/javascript'>/*<![CDATA[*/if(document.querySelector("#tocDiv")){var t = null,a = null,html="",e = 0;document.querySelectorAll(".amp-contnt h1,.amp-contnt h2, .amp-contnt h3, .amp-contnt h4").forEach(function(asd){asd.setAttribute("id", "Target"+e);var txt = asd.innerText;html+= "<li><a class='ScrolingToTarget' href='#Target"+e+"'>" + txt + "</a></li>";e++});/*]]>*/var Xhtml = `<div class='topcs7v'><b:class cond='data:title contains &quot;open&quot;' name='closed'/><div class='toctitle' expr:aria-label='data:content' for='naToc'><data:content/></div><ol id='tocList'>`+html+`</ol></div>`;/*<![CDATA[*/if (document.querySelectorAll('.amp-contnt h2, .amp-contnt h3, .amp-contnt h4').length != 0) {document.querySelector("#tocDiv").innerHTML = Xhtml;document.querySelectorAll(".ScrolingToTarget").forEach(function (asd) {asd.addEventListener("click", function (e) {e.preventDefault();document.querySelector(asd.getAttribute('href')).scrollIntoView({behavior: 'smooth'});});});document.querySelector('.toctitle').addEventListener('click', function (x) {document.querySelector('.topcs7v').classList.toggle('closed')});}}/*]]>*/</b:tag></b:if></b:includable>
              </b:widget>
              <b:widget id='ContactForm200' locked='true' title='نموذج الاتصال' type='ContactForm' version='2' visible='true'>
                <b:includable id='main'><b:if cond='data:view.isSingleItem'><b:include name='content'/></b:if></b:includable>
                <b:includable id='content'><div class='contact-form-widget'><div class='form'><form name='contact-form'><input class='contact-form-name' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/><br/><input class='contact-form-email' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg' name='email' size='30' type='text' value=''/><br/><textarea class='contact-form-email-message' cols='25' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg' name='email-message' rows='5'/><br/><input class='contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/><div style='width: calc(100% - 80px);display: flex;float: left;height: 30px;align-items: center;'><p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/><p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/></div></form></div></div></b:includable>
              </b:widget>
            </b:section>
          </b:includable>

        </b:defaultmarkup>
      </b:defaultmarkups>

      <label aria-label='Close Menu' class='pos-t-t' for='NavM'/><!-- start sidenav -->
      <div class='sidenav'>
        <div class='sidehead'><label aria-label='Close Menu' class='closemenu' for='NavM'/></div>
        <div class='SiteInfo'/>
        <div class='flexmenu'>
          <div class='mainmenu'/>
          <div class='bottommeny'>
            <div class='bottpage'/>
            <div class='bottsocial'/>
          </div>
        </div>
      </div><!-- end sidenav -->

      <input class='navC hidden' id='NavC' type='checkbox'/>
      <b:if cond='!data:view.isLayoutMode'><b:include name='HeaderSearch'/></b:if>

      <!-- end header -->

      <div class='container site'>

        <b:if cond='!data:view.isLayoutMode'>
          <b:if cond='data:view.isHomepage or data:view.isSingleItem'><b:include name='HeaderAds'/></b:if>
          </b:if>


        <div class='bocker'>
          <div class='r-r potg'>


            <b:section id='Tempnec' maxwidgets='1' showaddelement='no'>
              <b:widget id='Blog1' locked='true' title='رسائل المدونة الإلكترونية' type='Blog' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='commentLabel'>comments</b:widget-setting>
                  <b:widget-setting name='showShareButtons'>true</b:widget-setting>
                  <b:widget-setting name='authorLabel'>كتب:</b:widget-setting>
                  <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
                  <b:widget-setting name='timestampLabel'>-</b:widget-setting>
                  <b:widget-setting name='reactionsLabel'/>
                  <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
                  <b:widget-setting name='style.layout'>1x1</b:widget-setting>
                  <b:widget-setting name='showLocation'>false</b:widget-setting>
                  <b:widget-setting name='showTimestamp'>true</b:widget-setting>
                  <b:widget-setting name='postsPerAd'>1</b:widget-setting>
                  <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
                  <b:widget-setting name='showDateHeader'>false</b:widget-setting>
                  <b:widget-setting name='style.textcolor'>#ffffff</b:widget-setting>
                  <b:widget-setting name='showCommentLink'>true</b:widget-setting>
                  <b:widget-setting name='style.urlcolor'>#ffffff</b:widget-setting>
                  <b:widget-setting name='postLocationLabel'>Location:</b:widget-setting>
                  <b:widget-setting name='showAuthor'>true</b:widget-setting>
                  <b:widget-setting name='style.linkcolor'>#ffffff</b:widget-setting>
                  <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
                  <b:widget-setting name='showLabels'>true</b:widget-setting>
                  <b:widget-setting name='postLabelsLabel'/>
                  <b:widget-setting name='showBacklinks'>false</b:widget-setting>
                  <b:widget-setting name='showInlineAds'>false</b:widget-setting>
                  <b:widget-setting name='showReactions'>false</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
                  <b:if cond='data:view.isError'>
                    <b:include name='sp-errorPage'/>
                    <b:else/>
                    <b:if cond='not data:view.isSingleItem and not data:view.isError'>
                      <b:if cond='data:view.isHomepage'>
                        <div class='headline'>
                          <h2 class='title'><data:messages.latestPosts/></h2>
                          <a class='Lapel-Link' expr:href='data:blog.searchUrl'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>Show more<b:else/>عرض المزيد</b:if></a>
                        </div>
                        <b:else/>
                        <div class='headline'>
                          <h1 class='title'><b:if cond='data:blog.pageName'><data:blog.pageName/><b:else/><data:messages.latestPosts/></b:if></h1>
                        </div>
                      </b:if>
                    </b:if>


                    <div class='blog-posts hfeed'>
					<b:class cond='not data:view.isSingleItem' name='Sp-postsnew0'/> 

                      <b:if cond='data:view.isMultipleItems'><b:include name='postMetaHome'/></b:if>

                      <div class='Posts-byCategory'>
                        <b:loop index='i' values='data:posts' var='post'>
                          <b:include data='post' name='post'/>
                        </b:loop>
                      </div>
                    </div>
                  </b:if>
                  <b:include cond='data:view.isMultipleItems' name='sp-nextprev'/>
                </b:includable>
                <b:includable id='aboutPostAuthor'/>
                <b:includable id='addComments'/>
                <b:includable id='article-author'>
                  <!-- Post Author -->
                  <div class='article-author vcard'>

                    <b:if cond='data:post.author.authorPhoto.image'><img class='authorPhoto' expr:alt='data:messages.image' expr:data-src='data:post.author.authorPhoto.image' height='28' width='28'/></b:if>
                    <div class='metapost'>
                      <span class='fn authorname'><data:post.author.name/></span>
                      <div class='Times'><b:include data='post' name='article-time'/></div>
                    </div>
                  </div>
                </b:includable>
                <b:includable id='article-time'>
                  <b:if cond='data:widgets.Blog.first.allBylineItems.timestamp or data:view.isPage'>
                    <div class='article-timeago'>
                      اخر تحديث : <time class='agotime post-date published updated' expr:datetime='data:post.lastUpdated.iso8601'/>
                    </div>
                    <b:if cond='data:view.isPost'><div class='readTime'><span id='rdTime'/></div></b:if>
                  </b:if>
                </b:includable>
                <b:includable id='blogThisShare'/>
                <b:includable id='bylineByName' var='byline'/>
                <b:includable id='bylineRegion' var='regionItems'/>
                <b:includable id='commentAuthorAvatar'/>
                <b:includable id='commentDeleteIcon' var='comment'/>
                <b:includable id='commentForm' var='post'/>
                <b:includable id='commentFormIframeSrc' var='post'>
                  <a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=contempo&quot;' id='comment-editor-src' title='comment form link'/>
                </b:includable>
                <b:includable id='commentItem' var='comment'>
                  <!-- commentItem -->
                  <b:comment>
                    <li class='comment' expr:id='&quot;c&quot; + data:comment.id'>
                      <div class='CommentCounter'>
                        <div class='avatar-image-container'><b:if cond='data:comment.authorAvatarSrc contains &quot;blank.gif&quot;'><span class='noimg'/><b:else/><img expr:alt='data:comment.author' expr:data-src='resizeImage(data:comment.authorAvatarSrc, (data:comment.inReplyTo ? &quot;48&quot; : &quot;48&quot;) , &quot;1:1&quot;)' height='48' width='48'/></b:if></div>
                        <div class='comment-block'>
                          <div class='comment-header'>
                            <cite expr:class='data:comment.author == data:post.author.name ? &quot;user blog-author&quot; : &quot;user&quot;'><b:if cond='data:comment.authorUrl'><data:comment.author/><b:else/><data:comment.author/></b:if></cite>
                            <span class='datetime com-date' expr:data-date='data:comment.timestampAbs'><data:comment.timestamp/></span>
                          </div>	
                          <p class='comment-content'><data:comment.body/></p>
                          <span class='comment-actions secondary-text'>
                            <b:if cond='not data:comment.inReplyTo'><span class='comment-reply' expr:data-comment-id='data:comment.id'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>reply<b:else/>إرسال رد</b:if></span></b:if><span expr:class='data:comment.adminClass'><a expr:href='data:comment.deleteUrl' rel='nofollow noreferrer' target='_blank'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>delete<b:else/>حذف</b:if></a></span></span>
                        </div>
                      </div>
                      <div class='comment-replies'><ul><b:loop values='data:post.comments where (c=&gt; c.inReplyTo == data:comment.id)' var='reply'><b:include data='reply' name='commentItem'/></b:loop></ul></div>
                    </li>
                  </b:comment>
                </b:includable>
                <b:includable id='commentList' var='comments'/>
                <b:includable id='commentPicker' var='post'>

                  <div class='commentsection'>
                    <section class='topic-comments' id='item-comments'>
                      <div class='headline'>
                        <div class='title'><data:messages.comments/></div>
                        <div class='commentsShow'/>
                      </div>
                    </section>
                    <div id='commentsBlog'>
                      <div class='comments' id='comments'>

                        <div class='BloggerComment'>
                          <b:if cond='data:post.allowComments'>
                            <b:include data='post' name='threadedComments'/>
                          </b:if>
                        </div>
                        <div class='DisqusComment'/>
                        <div class='FacebookComment'/>

                      </div>
                    </div>

                  </div>



                </b:includable>
                <b:includable id='comments' var='post'>
                  <!-- commentItem -->
                  <b:comment>
                    <ul><b:loop values='data:post.comments where (c=&gt; not c.inReplyTo)' var='comment'><b:include data='comment' name='commentItem'/></b:loop></ul>
                    <b:if cond='data:post.commentPagingRequired'><div id='loadmore'><a class='ribble'><span><data:messages.moreEllipsis/></span></a></div></b:if>
                  </b:comment>
                </b:includable>
                <b:includable id='commentsLink'/>
                <b:includable id='commentsLinkIframe'/>
                <b:includable id='commentsTitle'/>
                <b:includable id='defaultAdUnit'/>
                <b:includable id='emailPostIcon'/>
                <b:includable id='facebookShare'/>
                <b:includable id='feedLinks'/>
                <b:includable id='feedLinksBody' var='links'/>
                <b:includable id='footerBylines'/>
                <b:includable id='googlePlusShare'/>
                <b:includable id='headerByline'/>
                <b:includable id='homePageLink'/>
                <b:includable id='iframeComments' var='post'/>
                <b:includable id='inlineAd' var='post'/>
                <b:includable id='linkShare'/>
                <b:includable id='manageComments'/>
                <b:includable id='nextPageLink'/>
                <b:includable id='otherSharingButton'/>
                <b:includable id='platformShare'/>
                <b:includable id='post' var='post'>

                  <article class='post-amp post hentry h-entry ' role='article'>
                    <b:class cond='!data:view.isSingleItem' name='posts'/>
                    <b:class cond='!data:view.isSingleItem' expr:name='&quot;postnum&quot; + data:i'/>

                    <b:if cond='data:view.isSingleItem'>
                      <b:if cond='data:post.body contains &quot;outSideSchemaSeoPlus&quot;'>
                        <b:else/>
                        <b:include data='post' name='postMeta'/>
                      </b:if>
                    </b:if>
                    <b:if cond='not data:view.isSingleItem'>
                      <b:include data='post' name='sp-homePosts'/>
                      <b:else/>
                      <div class='bobxed'>            
                        <div class='foqTitle'>
                          <b:if cond='data:post.labels.first'><a class='postTopTag' expr:href='data:post.labels.first.url' expr:title='data:post.labels.first.name'><data:post.labels.first.name/></a></b:if>

                        </div>

                        <b:include data='post' name='postTitle'/>
                        <div class='post-meta'>
                          <div class='au-ti'>
                            <b:include data='post' name='article-author'/>
                          </div>
                        </div>
                        <div class='TocList'/>

                      </div>
                      <b:include data='post' name='postBody'/>
                      <div class='hideensa'>
                        <b:include data='post' name='sp-postTags'/>
                        <b:include data='post' name='sp-sharePost'/>

                        <b:if cond='data:skin.vars.nextprev == &quot;1px&quot;'>
                          <b:include cond='data:view.isPost' data='post' name='sp-navigation'/>
                        </b:if>

                        <b:include data='post' name='sp-aboutPostAuthor'/>

                          <b:include cond='data:view.isPost' data='post' name='sp-RelatedPosts'/>
                      </div>

                      <b:if cond='data:post.allowComments'>
                        <script>
                          let POSTID = &quot;<data:post.id/>&quot;;
                          let comNum = <data:post.numberOfComments/>;
                          AllowCom = <data:post.allowNewComments/>;
                        </script>
                        <b:include cond='data:view.isSingleItem' data='post' name='commentPicker'/>

                      </b:if>

                    </b:if>
                  </article>
                </b:includable>
                <b:includable id='postAuthor'/>
                <b:includable id='postAuthorProfile' var='post'/>
                <b:includable id='postBody' var='post'>
                  <div class='amp-contnt post-body entry-content float-container'>
                    <b:if cond='data:view.isPost'><b:if cond='data:post.body contains &quot;↔&quot; or data:post.body contains &quot;↚&quot;'><b:else/><div id='top-a3lan'/></b:if></b:if>
                    <b:if cond='data:view.isPost'><b:if cond='data:post.body contains &quot;↔&quot; or data:post.body contains &quot;↚&quot; or data:post.body contains &quot;tocDiv&quot;'><b:else/><div id='tocDiv'/></b:if></b:if>
                    <data:post.body/>


                    <b:if cond='data:view.isPost'><b:if cond='data:post.body contains &quot;↔&quot; or data:post.body contains &quot;↚&quot;'><b:else/><div id='bot-a3lan'/></b:if></b:if>

                    <b:include cond='data:post.body contains &quot;ArchivePage&quot; and data:view.isPage' name='Archive'/> 

                    <div class='PostEdit blog-admin'><a class='noredi' expr:href='data:view.isPost ? &quot;https://www.blogger.com/blog/post/edit/&quot; + data:blog.blogId + &quot;/&quot; + data:post.id : &quot;https://www.blogger.com/blog/page/edit/&quot; + data:blog.blogId + &quot;/&quot; + data:post.id' rel='nofollow noopener' target='_blank'><b:if cond='data:view.isPost'>تعديل المقال<b:else/>تعديل الصفحة</b:if></a></div>


                  </div>
                </b:includable>
                <b:includable id='postBodySnippet' var='post'/>
                <b:includable id='postCommentsAndAd' var='post'/>
                <b:includable id='postCommentsLink'/>
                <b:includable id='postFooter' var='post'/>
                <b:includable id='postFooterAuthorProfile' var='post'/>
                <b:includable id='postHeader' var='post'/>
                <b:includable id='postInfoShareMore'>
                  <input class='shIn fixi hidden' id='forShare' type='checkbox'/>
                  <div class='shBr fixL'>
                    <div class='shBri fixLi'>
                      <div class='shBrs fixLs'>
                        <div class='shH fixH fixT' expr:data-text='data:messages.shareToOtherApps'>
                          <label aria-label='أغلاق' class='c cl' for='forShare'/>
                        </div>
                        <div class='shC social'>
                          <!--[ Share to other apps ]-->
                          <div class='shL'>
                            <div data-text='Facebook'>
                              <!-- Share to Facebook -->
                              <a aria-label='Facebook' expr:href='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='facebook'>
                                <svg class='n-line'><use href='#ic-facebook'/></svg>
                              </a>
                            </div>

                            <div data-text='WhatsApp'>
                              <!-- Share to Whatsapp -->
                              <a aria-label='Whatsapp' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='whatsapp'>
                                <svg class='n-line'><use href='#ic-whatsapp'/></svg>
                              </a>
                            </div>

                            <div data-text='Twitter'>
                              <!-- Share to Twitter -->
                              <a aria-label='Twitter' expr:href='&quot;https://twitter.com/share?url=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='twitter'>
                                <svg class='n-line'><use href='#ic-twitter'/></svg>
                              </a>
                            </div>

                            <div data-text='Telegram'>
                              <!-- Share to Telegram -->
                              <a aria-label='Telegram' expr:href='&quot;https://t.me/share/url?url=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='telegram'>
                                <svg class='n-line'><use href='#ic-telegram'/></svg>
                              </a>
                            </div>

                            <div data-text='Pinterest'>
                              <!-- Pin to Pinterst -->
                              <a aria-label='Pinterest' data-pin-config='beside' expr:href='&quot;https://pinterest.com/pin/create/button/?url=&quot; + data:blog.url.canonical + &quot;&amp;media=&quot; + resizeImage(data:blog.postImageUrl, 1600)' rel='noopener' target='_blank' title='pinterest'>
                                <svg class='n-line'><use href='#ic-pinterest'/></svg>
                              </a>
                            </div>

                            <div data-text='LinkedIn'>
                              <!-- Share Linkedin -->
                              <a aria-label='Linkedin' expr:href='&quot;https://www.linkedin.com/sharing/share-offsite/?url=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='linkedin'>
                                <svg class='n-line'><use href='#ic-linkedin'/></svg>
                              </a>
                            </div>

                            <div data-text='Line'>
                              <!-- Share to Line -->
                              <a aria-label='Line' expr:href='&quot;https://timeline.line.me/social-plugin/share?url=&quot; + data:blog.url.canonical' rel='noopener' target='_blank' title='line'>
                                <svg class='n-line'><use href='#ic-line'/></svg>
                              </a>
                            </div>

                            <div data-text='Email'>
                              <!-- Send to email -->
                              <a aria-label='Email' expr:href='&quot;mailto:?body=&quot; + data:blog.url.canonical' target='_blank' title='email'>
                                <svg class='n-line'><use href='#ic-email'/></svg>
                              </a>
                            </div>

                            <div data-text='reddit'>
                              <!-- Send to reddit -->
                              <a aria-label='reddit' expr:href='&quot;https://www.reddit.com/submit?url=&quot; + data:blog.url.canonical' target='_blank' title='reddit'>
                                <svg class='n-line'><use href='#ic-reddit'/></svg>
                              </a>
                            </div>

                            <div data-text='print'>
                              <!-- Send to print -->
                              <a aria-label='print' href='javascript:window.print()' title='print'>
                                <svg class='n-line'><use href='#ic-print'/></svg>
                              </a>
                            </div>

                          </div>

                        </div>
                      </div>
                    </div>

                    <label class='fCls sharebg' for='forShare'/>
                  </div>
                </b:includable>
                <b:includable id='postJumpLink' var='post'/>
                <b:includable id='postLabels'/>
                <b:includable id='postLocation'/>
                <b:includable id='postMeta' var='post'>
                  <script type='application/ld+json'>{&quot;@context&quot;: &quot;http://schema.org&quot;,&quot;@type&quot;: &quot;BlogPosting&quot;,&quot;mainEntityOfPage&quot;: {&quot;@type&quot;: &quot;WebPage&quot;,&quot;@id&quot;: &quot;<data:post.url.canonical/>&quot;},&quot;headline&quot;: &quot;<data:post.title.escaped/>&quot;,&quot;description&quot;: &quot;<data:post.snippets.short.escaped/>&quot;,<b:if cond='data:post.labels'>&quot;keywords&quot;:&quot;<b:loop index='l' values='data:post.labels' var='label'><data:label.name/><b:if cond='data:l != data:post.labels.length - 1'>,</b:if></b:loop>&quot;,</b:if>&quot;datePublished&quot;: &quot;<data:post.date.iso8601/>&quot;,&quot;dateModified&quot;: &quot;<data:post.lastUpdated.iso8601/>&quot;,&quot;image&quot;: {&quot;@type&quot;: &quot;ImageObject&quot;,&quot;url&quot;: &quot;<b:eval expr='data:post.firstImageUrl ? resizeImage(data:post.firstImageUrl, 1200, &quot;1200:630&quot;) : &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;'/>&quot;,&quot;height&quot;: <b:eval expr='data:post.firstImageUrl ? 630 : 348'/>,&quot;width&quot;: 1200},&quot;publisher&quot;: {&quot;@type&quot;: &quot;Organization&quot;,&quot;name&quot;: &quot;<data:blog.title/>&quot;,&quot;logo&quot;: {&quot;@type&quot;: &quot;ImageObject&quot;,&quot;url&quot;: &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;: 206,&quot;height&quot;: 60}},&quot;author&quot;: {&quot;@type&quot;: &quot;Person&quot;,&quot;jobTitle&quot;: &quot;Author&quot;,&quot;url&quot;: &quot;<b:if cond='data:post.author.profileUrl'><data:post.author.profileUrl/><b:else/>#</b:if>&quot;,&quot;name&quot;: &quot;<data:post.author.name/>&quot;}}</script>

                </b:includable>
                <b:includable id='postMetaHome'>
                  <b:tag name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;ItemList&quot;,&quot;itemListElement&quot;:[<b:loop index='i' values='data:posts' var='post'>{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:<b:eval expr='data:i + 1'/>,&quot;url&quot;:&quot;<data:post.url/>&quot;}<b:if cond='data:i != data:posts.length - 1'>,</b:if></b:loop>]}</b:tag>
                  <b:if cond='data:view.isLabelSearch'>
                    <b:tag cond='data:view.isLabelSearch' name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;item&quot;:{&quot;@id&quot;:&quot;<data:blog.homepageUrl/>&quot;,&quot;name&quot;:&quot;<data:blog.title/>&quot;}},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;item&quot;:{&quot;@id&quot;:&quot;<data:blog.searchUrl/>&quot;,&quot;name&quot;:&quot;search&quot;}},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;item&quot;:{&quot;@id&quot;:&quot;<data:view.url.canonical/>&quot;,&quot;name&quot;:&quot;<data:view.search.label/>&quot;}}]}</b:tag>
                  </b:if>
                </b:includable>
                <b:includable id='postMetadataJSONImage'/>
                <b:includable id='postMetadataJSONPublisher'/>
                <b:includable id='postPagination'/>
                <b:includable id='postReactions'/>
                <b:includable id='postShareButtons'/>
                <b:includable id='postTimestamp'/>
                <b:includable id='postTitle' var='post'>
                  <h1 class='entry-title topic-title'><data:post.title/></h1>
                </b:includable>
                <b:includable id='previousPageLink'/>
                <b:includable id='sharingButton'/>
                <b:includable id='sharingButtonContent'/>
                <b:includable id='sharingButtons'/>
                <b:includable id='sharingButtonsMenu'/>
                <b:includable id='sharingPlatformIcon'/>
                <b:includable id='sp-RelatedPosts' var='post'>

                  <div id='ret-a3lan'/>
                  <div class='RelatedPosts'>
                    <b:loop index='i' values='data:post.labels' var='label'>
                      <b:if cond='data:i == 0'>
                        <div class='headline RelatedPost'><h3 class='title'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>You may like these posts<b:else/>مقالات قد تهمك</b:if></h3></div>
                      </b:if>
                    </b:loop>
                    <div class='PostByCat Sp-posts1'><b:loop index='i' values='data:post.labels' var='label'><b:if cond='data:i == 0'><i class='posts-from' data-index='1' data-number='6' data-type='RetPosts' expr:data-label='data:label.name' style='height: 485px'/>

                      </b:if></b:loop></div>
                  </div>

                </b:includable>
                <b:includable id='sp-aboutPostAuthor' var='post'>

                  <b:if cond='data:view.isPost'>
                    <b:tag name='script' type='text/javascript'>let AuthorName=&quot;<data:post.author.name/>&quot;</b:tag>

                    <b:if cond='data:post.author.aboutMe'><div class='author-posts'>

                      <div class='authorImage'>
                        <div class='authorImg'>
                          <b:if cond='data:post.author.authorPhoto.image'>
                            <img expr:alt='data:post.author.name' expr:data-src='resizeImage(data:post.author.authorPhoto.image , &quot;1600&quot; )' expr:title='data:post.author.name' height='60' width='60'/>
                            <b:else/>
                            <img data-src='https://4.bp.blogspot.com/-ci3XMoAMGzg/WiCTxCLLWeI/AAAAAAAAPjI/UkV1sBTKC7EamOC_UmMJ4cQCv4xNNI82QCLcBGAs/s1600/log.jpg' expr:alt='data:post.author.name' expr:title='data:post.author.name' height='60' width='60'/>
                          </b:if>
                        </div>
                      </div>

                      <div class='authorInfo'>

                        <div class='author-name'>
                          بواسطة : <data:post.author.name/>
                        </div>
                        <div class='author-desc'>
                          <data:post.author.aboutMe/>
                        </div>

                      </div>

                      </div></b:if>
                  </b:if>

                </b:includable>
                <b:includable id='sp-errorPage'>
                  <div id='error-page'>
                    <svg style='width:300px;fill:var(--minColor)' viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'><path d='M256 32c14.2 0 27.3 7.5 34.5 19.8l216 368c7.3 12.4 7.3 27.7 .2 40.1S486.3 480 472 480H40c-14.3 0-27.6-7.7-34.7-20.1s-7-27.8 .2-40.1l216-368C228.7 39.5 241.8 32 256 32zm0 128c-13.3 0-24 10.7-24 24V296c0 13.3 10.7 24 24 24s24-10.7 24-24V184c0-13.3-10.7-24-24-24zm32 224c0-17.7-14.3-32-32-32s-32 14.3-32 32s14.3 32 32 32s32-14.3 32-32z'/></svg>
                    <h1 class='errornum'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>
                      ERROR 404
                      <b:else/>
                      خطأ 404
                      </b:if></h1>
                    <h2 class='error'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>
                      Sorry, the page you are looking for in this blog is not available.
                      <b:else/>
                      معذرة, فالصفحة التي تبحث عنها في هذه المدونة ليست متوفرة.
                      </b:if></h2>
                  </div>
                  <style>
                    div#error-page {
                    display: block;
                    text-align: center;
                    padding: 30px;
                    height: calc((100vh - 245px));
                    }
                    .r-r {
                    float: none;
                    width: 100%;
                    }
                    h1.errornum {
                    font-size: 80px;
                    }
                    h2.error {
                    font-size: 23px;
                    color: #4e4e4e;
                    }

                    @media screen and (max-width:992px){div#error-page {height:auto;}}
                  </style>
                </b:includable>
                <b:includable id='sp-homePosts' var='post'>

                  <a class='Img-Holder thumb' expr:href='data:post.url' expr:title='data:post.title'>
                    <span expr:class='&quot;postcat catnum&quot; + data:i' rel='tag'><data:post.labels.first.name/></span>
                    <b:if cond='data:post.thumbnailUrl'>
                      <img class='post-thumb' expr:alt='data:post.title' expr:data-src='resizeImage(data:post.thumbnailUrl, 1600)' expr:title='data:post.title' height='170' width='300'/>
                      <b:else/>
                      <span class='Noimger'/>
                    </b:if>
                  </a>

                  <div class='post-home cont'>
                    <div class='post-info'>
                      <span class='Date published updated'><svg><use href='#ic-clock'/></svg><a class='agotime' expr:datetime='data:post.lastUpdated.iso8601' expr:href='data:post.url'/></span>
                      <h2 class='rnav-title entry-title p-name'><a class='Title' expr:href='data:post.url' rel='bookmark'><data:post.title/></a></h2>
                    </div>
                    <div class='items'>
                      <b:if cond='data:post.author.profileUrl'>
                        <a class='author vcard' expr:href='data:post.author.profileUrl'>
                          <span class='fn'><data:post.author.name/></span></a>
                        <b:else/>
                        <span class='vcard'><span class='fn'><data:post.author.name/></span></span>
                      </b:if>
                    </div>
                    <div class='Short_content entry-content'><data:post.snippets.short/></div>
                    <a class='moreLink' expr:href='data:post.url' expr:title='data:post.title'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>read more<b:else/>اقرأ المزيد</b:if></a>
                  </div>
                </b:includable>
                <b:includable id='sp-navigation' var='post'>

                </b:includable>
                <b:includable id='sp-nextprev'>

                  <div class='loadMore'>
                      <a class='blog-pager-older-link hide' expr:href='data:olderPageUrl' title='NextUrl'/>
                      <div expr:data-index='data:numPosts' id='loadMorePosts'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>Show more <b:else/>تحميل المزيد من المشاركات</b:if></div>
                      <div id='loadMoreWait'><span class='spiner-icon'/> <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>Showing<b:else/>جاري التحميل ...</b:if></div>
                      <div id='loadMoreNomore'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>No More Posts<b:else/>لم يتم العثور على أي نتائج</b:if></div>
                    </div>

                </b:includable>
                <b:includable id='sp-postQuickEdit' var='post'>
                  <b:if cond='data:view.isPost'>
                    <!-- Quick Edit -->
                    <span expr:class='&quot;edit-post item-control &quot; + data:post.adminClass'>
                      <a expr:href='&quot;https://www.blogger.com/blog/post/edit/&quot; + data:blog.blogId + &quot;/&quot; + data:post.id' target='_blank'> <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>

                        <b:else/>

                        </b:if> </a>
                    </span></b:if>
                  <b:if cond='data:view.isPage'>
                    <!-- Quick Edit -->
                    <span expr:class='&quot;edit-post item-control &quot; + data:post.adminClass'>
                      <a expr:href='&quot;https://www.blogger.com/blog/page/edit/&quot; + data:blog.blogId + &quot;/&quot; + data:post.id' target='_blank'> <b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>

                        <b:else/>

                        </b:if> </a>
                    </span></b:if>
                </b:includable>
                <b:includable id='sp-postTags' var='post'>
                  <b:if cond='data:widgets.Blog.first.allBylineItems.labels and data:post.labels.any'>
                    <!-- Post Labels -->
                    <div class='post-tags'>
                      <span class='tagstitle'><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>Tags<b:else/>الأقسام</b:if></span>
                      <b:loop values='data:post.labels' var='label'>
                        <a expr:href='data:label.url' expr:title='data:label.name' rel='tag'><data:label.name/></a>
                      </b:loop>
                    </div>
                    <b:loop index='item' values='data:post.labels' var='label'>
                      <b:if cond='data:item lt 1'>
                        <script type='application/ld+json'>{
                          &quot;@context&quot;: &quot;http://schema.org&quot;,&quot;@type&quot;: &quot;BreadcrumbList&quot;,&quot;itemListElement&quot;: [{&quot;@type&quot;: &quot;ListItem&quot;,&quot;position&quot;: 1,&quot;item&quot;: {&quot;@id&quot;: &quot;<data:blog.homepageUrl.canonical/>&quot;,&quot;name&quot;: &quot;<data:blog.title/>&quot;}},{&quot;@type&quot;: &quot;ListItem&quot;,&quot;position&quot;: 2,&quot;item&quot;: {&quot;@id&quot;: &quot;<data:label.url.canonical/>&quot;,&quot;name&quot;: &quot;<data:label.name/>&quot;}},{&quot;@type&quot;: &quot;ListItem&quot;,&quot;position&quot;: 3,&quot;item&quot;: {&quot;@id&quot;: &quot;<data:post.url.canonical/>&quot;,&quot;name&quot;: &quot;<data:view.title.escaped/>&quot;}}]}</script>
                      </b:if>
                    </b:loop>
                  </b:if>
                </b:includable>
                <b:includable id='sp-sharePost' var='post'>

                  <b:if cond='data:widgets.Blog.first.allBylineItems.share and data:view.isPost'>
                    <div class='pSh'>
                      <div class='pShc' expr:data-text='data:messages.share + &quot; : &quot;'>
                        <!-- Share to Facebook -->
                        <a aria-label='Facebook' class='c fb' data-text='Share' expr:href='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:blog.url.canonical' rel='noopener' role='button' target='_blank'><svg class='n-line'><use href='#ic-facebook'/></svg></a>

                        <!-- Share to Whatsapp -->
                        <a aria-label='Whatsapp' class='c wa' data-text='Share' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:blog.url.canonical' rel='noopener' role='button' target='_blank'><svg class='n-line'><use href='#ic-whatsapp'/></svg></a>

                        <!-- Share to Twitter -->
                        <a aria-label='Twitter' class='c tw' data-text='Tweet' expr:href='&quot;https://twitter.com/share?url=&quot; + data:blog.url.canonical' rel='noopener' role='button' target='_blank'><svg class='n-line'><use href='#ic-twitter'/></svg></a>

                        <label class='sharemore' expr:aria-label='data:messages.shareToOtherApps' for='forShare'><svg class='n-line'><use href='#ic-share'/></svg></label>
                      </div>
                    </div>

                  </b:if>

                  <b:include cond='data:post.shareUrl and data:view.isPost and !data:view.isPreview' name='postInfoShareMore'/>

                </b:includable>
                <b:includable id='theme-custom-lang'>
                  <b:switch var='data:message'>
                    <b:case value='prevPost'/> <data:post.author.name/>
                  </b:switch>
                </b:includable>
                <b:includable id='threadedCommentForm' var='post'><div id='comments-respond'><div class='conart'><a class='go-respond ribble' href='#item-comments' id='comment-post-message'><data:messages.postAComment/></a><b:if cond='data:this.messages.blogComment != &quot;&quot;'><p><data:this.messages.blogComment/></p></b:if></div><a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=contempo&quot;' id='comment-editor-src' title='comment form link'/><iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' expr:data-src='data:post.commentFormIframeSrc + &quot;&amp;skin=contempo&quot;' frameborder='0' height='95px' id='comment-editor' name='comment-editor' title='comment form' width='100%'/><noscript>&lt;!--<data:post.cmtfpIframe/>--&gt;</noscript></div></b:includable>
                <b:includable id='threadedCommentJs' var='post'/>
                <b:includable id='threadedComments' var='post'><section class='comments threaded' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments-wrap'><b:if cond='data:post.allowNewComments'><div class='comment-footer'><b:include data='post' name='threadedCommentForm'/></div><b:else/><p class='c-not-allowed'><data:post.noNewCommentsText/></p></b:if><b:if cond='data:showCmtPopup'><p class='c-not-allowed'><data:post.noNewCommentsText/></p></b:if><div class='comments-content'><div class='comments-list' id='comment-holder'><ul/></div></div></section>
                </b:includable>
              </b:widget>
            </b:section>

            <b:section cond='data:view.isPost or data:view.isLayoutMode' id='PostA3lan' maxwidgets='1' showaddelement='no'>
              <b:widget id='HTML2' locked='true' title='اعلان اول المقال' type='HTML' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='content'/>
                </b:widget-settings>
                <b:includable id='main'>
                  <div class='myad-top SeoPlusAds'>
                    <data:content/>
                  </div>
                  <script>_$(&#39;#top-a3lan&#39;).prepend(_$(&#39;.myad-top&#39;));</script>
                </b:includable>
              </b:widget>
              <b:widget id='HTML3' locked='true' title='اعلان منتصف المقال' type='HTML' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='content'/>
                </b:widget-settings>
                <b:includable id='main'>
                  <div class='myad-cent SeoPlusAds'>
                    <data:content/>
                  </div>
                  <script>
                  

                  
                  var lenx = document.querySelectorAll(&#39;.post-body p&#39;);
                  var lenx2 = document.querySelectorAll(&#39;.post-body br&#39;);

                  if(lenx2.length){
                    lenx2[Math.floor(lenx2.length / 2)].after(_$(&#39;.myad-cent&#39;))
                  }else if(lenx.length){
                    lenx[Math.floor(lenx.length / 2)].after(_$(&#39;.myad-cent&#39;))
                  }

                  
                  </script>

                </b:includable>
              </b:widget>
              <b:widget id='HTML4' locked='true' title='اعلان اخر المقال' type='HTML' version='2' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='content'/>
                </b:widget-settings>
                <b:includable id='main'>
                  <div class='myad-bot SeoPlusAds'>
                    <data:content/>
                  </div>
                  <script>_$(&#39;#bot-a3lan&#39;).prepend(_$(&#39;.myad-bot&#39;));</script>
                </b:includable>
              </b:widget>
            </b:section>
            
            <b:if cond='!data:view.isLayoutMode'><b:if cond='data:view.isSingleItem'><b:include name='ArticaleSittings'/></b:if></b:if>


          </div>


            <b:if cond='!data:view.isError'>
              <aside class='potg btg2' id='sidepar-wid'>
                <b:section id='sidepar'>
                  <b:widget id='Label1' locked='false' title='التصنيفات' type='Label' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                      <b:widget-setting name='display'>LIST</b:widget-setting>
                      <b:widget-setting name='selectedLabelsList'/>
                      <b:widget-setting name='showType'>ALL</b:widget-setting>
                      <b:widget-setting name='showFreqNumbers'>true</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                    <b:includable id='cloud'>
  <b:loop values='data:labels' var='label'>
    <span class='label-size'>
      <b:class expr:name='&quot;label-size-&quot; + data:label.cssSize'/>
      <a class='label-name' expr:href='data:label.url'>
        <data:label.name/>
        <b:if cond='data:this.showFreqNumbers'>
          <span class='label-count'><data:label.count/></span>
        </b:if>
      </a>
    </span>
  </b:loop>
</b:includable>
                    <b:includable id='content'>
  <div class='widget-content'>
    <b:class expr:name='data:this.display + &quot;-label-widget-content&quot;'/>
    <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
    <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
  </div>
</b:includable>
                    <b:includable id='list'>
  <ul>
    <b:loop values='data:labels' var='label'>
      <li>
        <a class='label-name' expr:href='data:label.url'>
          <data:label.name/>
          <b:if cond='data:this.showFreqNumbers'>
            <span class='label-count'><data:label.count/></span>
          </b:if>
        </a>
      </li>
    </b:loop>
  </ul>
</b:includable>
                  </b:widget>
                  <b:widget id='HTML5' locked='false' title='اعلان' type='HTML' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-4294159533346602"
     crossorigin="anonymous"></script>
<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="fluid"
     data-ad-layout-key="-6g+ck-b-3y+i9"
     data-ad-client="ca-pub-4294159533346602"
     data-ad-slot="8707016258"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
  <b:include name='widget-title'/>
  <div class='widget-content'>
    <data:content/>
  </div>
</b:includable>
                  </b:widget>
                  <b:widget id='LinkList4' locked='true' title='تابعنا على' type='LinkList' version='2' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='text-1'>twitter</b:widget-setting>
                      <b:widget-setting name='link-1'><![CDATA[https://x.com/nornnna?t=y0uFGXR-XVdD4L_ndQ2Yzw&s=09]]></b:widget-setting>
                      <b:widget-setting name='text-0'>facebook</b:widget-setting>
                      <b:widget-setting name='link-2'>https://t.me/gazanewsps1</b:widget-setting>
                      <b:widget-setting name='link-0'><![CDATA[https://www.facebook.com/profile.php?id=61570650725890&mibextid=ZbWKwL]]></b:widget-setting>
                      <b:widget-setting name='text-2'>Telegram</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'><b:include name='widget-title'/><b:include name='content'/></b:includable>
                    <b:includable id='content'><ul class='social-static social'><b:loop values='data:links' var='link'><li><a expr:href='data:link.target' expr:title='data:link.name' rel='nofollow noopener' target='_blank'><svg><use expr:href='&quot;#ic-&quot; + data:link.name'/></svg></a></li></b:loop></ul></b:includable>
                  </b:widget>
                  <b:widget id='PopularPosts1' locked='false' title='' type='PopularPosts' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='numItemsToShow'>10</b:widget-setting>
                      <b:widget-setting name='showThumbnails'>true</b:widget-setting>
                      <b:widget-setting name='showSnippets'>true</b:widget-setting>
                      <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <div class='widget-content'>
    <b:include name='snippetedPosts'/>
  </div>
</b:includable>
                    <b:includable id='snippetedPostContent'>
          <b:if cond='data:postDisplay.showFeaturedImage'>
            <a class='item-thumbnail Img-Holder thumb' expr:href='data:post.url' expr:title='data:messages.image'>
              <b:if cond='data:post.featuredImage'>
                <b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><span class='postcat'><data:post.labels.first.name/></span></b:if>
                <img expr:alt='data:messages.image' expr:data-src='data:post.featuredImage' height='108' width='192'/>
                <b:else/>
                <span class='Noimger'/>
              </b:if>
            </a>
          </b:if>
          <b:if cond='data:postDisplay.showTitle'><h3 class='posts post-title'><span class='Date published updated'><svg><use href='#ic-clock'/></svg><a class='agotime' expr:datetime='data:post.lastUpdated.iso8601' expr:href='data:post.url'/></span><a class='title' expr:href='data:post.url'><data:post.title/></a></h3></b:if>
          <b:if cond='data:postDisplay.showSnippet'><p class='snippet-item'><b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><data:post.snippets.short/></b:if></p>
          </b:if>
        </b:includable>
                    <b:includable id='snippetedPosts'>
          <div expr:class='(data:postDisplay.showFeaturedImage ? &quot;ImgShow&quot; : &quot;Noimg&quot;)' role='feed'>
            <b:loop index='i' values='data:posts filter (p =&gt; p.id != data:view.postId)' var='post'>
              <article class='post' role='article'>
                <b:include name='snippetedPostContent'/>
              </article>
            </b:loop>
          </div>
        </b:includable>
                  </b:widget>
                  <b:widget id='ContactForm1' locked='false' title='نموذج الاتصال' type='ContactForm' visible='true'>
                    <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                    <b:includable id='content'>
          <div class='contact-form-widget'>
            <div class='form'>
              <form name='contact-form'>

                <input class='contact-form-name' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/>
                <br/>
                <input class='contact-form-email' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg' name='email' size='30' type='text' value=''/>
                <br/>

                <textarea class='contact-form-email-message' cols='25' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg' name='email-message' rows='5'/>
                <br/>
                <input class='contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/>
                <div style='width: calc(100% - 80px);display: flex;float: left;height: 30px;align-items: center;'>
                  <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
                  <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
                </div>
              </form>
            </div>
          </div>
        </b:includable>
                  </b:widget>
                </b:section>
              </aside>
            </b:if>
        </div>

        <div class='EndSides'/>

      </div>


      <footer>
        <div class='container'>

          <div class='mid-top-footer'>
            <b:section class='footer-col' id='footer-col1'>
              <b:widget id='Followers1' locked='false' title='تابع هنا' type='Followers' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='borderColorTransparent'>true</b:widget-setting>
                  <b:widget-setting name='useTemplateDefaultStyles'>true</b:widget-setting>
                  <b:widget-setting name='contentSecondaryTextColor'>#000000</b:widget-setting>
                  <b:widget-setting name='contentHeadlineColor'>#000000</b:widget-setting>
                  <b:widget-setting name='endcapTextColor'>#666666</b:widget-setting>
                  <b:widget-setting name='contentTextColor'>#666666</b:widget-setting>
                  <b:widget-setting name='contentSecondaryLinkColor'>#444444</b:widget-setting>
                  <b:widget-setting name='endcapLinkColor'>#444444</b:widget-setting>
                  <b:widget-setting name='contentLinkColor'>#444444</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main'>
  <b:if cond='data:title != &quot;&quot; and data:codeSnippet != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <div class='widget-content'>
    <div expr:id='data:widget.instanceId + &quot;-wrapper&quot;'>
      <b:if cond='data:codeSnippet != &quot;&quot;'>
        <div style='margin-right:2px;'>
          <data:codeSnippet/>
        </div>
      </b:if>
    </div>
    <b:include name='quickedit'/>
  </div>
</b:includable>
              </b:widget>
            </b:section>
            <b:section class='footer-col' id='footer-col2'>
              <b:widget id='FeaturedPost1' locked='false' title='مشاركة مميزة' type='FeaturedPost' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='showSnippet'>true</b:widget-setting>
                  <b:widget-setting name='showPostTitle'>true</b:widget-setting>
                  <b:widget-setting name='postId'>0</b:widget-setting>
                  <b:widget-setting name='showFirstImage'>true</b:widget-setting>
                  <b:widget-setting name='useMostRecentPost'>true</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <div class='widget-content'>
    <b:include name='snippetedPosts'/>
  </div>
</b:includable>
                <b:includable id='snippetedPostContent'>
          <b:if cond='data:postDisplay.showFeaturedImage'>
            <a class='item-thumbnail Img-Holder thumb' expr:href='data:post.url' expr:title='data:messages.image'>
              <b:if cond='data:post.featuredImage'>
                <b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><span class='postcat'><data:post.labels.first.name/></span></b:if>
                <img expr:alt='data:messages.image' expr:data-src='data:post.featuredImage' height='108' width='192'/>
                <b:else/>
                <span class='Noimger'/>
              </b:if>
            </a>
          </b:if>
          <b:if cond='data:postDisplay.showTitle'><h3 class='posts post-title'><span class='Date published updated'><svg><use href='#ic-clock'/></svg><a class='agotime' expr:datetime='data:post.lastUpdated.iso8601' expr:href='data:post.url'/></span><a class='title' expr:href='data:post.url'><data:post.title/></a></h3></b:if>
          <b:if cond='data:postDisplay.showSnippet'><p class='snippet-item'><b:if cond='data:widget.type == &quot;FeaturedPost&quot;'><data:post.snippets.short/></b:if></p>
          </b:if>
        </b:includable>
                <b:includable id='snippetedPosts'>
          <div expr:class='(data:postDisplay.showFeaturedImage ? &quot;ImgShow&quot; : &quot;Noimg&quot;)' role='feed'>
            <b:loop index='i' values='data:posts filter (p =&gt; p.id != data:view.postId)' var='post'>
              <article class='post' role='article'>
                <b:include name='snippetedPostContent'/>
              </article>
            </b:loop>
          </div>
        </b:includable>
              </b:widget>
            </b:section>
            <b:section class='footer-col' id='footer-col3'/>
            <b:section class='footer-col' id='footer-col4'/>
          </div>
        </div>
        <div class='bottom-footer'>
          <div class='container'>
            <div class='yemen'>
              <span><b:if cond='data:blog.languageDirection == &quot;ltr&quot;'>
                all rights are save
                <b:else/>
                جميع الحقوق محفوظة
                </b:if> &#169;</span><a expr:href='data:blog.homepageUrl' id='7qok' target='_blank'><data:blog.title/></a>
            </div>
            <div class='shmal'>
              <b:section id='footer-social' maxwidgets='1' showaddelement='no'>
                <b:widget id='LinkList2' locked='true' title='مواقع التواصل الإجتماعي' type='LinkList' version='2' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='sorting'>NONE</b:widget-setting>
                    <b:widget-setting name='text-1'>facebook</b:widget-setting>
                    <b:widget-setting name='link-1'><![CDATA[https://www.facebook.com/profile.php?id=61570650725890&mibextid=ZbWKwL]]></b:widget-setting>
                    <b:widget-setting name='text-0'>twitter</b:widget-setting>
                    <b:widget-setting name='link-0'><![CDATA[https://x.com/nornnna?t=y0uFGXR-XVdD4L_ndQ2Yzw&s=09]]></b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'><b:include name='content'/></b:includable>
                  <b:includable id='content'><ul class='social-static social'><b:loop values='data:links' var='link'><li><a expr:href='data:link.target' expr:title='data:link.name' rel='nofollow noopener' target='_blank'><svg><use expr:href='&quot;#ic-&quot; + data:link.name'/></svg></a></li></b:loop></ul></b:includable>
                </b:widget>
              </b:section>
            </div>
          </div>
        </div>
      </footer>


      <div class='toTopB' id='backTop' onclick='window.scrollTo({top: 0});'><b:include name='arrow-up-circle-icon'/></div>


      <b:if cond='data:view.isSingleItem'><div id='ReadPage'/></b:if>
      </div>




    <b:include name='themeFunctions'/>

    <svg class='hide'>
      <b:include name='themeIcons'/>
    </svg>


    &lt;noscript id=&#39;blogger-components&#39;&gt;</body>&lt;/noscript&gt;&lt;/body&gt;
</html>
