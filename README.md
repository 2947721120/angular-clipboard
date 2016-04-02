##CN 机器翻译，请参照EN下面原版理解
<article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-angular-clipboard" class="anchor" href="#angular-clipboard" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="angular-clipboard" data-dst="角剪贴板">角剪贴板</trans></h1>

<p><a href="https://travis-ci.org/omichelsen/angular-clipboard"><img src="https://camo.githubusercontent.com/643f14fd849a944851e17e5b9e5ae10773826239/68747470733a2f2f696d672e736869656c64732e696f2f7472617669732f6f6d696368656c73656e2f616e67756c61722d636c6970626f6172642f6d61737465722e737667" alt="Build Status" data-canonical-src="https://img.shields.io/travis/omichelsen/angular-clipboard/master.svg" style="max-width:100%;"></a>
<a href="https://coveralls.io/r/omichelsen/angular-clipboard?branch=master"><img src="https://camo.githubusercontent.com/e7eaf6252c64a16ff3f2d26bb26d764956259f84/68747470733a2f2f696d672e736869656c64732e696f2f636f766572616c6c732f6f6d696368656c73656e2f616e67756c61722d636c6970626f6172642f6d61737465722e737667" alt="Test Coverage" data-canonical-src="https://img.shields.io/coveralls/omichelsen/angular-clipboard/master.svg" style="max-width:100%;"></a></p>

<p><trans data-src="Copy text to clipboard by clicking a button, without using Flash. This is using the new " data-dst="通过点击一个按钮，剪贴板复制文本，而无需使用闪光灯。这是使用新的">通过点击一个按钮，剪贴板复制文本，而无需使用闪光灯。这是使用新的</trans><a href="https://developer.mozilla.org/en-US/docs/Web/API/Selection"><trans data-src="Selection API" data-dst="选择API">选择API</trans></a><trans data-src=" and " data-dst="和">和</trans><a href="https://developer.mozilla.org/en-US/docs/Web/API/ClipboardEvent"><trans data-src="Clipboard API" data-dst="剪贴板API">剪贴板API</trans></a><trans data-src=" available in the latest browsers." data-dst="在最新的浏览器可用。">在最新的浏览器可用。</trans></p>

<p><trans data-src="Browser support: Chrome 43+, Firefox 41+, Opera 29+ and IE10+." data-dst="浏览器支持：Chrome 43，Firefox 41，Opera 29和IE10。">浏览器支持：Chrome 43，Firefox 41，Opera 29和IE10。</trans></p>

<p><trans data-src="See the " data-dst="看到">看到</trans><a href="https://rawgit.com/omichelsen/angular-clipboard/master/demo/demo.html"><trans data-src="demo" data-dst="演示">演示</trans></a><trans data-src="." data-dst="。">。</trans></p>

<h2><a id="user-content-install" class="anchor" href="#install" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="Install" data-dst="安装">安装</trans></h2>

<p><trans data-src="Install using " data-dst="安装使用">安装使用</trans><code><trans data-src="npm" data-dst="新公共管理">新公共管理</trans></code><trans data-src=" or " data-dst="或">或</trans><code><trans data-src="bower" data-dst="鲍尔">鲍尔</trans></code><trans data-src=":" data-dst="：">：</trans></p>

<div class="highlight highlight-source-shell"><pre><trans data-src="$ npm install angular-clipboard --save" data-dst="NPM安装角剪贴板--拯救美元">NPM安装角剪贴板--拯救美元</trans></pre></div>

<div class="highlight highlight-source-shell"><pre><trans data-src="$ bower install angular-clipboard --save" data-dst="鲍尔安装角剪贴板--拯救美元">鲍尔安装角剪贴板--拯救美元</trans></pre></div>

<p><trans data-src="angular-clipboard has no other dependencies than " data-dst="角板没有其他依赖于">角板没有其他依赖于</trans><a href="https://angularjs.org/"><trans data-src="Angular" data-dst="角">角</trans></a><trans data-src="
itself." data-dst="本身。">本身。</trans></p>

