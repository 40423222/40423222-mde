# 40423222-mde

<!DOCTYPE html>
<html lang="en"
>
<head>
    <title>Kmolab (虎尾科大MDE)</title>
    <!-- Using the latest rendering mode for IE -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">




<style type="text/css">

/*some stuff for output/input prompts*/
div.cell{border:1px solid transparent;display:-webkit-box;-webkit-box-orient:vertical;-webkit-box-align:stretch;display:-moz-box;-moz-box-orient:vertical;-moz-box-align:stretch;display:box;box-orient:vertical;box-align:stretch;display:flex;flex-direction:column;align-items:stretch}div.cell.selected{border-radius:4px;border:thin #ababab solid}
div.cell.edit_mode{border-radius:4px;border:thin #008000 solid}
div.cell{width:100%;padding:5px 5px 5px 0;margin:0;outline:none}
div.prompt{min-width:11ex;padding:.4em;margin:0;font-family:monospace;text-align:right;line-height:1.21429em}
@media (max-width:480px){div.prompt{text-align:left}}div.inner_cell{display:-webkit-box;-webkit-box-orient:vertical;-webkit-box-align:stretch;display:-moz-box;-moz-box-orient:vertical;-moz-box-align:stretch;display:box;box-orient:vertical;box-align:stretch;display:flex;flex-direction:column;align-items:stretch;-webkit-box-flex:1;-moz-box-flex:1;box-flex:1;flex:1}
div.input_area{border:1px solid #cfcfcf;border-radius:4px;background:#f7f7f7;line-height:1.21429em}
div.prompt:empty{padding-top:0;padding-bottom:0}
div.input{page-break-inside:avoid;display:-webkit-box;-webkit-box-orient:horizontal;-webkit-box-align:stretch;display:-moz-box;-moz-box-orient:horizontal;-moz-box-align:stretch;display:box;box-orient:horizontal;box-align:stretch;}
div.inner_cell{width:90%;}
div.input_area{border:1px solid #cfcfcf;border-radius:4px;background:#f7f7f7;}
div.input_prompt{color:navy;border-top:1px solid transparent;}
div.output_wrapper{margin-top:5px;position:relative;display:-webkit-box;-webkit-box-orient:vertical;-webkit-box-align:stretch;display:-moz-box;-moz-box-orient:vertical;-moz-box-align:stretch;display:box;box-orient:vertical;box-align:stretch;width:100%;}
div.output_scroll{height:24em;width:100%;overflow:auto;border-radius:4px;-webkit-box-shadow:inset 0 2px 8px rgba(0, 0, 0, 0.8);-moz-box-shadow:inset 0 2px 8px rgba(0, 0, 0, 0.8);box-shadow:inset 0 2px 8px rgba(0, 0, 0, 0.8);}
div.output_collapsed{margin:0px;padding:0px;display:-webkit-box;-webkit-box-orient:vertical;-webkit-box-align:stretch;display:-moz-box;-moz-box-orient:vertical;-moz-box-align:stretch;display:box;box-orient:vertical;box-align:stretch;width:100%;}
div.out_prompt_overlay{height:100%;padding:0px 0.4em;position:absolute;border-radius:4px;}
div.out_prompt_overlay:hover{-webkit-box-shadow:inset 0 0 1px #000000;-moz-box-shadow:inset 0 0 1px #000000;box-shadow:inset 0 0 1px #000000;background:rgba(240, 240, 240, 0.5);}
div.output_prompt{color:darkred;}

a.anchor-link:link{text-decoration:none;padding:0px 20px;visibility:hidden;}
h1:hover .anchor-link,h2:hover .anchor-link,h3:hover .anchor-link,h4:hover .anchor-link,h5:hover .anchor-link,h6:hover .anchor-link{visibility:visible;}
/* end stuff for output/input prompts*/


.highlight-ipynb .hll { background-color: #ffffcc }
.highlight-ipynb  { background: #f8f8f8; }
.highlight-ipynb .c { color: #408080; font-style: italic } /* Comment */
.highlight-ipynb .err { border: 1px solid #FF0000 } /* Error */
.highlight-ipynb .k { color: #008000; font-weight: bold } /* Keyword */
.highlight-ipynb .o { color: #666666 } /* Operator */
.highlight-ipynb .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight-ipynb .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight-ipynb .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight-ipynb .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight-ipynb .gd { color: #A00000 } /* Generic.Deleted */
.highlight-ipynb .ge { font-style: italic } /* Generic.Emph */
.highlight-ipynb .gr { color: #FF0000 } /* Generic.Error */
.highlight-ipynb .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight-ipynb .gi { color: #00A000 } /* Generic.Inserted */
.highlight-ipynb .go { color: #888888 } /* Generic.Output */
.highlight-ipynb .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight-ipynb .gs { font-weight: bold } /* Generic.Strong */
.highlight-ipynb .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight-ipynb .gt { color: #0044DD } /* Generic.Traceback */
.highlight-ipynb .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight-ipynb .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight-ipynb .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight-ipynb .kp { color: #008000 } /* Keyword.Pseudo */
.highlight-ipynb .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight-ipynb .kt { color: #B00040 } /* Keyword.Type */
.highlight-ipynb .m { color: #666666 } /* Literal.Number */
.highlight-ipynb .s { color: #BA2121 } /* Literal.String */
.highlight-ipynb .na { color: #7D9029 } /* Name.Attribute */
.highlight-ipynb .nb { color: #008000 } /* Name.Builtin */
.highlight-ipynb .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight-ipynb .no { color: #880000 } /* Name.Constant */
.highlight-ipynb .nd { color: #AA22FF } /* Name.Decorator */
.highlight-ipynb .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight-ipynb .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight-ipynb .nf { color: #0000FF } /* Name.Function */
.highlight-ipynb .nl { color: #A0A000 } /* Name.Label */
.highlight-ipynb .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight-ipynb .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight-ipynb .nv { color: #19177C } /* Name.Variable */
.highlight-ipynb .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight-ipynb .w { color: #bbbbbb } /* Text.Whitespace */
.highlight-ipynb .mf { color: #666666 } /* Literal.Number.Float */
.highlight-ipynb .mh { color: #666666 } /* Literal.Number.Hex */
.highlight-ipynb .mi { color: #666666 } /* Literal.Number.Integer */
.highlight-ipynb .mo { color: #666666 } /* Literal.Number.Oct */
.highlight-ipynb .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight-ipynb .sc { color: #BA2121 } /* Literal.String.Char */
.highlight-ipynb .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight-ipynb .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight-ipynb .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight-ipynb .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight-ipynb .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight-ipynb .sx { color: #008000 } /* Literal.String.Other */
.highlight-ipynb .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight-ipynb .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight-ipynb .ss { color: #19177C } /* Literal.String.Symbol */
.highlight-ipynb .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight-ipynb .vc { color: #19177C } /* Name.Variable.Class */
.highlight-ipynb .vg { color: #19177C } /* Name.Variable.Global */
.highlight-ipynb .vi { color: #19177C } /* Name.Variable.Instance */
.highlight-ipynb .il { color: #666666 } /* Literal.Number.Integer.Long */
</style>

<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
div.entry-content {
  overflow: visible;
  padding: 8px;
}
.input_area {
  padding: 0.2em;
}

a.heading-anchor {
 white-space: normal;
}

.rendered_html
code {
 font-size: .8em;
}

pre.ipynb {
  color: black;
  background: #f7f7f7;
  border: none;
  box-shadow: none;
  margin-bottom: 0;
  padding: 0;
  margin: 0px;
  font-size: 13px;
}

/* remove the prompt div from text cells */
div.text_cell .prompt {
    display: none;
}

/* remove horizontal padding from text cells, */
/* so it aligns with outer body text */
div.text_cell_render {
    padding: 0.5em 0em;
}

img.anim_icon{padding:0; border:0; vertical-align:middle; -webkit-box-shadow:none; -box-shadow:none}
</style>

<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML" type="text/javascript"></script>
<script type="text/javascript">
init_mathjax = function() {
    if (window.MathJax) {
        // MathJax loaded
        MathJax.Hub.Config({
            tex2jax: {
                inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                displayMath: [ ['$$','$$'], ["\\[","\\]"] ]
            },
            displayAlign: 'left', // Change this to 'center' to center equations.
            "HTML-CSS": {
                styles: {'.MathJax_Display': {"margin": 0}}
            }
        });
        MathJax.Hub.Queue(["Typeset",MathJax.Hub]);
    }
}
init_mathjax();
</script>

<link rel="canonical" href="http://chiamingyen.github.io/kmolab/blog">
        <meta name="author" content="kmol" />

    <!-- Open Graph tags -->
        <meta property="og:site_name" content="Kmolab (虎尾科大MDE)" />
        <meta property="og:type" content="website"/>
        <meta property="og:title" content="Kmolab (虎尾科大MDE)"/>
        <meta property="og:url" content="http://chiamingyen.github.io/kmolab/blog"/>
        <meta property="og:description" content="Kmolab (虎尾科大MDE)"/>


    <!-- Bootstrap -->
        <link rel="stylesheet" href="http://chiamingyen.github.io/kmolab/blog/theme/css/bootstrap.united.min.css" type="text/css"/>
    <link href="http://chiamingyen.github.io/kmolab/blog/theme/css/font-awesome.min.css" rel="stylesheet">

    <link href="http://chiamingyen.github.io/kmolab/blog/theme/css/pygments/monokai.css" rel="stylesheet">
    <link href="http://chiamingyen.github.io/kmolab/blog/theme/tipuesearch/tipuesearch.css" rel="stylesheet">
    <link rel="stylesheet" href="http://chiamingyen.github.io/kmolab/blog/theme/css/style.css" type="text/css"/>

        <link href="http://chiamingyen.github.io/kmolab/blog/feeds/all.atom.xml" type="application/atom+xml" rel="alternate"
              title="Kmolab (虎尾科大MDE) ATOM Feed"/>

<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shCore.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushJScript.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushJava.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushPython.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushSql.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushXml.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushPhp.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushCpp.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushCss.js"></script>
<script type="text/javascript" src="http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/shBrushCSharp.js"></script>
<script type='text/javascript'>
	(function(){
		var corecss = document.createElement('link');
		var themecss = document.createElement('link');
		var corecssurl = "http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/css/shCore.css";
		if ( corecss.setAttribute ) {
				corecss.setAttribute( "rel", "stylesheet" );
				corecss.setAttribute( "type", "text/css" );
				corecss.setAttribute( "href", corecssurl );
		} else {
				corecss.rel = "stylesheet";
				corecss.href = corecssurl;
		}
		document.getElementsByTagName("head")[0].insertBefore( corecss, document.getElementById("syntaxhighlighteranchor") );
		var themecssurl = "http://chiamingyen.github.io/kmolab_data/files/syntaxhighlighter/css/shThemeDefault.css?ver=3.0.9b";
		if ( themecss.setAttribute ) {
				themecss.setAttribute( "rel", "stylesheet" );
				themecss.setAttribute( "type", "text/css" );
				themecss.setAttribute( "href", themecssurl );
		} else {
				themecss.rel = "stylesheet";
				themecss.href = themecssurl;
		}
		//document.getElementById("syntaxhighlighteranchor").appendChild(themecss);
		document.getElementsByTagName("head")[0].insertBefore( themecss, document.getElementById("syntaxhighlighteranchor") );
	})();
	SyntaxHighlighter.config.strings.expandSource = '+ expand source';
	SyntaxHighlighter.config.strings.help = '?';
	SyntaxHighlighter.config.strings.alert = 'SyntaxHighlighter\n\n';
	SyntaxHighlighter.config.strings.noBrush = 'Can\'t find brush for: ';
	SyntaxHighlighter.config.strings.brushNotHtmlScript = 'Brush wasn\'t configured for html-script option: ';
	SyntaxHighlighter.defaults['pad-line-numbers'] = false;
	SyntaxHighlighter.defaults['toolbar'] = false;
	SyntaxHighlighter.all();
</script>

</head>
<body>

<div class="navbar navbar-default navbar-fixed-top" role="navigation">
	<div class="container">
        <div class="navbar-header">
            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-ex1-collapse">
                <span class="sr-only">Toggle navigation</span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
            </button>
            <a href="http://chiamingyen.github.io/kmolab/blog/" class="navbar-brand">
Kmolab (虎尾科大MDE)            </a>
        </div>
        <div class="collapse navbar-collapse navbar-ex1-collapse">
            <ul class="nav navbar-nav">
                         <li><a href="http://chiamingyen.github.io/kmolab/blog/pages/about/">
                             About
                          </a></li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/alumni.html">Alumni</a>
                        </li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/cadlab.html">Cadlab</a>
                        </li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/courses.html">Courses</a>
                        </li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/project.html">Project</a>
                        </li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/python.html">Python</a>
                        </li>
                        <li >
                            <a href="http://chiamingyen.github.io/kmolab/blog/category/ubuntu.html">Ubuntu</a>
                        </li>
            </ul>
            <ul class="nav navbar-nav navbar-right">
              <li><span>
                <form class="navbar-search" action="http://chiamingyen.github.io/kmolab/blog/search.html">
                  <input type="text" class="search-query" placeholder="Search" name="q" id="tipue_search_input" required>
                </form></span>
              </li>
              <li><a href="http://chiamingyen.github.io/kmolab/blog/archives.html"><i class="fa fa-th-list"></i><span class="icon-label">Archives</span></a></li>
            </ul>
        </div>
        <!-- /.navbar-collapse -->
    </div>
</div> <!-- /.navbar -->
<!-- Banner -->
<!-- End Banner -->
<div class="container">
    <div class="row">
        <div class="col-sm-9">

            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/git-shi-yong-dao-yin.html">Git 使用導引</a></h2>
                <div class="summary"><p>Git 是一套分散式數位資料版本控制系統, 而學習 Git 最好的參考資料就是 <a href="https://git-scm.com/book/zh-tw/v2"> Pro Git</a> (<a href="https://git-scm.com/book/zh-tw/v1">第1版</a>).</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/git-shi-yong-dao-yin.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/ji-suan-ji-cheng-shi-er.html">計算機程式 (二)</a></h2>
                <div class="summary"><p>2016Fall 的計算機程式課程已經從 Github 的應用開始, 先讓學員利用 Git 分散式管理工具進行團隊間的數位資料管理, 然後再以線上的分組程式為例, 說明運用計算機程式, 如何將原本繁雜的資料排序流程, 導向能隨需求而快速因應變化的網際程式流程.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/ji-suan-ji-cheng-shi-er.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-er.html">電腦輔助設計實習 (二)</a></h2>
                <div class="summary"><p>電腦輔助設計實習課程主要利用 Github 網際分散式數位檔案版次管理系統, 讓學員可以利用 Git 工具進行近端與遠端電腦輔助設計檔案的管理.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-er.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-cao-zuo-liu-cheng-lu-ying-gong-ju.html">電腦操作流程錄影工具</a></h2>
                <div class="summary"><p>製作多媒體影音檔案是機械設計工程師在產品設計開發過程中六種表達中的重要技能之一, 因為其中融合口語表達、文字表達、2D 圖像表達與(3D) 動態資料表達、解析模型表達與實體原型表達等內容, 在 2016Fall 的<a href="https://github.com/mdecourse/2016fallcp">計算機程式</a>與<a href="https://github.com/mdecourse/2016fallcadp">電腦輔助設計實習</a>課程中, 我們將採用 <a href="https://github.com/ShareX/ShareX">ShareX</a> (建議<a href="https://github.com/ShareX/ShareX/releases">下載 ShareX portable 版本</a>) 與 <a href="https://github.com/aaae/kazam">Kazam</a> 等兩套用來錄製多媒體影片的工具, 其中 <a href="https://github.com/ShareX/ShareX">ShareX</a> 以 C# 編寫, 適用於 Windows, 而 <a href="https://github.com/aaae/kazam">Kazam</a> 則採用 Python3 編寫, 可用於 Ubuntu 操作系統環境中的螢幕操作錄影.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/dian-nao-cao-zuo-liu-cheng-lu-ying-gong-ju.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-yi.html">電腦輔助設計實習 (一)</a></h2>
                <div class="summary"><p>2016FallCADP 課程倉儲: <a href="https://github.com/mdecourse/2016fallcadp">https://github.com/mdecourse/2016fallcadp</a></p>
<p>2016FallCADP 上課筆記: <a href="https://github.com/mdecourse/2016fallcadp/wiki">https://github.com/mdecourse/2016fallcadp/wiki</a></p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-yi.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/ji-suan-ji-cheng-shi-yi.html">計算機程式 (一)</a></h2>
                <div class="summary"><p>2016FallCP 課程倉儲: <a href="https://github.com/mdecourse/2016fallcp">https://github.com/mdecourse/2016fallcp</a></p>
<p>2016FallCP 上課筆記: <a href="https://github.com/mdecourse/2016fallcp/wiki">https://github.com/mdecourse/2016fallcp/wiki</a></p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/ji-suan-ji-cheng-shi-yi.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/xie-tong-chan-pin-she-ji-shi-xi-xi-lie-ke-cheng.html">協同產品設計實習系列課程</a></h2>
                <div class="summary"><p>二十一世紀的科技發展, 拜網路普及與數位運算能力大幅提升之賜, 使得集合在不同地理位置與時區上的工程師, 執行同步或非同步協同產品開發專案的模式, 已然成為常態.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/xie-tong-chan-pin-she-ji-shi-xi-xi-lie-ke-cheng.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/wang-ji-3d-zheng-chi-lun-chuan-dong-mo-ni-yi.html">網際 3D 正齒輪傳動模擬 (一)</a></h2>
                <div class="summary"><p>Onshape 的正齒輪設計繪圖與組立, 其基本原理與先前的 2D 網際繪圖類似, 只不過在以下的 3D 正齒輪傳動組立過程, 只有 Spur Gear 功能採用 Featurescript 編寫, 雖然在 Onshape Part Studio 中, 所有的零件可以透過統一的設計變數進行控管, 但若一旦設計流程的變化超出原先 Featurescript 的表單設定範圍 (例如: SG Featurescript 中的 Offset angle 只允許 0-360 的正值角度輸入), 設計者就必須介入調整不符合表單設計的 error.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/wang-ji-3d-zheng-chi-lun-chuan-dong-mo-ni-yi.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/wang-ji-2d-zheng-chi-lun-xie-tong-hui-tu-gui-hua.html">網際 2D 正齒輪協同繪圖規劃</a></h2>
                <div class="summary"><p>利用 Python 物件導向架構執行網際 2D 正齒輪傳動協同繪圖時, 各組員可以將各種不同繪圖元件, 建置在個人的網頁空間中, 讓其他參與協同的組員連結應用. 唯一必須注意的是, 就網際繪圖模式而言, 儘管 Brython 繪圖最終仍轉為 JavaScript, 以 Canvas 或 WebGL 完成繪圖, 但是 Python 程式碼在各自的 script 標註中屬於各自的命名空間 (此點與 Prototype based 的 JavaScript 有很大的差別), 因此以下的範例, 必須將各自在引用的 script 標註中, 以 id 命名, 然後根據 id 名稱, 在其他命名空間中以 import 引用.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/wang-ji-2d-zheng-chi-lun-xie-tong-hui-tu-gui-hua.html">more ...</a>
                </div>
            </article>
            <hr/>
            <article>
                <h2><a href="http://chiamingyen.github.io/kmolab/blog/wang-ji-3d-zheng-chi-lun-chuan-dong-mo-ni.html">網際 3D 正齒輪傳動模擬</a></h2>
                <div class="summary"><p>Onshape 終於正式公開 <a href="https://www.onshape.com/featurescript">FeatureScript</a> 以及所有內建特徵功能的<a href="https://cad.onshape.com/documents/5749364ce4b0f60f1b7940fe/w/925a5467b6e725168eb9c993/e/ff3b765aacc32576f893ed23">原始碼</a>, 並且同時追加了許多新的功能, 包括機構的動態模擬.</p>

                    <a class="btn btn-default btn-xs" href="http://chiamingyen.github.io/kmolab/blog/wang-ji-3d-zheng-chi-lun-chuan-dong-mo-ni.html">more ...</a>
                </div>
            </article>
            <hr/>

        <ul class="pagination">
                <li class="prev disabled"><a href="#">&laquo;</a></li>
                    <li class="active"><a
                            href="http://chiamingyen.github.io/kmolab/blog/index.html">1</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index2.html">2</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index3.html">3</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index4.html">4</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index5.html">5</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index6.html">6</a></li>
                    <li class=""><a
                            href="http://chiamingyen.github.io/kmolab/blog/index7.html">7</a></li>
                <li class="next"><a
                        href="http://chiamingyen.github.io/kmolab/blog/index2.html">&raquo;</a></li>
        </ul>
        </div>
        <div class="col-sm-3" id="sidebar">
            <aside>

<section class="well well-sm">
    <ul class="list-group list-group-flush">

            <li class="list-group-item"><h4><i class="fa fa-home fa-lg"></i><span class="icon-label">Recent Posts</span></h4>
                <ul class="list-group" id="recentposts">
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/git-shi-yong-dao-yin.html">
                            Git 使用導引
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/ji-suan-ji-cheng-shi-er.html">
                            計算機程式 (二)
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-er.html">
                            電腦輔助設計實習 (二)
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-cao-zuo-liu-cheng-lu-ying-gong-ju.html">
                            電腦操作流程錄影工具
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/dian-nao-fu-zhu-she-ji-shi-xi-yi.html">
                            電腦輔助設計實習 (一)
                        </a>
                    </li>
                </ul>
            </li>

            <li class="list-group-item"><a href="http://chiamingyen.github.io/kmolab/blog/categories.html"><h4><i class="fa fa-home fa-lg"></i><span class="icon-label">Categories</span></h4></a>
                <ul class="list-group" id="categories">
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/alumni.html">
                            <i class="fa fa-folder-open fa-lg"></i> Alumni
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/cadlab.html">
                            <i class="fa fa-folder-open fa-lg"></i> cadlab
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/courses.html">
                            <i class="fa fa-folder-open fa-lg"></i> Courses
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/project.html">
                            <i class="fa fa-folder-open fa-lg"></i> Project
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/python.html">
                            <i class="fa fa-folder-open fa-lg"></i> Python
                        </a>
                    </li>
                    <li class="list-group-item">
                        <a href="http://chiamingyen.github.io/kmolab/blog/category/ubuntu.html">
                            <i class="fa fa-folder-open fa-lg"></i> Ubuntu
                        </a>
                    </li>
                </ul>
            </li>

            <li class="list-group-item"><a href="http://chiamingyen.github.io/kmolab/blog/tags.html"><h4><i class="fa fa-tags fa-lg"></i><span class="icon-label">Tags</span></h4></a>
                <ul class="list-group list-inline tagcloud" id="tags">
                </ul>
            </li>
    <li class="list-group-item"><h4><i class="fa fa-external-link-square fa-lg"></i><span class="icon-label">Links</span></h4>
      <ul class="list-group" id="links">
        <li class="list-group-item">
            <a href="http://getpelican.com/" target="_blank">
                Pelican
            </a>
        </li>
        <li class="list-group-item">
            <a href="https://github.com/DandyDev/pelican-bootstrap3/" target="_blank">
                pelican-bootstrap3
            </a>
        </li>
        <li class="list-group-item">
            <a href="https://github.com/getpelican/pelican-plugins" target="_blank">
                pelican-plugins
            </a>
        </li>
        <li class="list-group-item">
            <a href="https://github.com/Tipue/Tipue-Search" target="_blank">
                Tipue search
            </a>
        </li>
      </ul>
    </li>
    </ul>
</section>
            </aside>
        </div>
    </div>
</div>
<footer>
   <div class="container">
      <hr>
      <div class="row">
         <div class="col-xs-10">&copy; 2016 kmol
            &middot; Powered by <a href="https://github.com/DandyDev/pelican-bootstrap3" target="_blank">pelican-bootstrap3</a>,
            <a href="http://docs.getpelican.com/" target="_blank">Pelican</a>,
            <a href="http://getbootstrap.com" target="_blank">Bootstrap</a>         </div>
         <div class="col-xs-2"><p class="pull-right"><i class="fa fa-arrow-up"></i> <a href="#">Back to top</a></p></div>
      </div>
   </div>
</footer>
<script src="http://chiamingyen.github.io/kmolab/blog/theme/js/jquery.min.js"></script>

<!-- Include all compiled plugins (below), or include individual files as needed -->
<script src="http://chiamingyen.github.io/kmolab/blog/theme/js/bootstrap.min.js"></script>

<!-- Enable responsive features in IE8 with Respond.js (https://github.com/scottjehl/Respond) -->
<script src="http://chiamingyen.github.io/kmolab/blog/theme/js/respond.min.js"></script>

    <!-- Disqus -->
    <script type="text/javascript">
        /* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
        var disqus_shortname = 'kmolab'; // required: replace example with your forum shortname

        /* * * DON'T EDIT BELOW THIS LINE * * */
        (function () {
            var s = document.createElement('script');
            s.async = true;
            s.type = 'text/javascript';
            s.src = '//' + disqus_shortname + '.disqus.com/count.js';
            (document.getElementsByTagName('HEAD')[0] || document.getElementsByTagName('BODY')[0]).appendChild(s);
        }());
    </script>
    <!-- End Disqus Code -->

</body>
</html>