<h2><a id="user-content-usage" class="anchor" href="#usage" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="Usage" data-dst="使用">使用</trans></h2>

<p><trans data-src="Require angular-clipboard as a dependency for your app:" data-dst="需要角剪贴板作为你的应用程序依赖：">需要角剪贴板作为你的应用程序依赖：</trans></p>

<div class="highlight highlight-source-js"><pre><span class="pl-smi"><trans data-src="angular" data-dst="角">角</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="module" data-dst="模块">模块</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="MyApp" data-dst="MyApp">MyApp</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", [" data-dst="，[">，[</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="angular-clipboard" data-dst="角剪贴板">角剪贴板</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src="])
    ." data-dst="]）。">]）。</trans><span class="pl-en"><trans data-src="controller" data-dst="控制器">控制器</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="MyController" data-dst="传递">传递</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", [" data-dst="，[">，[</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", " data-dst="，">，</trans><span class="pl-k"><trans data-src="function" data-dst="功能">功能</trans></span><trans data-src=" (" data-dst="（">（</trans><span class="pl-smi"><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans></span><trans data-src=") {
        " data-dst="）{">）{</trans><span class="pl-smi"><trans data-src="$scope" data-dst="$scope">$scope</trans></span><trans data-src="." data-dst=".">.</trans><span class="pl-smi"><trans data-src="textToCopy" data-dst="texttocopy">texttocopy</trans></span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="I can copy by clicking!" data-dst="我可以通过点击！">我可以通过点击！</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=";

        " data-dst="；">；</trans><span class="pl-smi"><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="success" data-dst="成功">成功</trans></span> <span class="pl-k">=</span> <span class="pl-k"><trans data-src="function" data-dst="功能">功能</trans></span><trans data-src=" () {
            " data-dst="（）{">（）{</trans><span class="pl-en"><trans data-src="console" data-dst="控制台">控制台</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-c1"><trans data-src="log" data-dst="日志">日志</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="Copied!" data-dst="复制！">复制！</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=");
        };

        " data-dst="
）；">
）；</trans><span class="pl-smi"><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="fail" data-dst="失败">失败</trans></span> <span class="pl-k">=</span> <span class="pl-k"><trans data-src="function" data-dst="功能">功能</trans></span><trans data-src=" (" data-dst="（">（</trans><span class="pl-smi"><trans data-src="err" data-dst="犯错">犯错</trans></span><trans data-src=") {
            " data-dst="）{">）{</trans><span class="pl-en"><trans data-src="console" data-dst="控制台">控制台</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-c1"><trans data-src="error" data-dst="误差">误差</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="Error!" data-dst="误差！">误差！</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", err);
        };
    }]);" data-dst="
，ERR）；）；} }；
 ]">
，ERR）；）；} }；
 ]</trans></pre></div>

<p><trans data-src="Copy text from an input field by clicking a button:" data-dst="通过点击一个按钮从一个输入字段复制文本：">通过点击一个按钮从一个输入字段复制文本：</trans></p>

<div class="highlight highlight-text-html-basic"><pre>&lt;<span class="pl-ent"><trans data-src="input" data-dst="输入">输入</trans></span> <span class="pl-e"><trans data-src="type" data-dst="类型">类型</trans></span>=<span class="pl-s"><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span><trans data-src="text" data-dst="文本">文本</trans><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span></span> <span class="pl-e"><trans data-src="ng-model" data-dst="NG型">NG型</trans></span>=<span class="pl-s"><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span><trans data-src="textToCopy" data-dst="texttocopy">texttocopy</trans><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span></span>&gt;
&lt;<span class="pl-ent"><trans data-src="button" data-dst="按钮">按钮</trans></span> <span class="pl-e"><trans data-src="clipboard" data-dst="剪贴板">剪贴板</trans></span> <span class="pl-e"><trans data-src="text" data-dst="文本">文本</trans></span>=<span class="pl-s"><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span><trans data-src="textToCopy" data-dst="texttocopy">texttocopy</trans><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span></span> <span class="pl-e"><trans data-src="on-copied" data-dst="copied在线">copied在线</trans></span>=<span class="pl-s"><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span><trans data-src="success()" data-dst="（成功）">（成功）</trans><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span></span> <span class="pl-e"><trans data-src="on-error" data-dst="我们的错误">我们的错误</trans></span>=<span class="pl-s"><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span><trans data-src="fail(err)" data-dst="失败（错误）">失败（错误）</trans><span class="pl-pds"><trans data-src="" "="" data-dst="“">“</trans></span></span>&gt;Copy&lt;/<span class="pl-ent"><trans data-src="button" data-dst="按钮">按钮</trans></span>&gt;</pre></div>

<p><trans data-src="You can supply a method to be called for the " data-dst="你可以被称为供应方法">你可以被称为供应方法</trans><code><trans data-src="on-copied" data-dst="copied在线">copied在线</trans></code><trans data-src=" and " data-dst="和">和</trans><code><trans data-src="on-error" data-dst="我们的错误">我们的错误</trans></code><trans data-src=" event. The " data-dst="事件这个">事件这个</trans><code><trans data-src="on-error" data-dst="我们的错误">我们的错误</trans></code><trans data-src=" function will be called with the error object as argument " data-dst="函数将被调用的错误对象作为参数" style="background: transparent;">函数将被调用的错误对象作为参数</trans><code><trans data-src="err" data-dst="犯错">犯错</trans></code><trans data-src="." data-dst="。">。</trans></p>

<h3><a id="user-content-use-as-service" class="anchor" href="#use-as-service" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="Use as service" data-dst="使用服务">使用服务</trans></h3>

<p><trans data-src="You can also invoke the copy to clipboard action directly by injecting the " data-dst="你也可以调用复制到剪贴板动作直接注入">你也可以调用复制到剪贴板动作直接注入</trans><code><trans data-src="clipboard" data-dst="剪贴板">剪贴板</trans></code><trans data-src=" service. Just remember it has to be in a click event, as clipboard access requires user action." data-dst="服务只记得它是在一个点击事件，剪贴板访问需要用户行为。">服务只记得它是在一个点击事件，剪贴板访问需要用户行为。</trans></p>

<div class="highlight highlight-source-js"><pre><span class="pl-smi"><trans data-src="angular" data-dst="角">角</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="module" data-dst="模块">模块</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="MyApp" data-dst="MyApp">MyApp</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", [" data-dst="，[">，[</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="angular-clipboard" data-dst="角剪贴板">角剪贴板</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src="])
    ." data-dst="]）。">]）。</trans><span class="pl-en"><trans data-src="controller" data-dst="controller">控制器</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="MyController" data-dst="传递">传递</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", [" data-dst="，[">，[</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", " data-dst="，">，</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="clipboard" data-dst="剪贴板">剪贴板</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", " data-dst="，">，</trans><span class="pl-k"><trans data-src="function" data-dst="功能">功能</trans></span><trans data-src=" (" data-dst="（">（</trans><span class="pl-smi"><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans></span><trans data-src=", " data-dst="，">，</trans><span class="pl-smi"><trans data-src="clipboard" data-dst="剪贴板">剪贴板</trans></span><trans data-src=") {
        " data-dst="）{">）{</trans><span class="pl-smi"><trans data-src="$scope" data-dst="美元的范围">美元的范围</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="clickHandler" data-dst="clickhandler">clickhandler</trans></span> <span class="pl-k">=</span> <span class="pl-k"><trans data-src="function" data-dst="功能">功能</trans></span><trans data-src=" () {
            " data-dst="（）{">（）{</trans><span class="pl-smi"><trans data-src="clipboard" data-dst="clipboard">剪贴板</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="copyText" data-dst="文本拷贝">文本拷贝</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="Copy this text" data-dst="复制这个文本">复制这个文本</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=");
        };
    }]);" data-dst="
）；}；
 } ]；">
）；}；
 } ]；</trans></pre></div>

<h3><a id="user-content-use-with-a-module-loader" class="anchor" href="#use-with-a-module-loader" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="Use with a module loader" data-dst="使用一个模块加载器">使用一个模块加载器</trans></h3>

<p><trans data-src="If you are using a module loader, you can import the module name when requiring it in angular. Works with any AMD/UMD/CommonJS module loader." data-dst="如果你正在使用一个模块的加载，你可以导入模块的名字时，需要在角。任何AMD / UMD / CommonJS模块装载机工程。">如果你正在使用一个模块的加载，你可以导入模块的名字时，需要在角。任何AMD / UMD / CommonJS模块装载机工程。</trans></p>

<div class="highlight highlight-source-js"><pre><span class="pl-k"><trans data-src="import" data-dst="进口">进口</trans></span> <span class="pl-smi"><trans data-src="clipboardModule" data-dst="clipboardmodule">clipboardmodule</trans></span> <span class="pl-k"><trans data-src="from" data-dst="从">从</trans></span> <span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="angular-clipboard" data-dst="角剪贴板">角剪贴板</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=";

" data-dst="；">；</trans><span class="pl-smi"><trans data-src="angular" data-dst="角">角</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="module" data-dst="module">模块</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="mymodule" data-dst="mymodule">mymodule</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", [" data-dst="，[">，[</trans><span class="pl-smi"><trans data-src="clipboardModule" data-dst="clipboardmodule">clipboardmodule</trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-c1"><trans data-src="name" data-dst="姓名">姓名</trans></span><trans data-src="]);" data-dst="]）；">]）；</trans></pre></div>
</article>
###EN
# angular-clipboard

[![Build Status][travis-image]][travis-url]
[![Test Coverage][coveralls-image]][coveralls-url]

Copy text to clipboard by clicking a button, without using Flash. This is using the new [Selection API](https://developer.mozilla.org/en-US/docs/Web/API/Selection) and [Clipboard API](https://developer.mozilla.org/en-US/docs/Web/API/ClipboardEvent) available in the latest browsers.

Browser support: Chrome 43+, Firefox 41+, Opera 29+ and IE10+.

See the [demo](https://rawgit.com/omichelsen/angular-clipboard/master/demo/demo.html).

## Install

Install using `npm` or `bower`:

```bash
$ npm install angular-clipboard --save
```
```bash
$ bower install angular-clipboard --save
```

angular-clipboard has no other dependencies than [Angular](https://angularjs.org/)
itself.

## Usage

Require angular-clipboard as a dependency for your app:

```javascript
angular.module('MyApp', ['angular-clipboard'])
    .controller('MyController', ['$scope', function ($scope) {
        $scope.textToCopy = 'I can copy by clicking!';

        $scope.success = function () {
            console.log('Copied!');
        };

        $scope.fail = function (err) {
            console.error('Error!', err);
        };
    }]);
```

Copy text from an input field by clicking a button:

```html
<input type="text" ng-model="textToCopy">
<button clipboard text="textToCopy" on-copied="success()" on-error="fail(err)">Copy</button>
```

You can supply a method to be called for the `on-copied` and `on-error` event. The `on-error` function will be called with the error object as argument `err`.

### Use as service

You can also invoke the copy to clipboard action directly by injecting the `clipboard` service. Just remember it has to be in a click event, as clipboard access requires user action.

```javascript
angular.module('MyApp', ['angular-clipboard'])
    .controller('MyController', ['$scope', 'clipboard', function ($scope, clipboard) {
        $scope.clickHandler = function () {
            clipboard.copyText('Copy this text');
        };
    }]);
```

### Use with a module loader

If you are using a module loader, you can import the module name when requiring it in angular. Works with any AMD/UMD/CommonJS module loader.

```javascript
import clipboardModule from 'angular-clipboard';

angular.module('mymodule', [clipboardModule.name]);
```

[travis-image]: https://img.shields.io/travis/omichelsen/angular-clipboard/master.svg
[travis-url]: https://travis-ci.org/omichelsen/angular-clipboard
[coveralls-image]: https://img.shields.io/coveralls/omichelsen/angular-clipboard/master.svg
[coveralls-url]: https://coveralls.io/r/omichelsen/angular-clipboard?branch=master
