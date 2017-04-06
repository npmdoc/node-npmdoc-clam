# api documentation for  clam (v1.0.12)  [![npm package](https://img.shields.io/npm/v/npmdoc-clam.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-clam) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-clam.svg)](https://travis-ci.org/npmdoc/node-npmdoc-clam)
#### A full Web front end develop envirment.

[![NPM](https://nodei.co/npm/clam.png?downloads=true)](https://www.npmjs.com/package/clam)

[![apidoc](https://npmdoc.github.io/node-npmdoc-clam/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-clam_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-clam/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-clam/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-clam/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Wayfind"
    },
    "bin": {
        "clam": "./bin/clam"
    },
    "dependencies": {
        "commander": "~1.0.5",
        "condenser": "~0.0.15",
        "cpr": "~0.1.1",
        "debug": "~0.7.0",
        "doji": "~0.1.6",
        "essi": "~0.10.26",
        "flex-combo": "~0.12.20",
        "iconv-lite": "~0.4.11",
        "is-utf8": "~0.2.0",
        "joinbuffers": "~0.1.1",
        "juicer": "~0.6.11",
        "less": "1.6.0",
        "mime": "~1.2.7",
        "mkdirp": "~0.3.4",
        "plug-base": "~0.9.4",
        "send": "0.1.0",
        "underscore": "~1.4.2",
        "update-notifier": "~0.3.1"
    },
    "description": "A full Web front end develop envirment.",
    "devDependencies": {},
    "directories": {
        "test": "tests"
    },
    "dist": {
        "shasum": "80cfd41121f968d212066958117f2b6cadb50f77",
        "tarball": "https://registry.npmjs.org/clam/-/clam-1.0.12.tgz"
    },
    "gitHead": "48c260861ad2495bd19251c3f7bda0749b82bbc4",
    "keywords": [
        "toolchain",
        "commandline",
        "frontend"
    ],
    "license": "BSD",
    "main": "index.js",
    "maintainers": [
        {
            "name": "wayfind",
            "email": "whyer1@gmail.com"
        },
        {
            "name": "xudafeng",
            "email": "xudafeng@126.com"
        },
        {
            "name": "limingv5",
            "email": "limingv5@gmail.com"
        },
        {
            "name": "lichenhao",
            "email": "crazy.jser@gmail.com"
        }
    ],
    "name": "clam",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git@gitlab.alibaba-inc.com:aaa/clam.git"
    },
    "scripts": {
        "test": "mocha tests/test.js"
    },
    "version": "1.0.12"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module clam](#apidoc.module.clam)
1.  [function <span class="apidocSignatureSpan">clam.</span>build (timestamp)](#apidoc.element.clam.build)
1.  [function <span class="apidocSignatureSpan">clam.</span>dataApiHandle ()](#apidoc.element.clam.dataApiHandle)
1.  [function <span class="apidocSignatureSpan">clam.</span>init ()](#apidoc.element.clam.init)
1.  [function <span class="apidocSignatureSpan">clam.</span>on ()](#apidoc.element.clam.on)
1.  [function <span class="apidocSignatureSpan">clam.</span>project (prj)](#apidoc.element.clam.project)
1.  object <span class="apidocSignatureSpan">clam.</span>assetUrl
1.  object <span class="apidocSignatureSpan">clam.</span>assetsTool
1.  object <span class="apidocSignatureSpan">clam.</span>config
1.  object <span class="apidocSignatureSpan">clam.</span>hosts
1.  object <span class="apidocSignatureSpan">clam.</span>jsonHandle
1.  object <span class="apidocSignatureSpan">clam.</span>mocker
1.  object <span class="apidocSignatureSpan">clam.</span>mod
1.  object <span class="apidocSignatureSpan">clam.</span>page
1.  object <span class="apidocSignatureSpan">clam.</span>proxy
1.  object <span class="apidocSignatureSpan">clam.</span>selectfile
1.  object <span class="apidocSignatureSpan">clam.</span>template
1.  object <span class="apidocSignatureSpan">clam.</span>widget

#### [module clam.assetUrl](#apidoc.module.clam.assetUrl)
1.  [function <span class="apidocSignatureSpan">clam.assetUrl.</span>toAbsolutePath (pageContent, urlDir)](#apidoc.element.clam.assetUrl.toAbsolutePath)

#### [module clam.assetsTool](#apidoc.module.clam.assetsTool)
1.  [function <span class="apidocSignatureSpan">clam.assetsTool.</span>clearCacheMod ()](#apidoc.element.clam.assetsTool.clearCacheMod)
1.  [function <span class="apidocSignatureSpan">clam.assetsTool.</span>feLoader (data)](#apidoc.element.clam.assetsTool.feLoader)

#### [module clam.config](#apidoc.module.clam.config)
1.  [function <span class="apidocSignatureSpan">clam.config.</span>get (key)](#apidoc.element.clam.config.get)
1.  [function <span class="apidocSignatureSpan">clam.config.</span>init ()](#apidoc.element.clam.config.init)
1.  [function <span class="apidocSignatureSpan">clam.config.</span>on (evtName, fn)](#apidoc.element.clam.config.on)
1.  [function <span class="apidocSignatureSpan">clam.config.</span>root ()](#apidoc.element.clam.config.root)
1.  [function <span class="apidocSignatureSpan">clam.config.</span>set (key, config)](#apidoc.element.clam.config.set)

#### [module clam.dataApiHandle](#apidoc.module.clam.dataApiHandle)
1.  [function <span class="apidocSignatureSpan">clam.</span>dataApiHandle ()](#apidoc.element.clam.dataApiHandle.dataApiHandle)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>_local (req, res, next, options)](#apidoc.element.clam.dataApiHandle._local)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>_remote (req, res, next, options)](#apidoc.element.clam.dataApiHandle._remote)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>handle ()](#apidoc.element.clam.dataApiHandle.handle)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>httpProxy (req, res, next, options)](#apidoc.element.clam.dataApiHandle.httpProxy)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>httpsProxy (req, res, next, info)](#apidoc.element.clam.dataApiHandle.httpsProxy)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>proxy (req, res, next, options)](#apidoc.element.clam.dataApiHandle.proxy)
1.  [function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>socketProxy (req, res, next, info)](#apidoc.element.clam.dataApiHandle.socketProxy)
1.  object <span class="apidocSignatureSpan">clam.dataApiHandle.</span>_reFullURI
1.  object <span class="apidocSignatureSpan">clam.dataApiHandle.</span>remotes
1.  string <span class="apidocSignatureSpan">clam.dataApiHandle.</span>charset

#### [module clam.hosts](#apidoc.module.clam.hosts)
1.  [function <span class="apidocSignatureSpan">clam.hosts.</span>restore ()](#apidoc.element.clam.hosts.restore)
1.  [function <span class="apidocSignatureSpan">clam.hosts.</span>setHosts (pro_hosts)](#apidoc.element.clam.hosts.setHosts)

#### [module clam.jsonHandle](#apidoc.module.clam.jsonHandle)
1.  [function <span class="apidocSignatureSpan">clam.jsonHandle.</span>json ()](#apidoc.element.clam.jsonHandle.json)

#### [module clam.mocker](#apidoc.module.clam.mocker)
1.  [function <span class="apidocSignatureSpan">clam.mocker.</span>getMixedMockDate (param, url, isRootPage)](#apidoc.element.clam.mocker.getMixedMockDate)

#### [module clam.mod](#apidoc.module.clam.mod)
1.  [function <span class="apidocSignatureSpan">clam.mod.</span>add (modName, description, template)](#apidoc.element.clam.mod.add)
1.  [function <span class="apidocSignatureSpan">clam.mod.</span>addCore ()](#apidoc.element.clam.mod.addCore)
1.  [function <span class="apidocSignatureSpan">clam.mod.</span>del (data)](#apidoc.element.clam.mod.del)
1.  [function <span class="apidocSignatureSpan">clam.mod.</span>list ()](#apidoc.element.clam.mod.list)

#### [module clam.page](#apidoc.module.clam.page)
1.  [function <span class="apidocSignatureSpan">clam.page.</span>add (name, url, description, template)](#apidoc.element.clam.page.add)
1.  [function <span class="apidocSignatureSpan">clam.page.</span>del (data)](#apidoc.element.clam.page.del)
1.  [function <span class="apidocSignatureSpan">clam.page.</span>list ()](#apidoc.element.clam.page.list)
1.  [function <span class="apidocSignatureSpan">clam.page.</span>update ()](#apidoc.element.clam.page.update)

#### [module clam.project](#apidoc.module.clam.project)
1.  [function <span class="apidocSignatureSpan">clam.</span>project (prj)](#apidoc.element.clam.project.project)
1.  [function <span class="apidocSignatureSpan">clam.project.</span>setUrls (urls)](#apidoc.element.clam.project.setUrls)

#### [module clam.proxy](#apidoc.module.clam.proxy)
1.  [function <span class="apidocSignatureSpan">clam.proxy.</span>fetch (url, host, callback)](#apidoc.element.clam.proxy.fetch)

#### [module clam.selectfile](#apidoc.module.clam.selectfile)
1.  [function <span class="apidocSignatureSpan">clam.selectfile.</span>getTree (root)](#apidoc.element.clam.selectfile.getTree)

#### [module clam.template](#apidoc.module.clam.template)
1.  [function <span class="apidocSignatureSpan">clam.template.</span>convert (src, dest, param, destName)](#apidoc.element.clam.template.convert)
1.  [function <span class="apidocSignatureSpan">clam.template.</span>init ()](#apidoc.element.clam.template.init)

#### [module clam.widget](#apidoc.module.clam.widget)
1.  [function <span class="apidocSignatureSpan">clam.widget.</span>add (widgetName, description, template)](#apidoc.element.clam.widget.add)
1.  [function <span class="apidocSignatureSpan">clam.widget.</span>del (data)](#apidoc.element.clam.widget.del)
1.  [function <span class="apidocSignatureSpan">clam.widget.</span>list ()](#apidoc.element.clam.widget.list)



# <a name="apidoc.module.clam"></a>[module clam](#apidoc.module.clam)

#### <a name="apidoc.element.clam.build"></a>[function <span class="apidocSignatureSpan">clam.</span>build (timestamp)](#apidoc.element.clam.build)
- description and source-code
```javascript
build = function (timestamp){
    var build = require('./lib/build.js');
    build.build('server', timestamp);
}
```
- example usage
```shell
...
            return;
        }
        var startServer = require('./lib/server.js');
        startServer(false);
    },
    build: function(timestamp){
        var build = require('./lib/build.js');
        build.build('server', timestamp);
    }
}
// clam.on();
...
```

#### <a name="apidoc.element.clam.dataApiHandle"></a>[function <span class="apidocSignatureSpan">clam.</span>dataApiHandle ()](#apidoc.element.clam.dataApiHandle)
- description and source-code
```javascript
dataApiHandle = function () {
    return function (req, res, next) {
        var remotes = exports.remotes;
        // no interfaces defined
        if (!remotes || !remotes.length) {
            next();
            return;
        }
        var url = uri.parse(req.url);
        _.some(remotes, function (options) {
            // equals or matched the option pathname
            if (options.pathname === url.pathname || url.pathname.match(options.pathname)) {
                exports.proxy(req, res, next, options);
                return true;
            }
        }) || next();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.init"></a>[function <span class="apidocSignatureSpan">clam.</span>init ()](#apidoc.element.clam.init)
- description and source-code
```javascript
init = function (){
    config.init();
    template.init();
    var ret = project({});

    ret.data.forEach(function (ac) {
        debug(ac.action, ac.content);
    });
    process.exit(0);
}
```
- example usage
```shell
...
var template = require('./lib/template.js');
var mod = require('./lib/mod.js');
var page = require('./lib/page.js');
var widget = require('./lib/widget.js');

var clam = module.exports = {
    init: function(){
config.init();
template.init();
var ret = project({});

ret.data.forEach(function (ac) {
    debug(ac.action, ac.content);
});
process.exit(0);
...
```

#### <a name="apidoc.element.clam.on"></a>[function <span class="apidocSignatureSpan">clam.</span>on ()](#apidoc.element.clam.on)
- description and source-code
```javascript
on = function (){
    var prjInfo = config.get('project');
    if (!prjInfo) {
        console.log('Execute "clam init".');
        return;
    }
    var startServer = require('./lib/server.js');
    startServer(false);
}
```
- example usage
```shell
...
        startServer(false);
    },
    build: function(timestamp){
        var build = require('./lib/build.js');
        build.build('server', timestamp);
    }
}
// clam.on();
...
```

#### <a name="apidoc.element.clam.project"></a>[function <span class="apidocSignatureSpan">clam.</span>project (prj)](#apidoc.element.clam.project)
- description and source-code
```javascript
project = function (prj) {
  prjDir = config.root();
  debug('项目目录:%s', prjDir);
  var state = prjState(prjDir);
  debug('项目状态:%s', state);
  if (!prj) {
    var info = getProject(prjDir, state);
    return info;
  }

  var actions = [];
  if (state !== 'normal') {
    if (state === 'blank') {
      var pagesFullDir = path.join(prjDir, initConf.pagesDir);
      mkdirp.sync(pagesFullDir);
      actions.push({action: '创建页面目录', content: pagesFullDir});

      var modsFullDir = path.join(prjDir, initConf.modsDir);
      mkdirp.sync(modsFullDir);
      actions.push({action: '创建模块目录', content: modsFullDir});

      var widgetsFullDir = path.join(prjDir, initConf.widgetsDir)
      mkdirp.sync(widgetsFullDir);
      actions.push({action: '创建组件目录', content: widgetsFullDir});

      var buildFullDir = path.join(prjDir, initConf.buildDir);
      mkdirp.sync(buildFullDir);
      actions.push({action: '创建构建目录', content: buildFullDir});

      var testsFullDir = path.join(prjDir, initConf.testsDir);
      mkdirp.sync(testsFullDir);
      actions.push({action: '创建测试目录', content: testsFullDir});
    }
    prj = initConf;
    var dirs = prjDir.split(path.sep);
    prj.name = dirs[dirs.length - 1];
  }


  var oldPrj = config.get('project') || prj;
  if (oldPrj.hosts && prj.hosts && oldPrj.hosts !== prj.hosts) {
    hostSwitch.setHosts(prj.hosts);
    actions.push({action: '更新hosts文件', content: '操作系统hosts文件'});
  }
  for (var k in prj) {
    oldPrj[k] = prj[k];
  }

  config.set('project', oldPrj);
  actions.push({action: '更新项目元文件', content: '.clam/project.json'});

  //getMuiConfig();
  //actions.push({action: '更新项目gconfig文件', content: '.clam/gconfig.json'});

  return {
    succeed: true,
    msg: '更新项目信息',
    data: actions
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.assetUrl"></a>[module clam.assetUrl](#apidoc.module.clam.assetUrl)

#### <a name="apidoc.element.clam.assetUrl.toAbsolutePath"></a>[function <span class="apidocSignatureSpan">clam.assetUrl.</span>toAbsolutePath (pageContent, urlDir)](#apidoc.element.clam.assetUrl.toAbsolutePath)
- description and source-code
```javascript
function toAbsolutePath(pageContent, urlDir) {
    var cdnPath = config.get('project').cdnPath;

    //处理模块中资源引用
    var localHosts = localhosts();
    debug('本地host列表[%s]', localHosts);

<span class="apidocCodeCommentSpan">    /*/抽取cdn域名
    var cdnHost = cdnPath.match(cdnPathReg);
    if (cdnHost) {
        cdnHost = cdnHost[0];
    }
    else {
        cdnHost = '';
    }*/
</span>
    //以http开头的就改变cndPath中的端口号
    var port = config.get('project').port;
    var cdnPathWithPort = cdnPath;
    if (cdnPath.indexOf('http') === 0) {
        //如果是预览服务器运行在80端口，就不更改
        if (!port || port == 80) {
            port = '';
        }
        else {
            port = ':' + port;
        }
        var matchResult = cdnPath.match(/(http:\/\/[\w\.]+?)(\/.*)/);
        if (matchResult) {
            cdnPathWithPort = matchResult[1] + port + matchResult[2];
        }
    }

    var resourceRootDir = '';
    debug('资源跟路径%s', resourceRootDir);
    //debug('处理前内容%s', pageContent);
    //处理带域名的链接。1、增加端口号。2、增加时间戳路径
    localHosts.forEach(function(localHost){
        localHost = localHost.replace(/\./g, '\\.');
        var scriptWithDomain = new RegExp('<script[^>]*? src=[\'"](?:http[s]?:\\/\\/)(' + localHost + ')(.*)[\'"][^>]*?>', 'g');
        pageContent = pageContent.replace(scriptWithDomain, function ($1, $2) {
            return $1.replace($2, $2 + port);
        });
    });

    localHosts.forEach(function(localHost){
        localHost = localHost.replace(/\./g, '\\.');
        var styleWithDomain = new RegExp('<link[^>]*? href=[\'"](?:http[s]?:\\/\\/)(' + localHost + ')(.*)[\'"][^>]*?>', 'g');
        pageContent = pageContent.replace(styleWithDomain, function ($1, $2) {
            return $1.replace($2, $2 + port);
        });
    });
    //替换资源相对路径应为带域名和端口号的绝对路径，根据当前页面所在相对路径转换
    pageContent = pageContent.replace(scriptReg, function ($1, $2, $3) {
        if ($3.match(/^\$\{/)) {
            return $1;
        }
        else {
            var replacedPath = join(resourceRootDir, urlDir, $3).replace(/\\/ig, '/');
            if ($1.match(/clam-moveto/) && !$1.match(/clam-moveto\s{0,}=\s{0,}["']\s{0,}head\s{0,}["']/) && !$1.match(/clam-moveto\s{0,}=\s{0,}["']\s{0,}tail\s{0,}["']/)) {
                replacedPath = "$CLAM_VER$/"+replacedPath;
            }
            return $1.replace($3, cdnPathWithPort + '/' + replacedPath).replace(/["'](\s{0,})([^"']*?)(\s{0,})["']/g, function($
1,$2,$3) {
                return '"'+$3+'"';
            });
        }
    });
    pageContent = pageContent.replace(styleReg, function ($1, $2, $3) {
        if ($3.match(/^\$\{/)) {
            return $1;
        }
        else {
            var replacedPath = join(resourceRootDir, urlDir, $3).replace(/\\/ig, '/');
            if ($1.match(/clam-moveto/) && !$1.match(/clam-moveto\s{0,}=\s{0,}["']\s{0,}head\s{0,}["']/) && !$1.match(/clam-moveto\s{0,}=\s{0,}["']\s{0,}tail\s{0,}["']/)) {
                console.log(replacedPath)
                replacedPath = "$CLAM_VER$/"+replacedPath;
            }
            return $1.replace($3, cdnPathWithPort + '/' + replacedPath).replace(/["'](\s{0,})([^"']*?)(\s{0,})["']/g, function($
1,$2,$3) {
                return '"'+$3+'"';
            });
        }
    });

    //处理绝对路径引用。直接增加域名和端口号
    pageContent = pageContent.replace(absScript, function ($1, $2) {
        return $1.replace($2, cdnPathWithPort + $2);
    });
    pageContent = pageContent.replace(absStyle, function ($1, $2) {
        return $1.replace($2, cdnPathWithPort + $2);
    });
    //debug('处理后内容%s', pageContent);
    return pageContent;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.assetsTool"></a>[module clam.assetsTool](#apidoc.module.clam.assetsTool)

#### <a name="apidoc.element.clam.assetsTool.clearCacheMod"></a>[function <span class="apidocSignatureSpan">clam.assetsTool.</span>clearCacheMod ()](#apidoc.element.clam.assetsTool.clearCacheMod)
- description and source-code
```javascript
clearCacheMod = function () {
    hasLoadMod = {};   // 页面刷新时需要清楚记录的模块
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.assetsTool.feLoader"></a>[function <span class="apidocSignatureSpan">clam.assetsTool.</span>feLoader (data)](#apidoc.element.clam.assetsTool.feLoader)
- description and source-code
```javascript
function feLoader(data) {
    var cmd = [];
    data.forEach(function(i){
        cmd.push('{express:' + i['express'] + ', id:"'+ i['id'] + '"}');
    })

    cmd = 'var data = [' + cmd.join(',') + '], ret = [];'
        + 'for (var i = 0, str; i < data.length; i++) {'
        + '    str = data[i]["express"];'
        + '    if (str) {'
        + '        ret.push({'
        + '            express: str,'
        + '            id: data[i]["id"]'
        + '        });'
        + '    }'
        + '}'
        + 'return ret;';

    var fn = new Function('$assetsTool', cmd);
    return fn(new AssetsTool());
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.config"></a>[module clam.config](#apidoc.module.clam.config)

#### <a name="apidoc.element.clam.config.get"></a>[function <span class="apidocSignatureSpan">clam.config.</span>get (key)](#apidoc.element.clam.config.get)
- description and source-code
```javascript
function get(key){
    if(!PRJROOT){
        init();
    }
    return CONFIG[key];
}
```
- example usage
```shell
...

    ret.data.forEach(function (ac) {
        debug(ac.action, ac.content);
    });
    process.exit(0);
},
on: function(){
    var prjInfo = config.get('project');
    if (!prjInfo) {
        console.log('Execute "clam init".');
        return;
    }
    var startServer = require('./lib/server.js');
    startServer(false);
},
...
```

#### <a name="apidoc.element.clam.config.init"></a>[function <span class="apidocSignatureSpan">clam.config.</span>init ()](#apidoc.element.clam.config.init)
- description and source-code
```javascript
function init() {

    //只初始化一次
    if (PRJROOT) {
        return;
    }

    //命令行传入的目录参数在不同调用方式下下标不同，处理相对路径为绝对路径
    var argvs = process.argv;
    var dir = process.cwd();

    //从获取命令行--root参数
    for (var i = 0; i < argvs.length; i++) {
        if (argvs[i] === '--root' || argvs[i] === '-r') {
            if (i + 1 < argvs.length) {
                dir = argvs[i + 1];
            }
        }
    }
    dir = path.resolve(dir);
    var metaDir = path.join(dir, META.dir);

    //兼容windows和Linux路径
    while (!fs.existsSync(metaDir) && metaDir !== '/' + META.dir && !metaDir.match(/\w{1,1}:\\.clam/)) {
        metaDir = path.join(metaDir, '../..', META.dir);
    }
    PRJROOT = path.join(metaDir, '..');
    if (PRJROOT === '/' || PRJROOT.match(/\w{1,1}:\\$/)) {
        PRJROOT = dir;
    }

    var metaDir = path.join(PRJROOT, META.dir);
    if(!fs.existsSync(metaDir)){
        return;
    }
    var files = fs.readdirSync(metaDir);
    debug('%s目录，文件列表%s', metaDir, util.inspect(files));

    files.forEach(function (file, i) {
        if (/.+\.json$/.test(file)) {
            readFromFile(file);
            createWatch(file, metaDir);
        }
    });
}
```
- example usage
```shell
...
var template = require('./lib/template.js');
var mod = require('./lib/mod.js');
var page = require('./lib/page.js');
var widget = require('./lib/widget.js');

var clam = module.exports = {
    init: function(){
config.init();
template.init();
var ret = project({});

ret.data.forEach(function (ac) {
    debug(ac.action, ac.content);
});
process.exit(0);
...
```

#### <a name="apidoc.element.clam.config.on"></a>[function <span class="apidocSignatureSpan">clam.config.</span>on (evtName, fn)](#apidoc.element.clam.config.on)
- description and source-code
```javascript
function on(evtName, fn){
    return EVENT.on(evtName, fn);
}
```
- example usage
```shell
...
        startServer(false);
    },
    build: function(timestamp){
        var build = require('./lib/build.js');
        build.build('server', timestamp);
    }
}
// clam.on();
...
```

#### <a name="apidoc.element.clam.config.root"></a>[function <span class="apidocSignatureSpan">clam.config.</span>root ()](#apidoc.element.clam.config.root)
- description and source-code
```javascript
function root(){
    if(!PRJROOT){
        init();
    }
    return PRJROOT;
}
```
- example usage
```shell
...
// ["socket://www.taobao.com:80/a/d/b?a=1&b=2", "socket", "www.taobao.com", "80", "/a/d/b", "a=1&b=2"]
// 'socket://www.taobao.com:80/a/d/b?a=1&b=2'.match(/^(?:(http(?:s*)|socket):\/\/)*([^\:\/]+)*(?:\:(\d+))*(\/[^?]*)(?:\?(.*))*$/)
exports._reFullURI = /^(?:(http(?:s*)|socket):\/\/)*([^\:\/]+)*(?:\:(\d+))*(\/[^?]*)(?:\?(.*))*$/;

if (prjInfo && prjInfo.dataApi) {
_.each(prjInfo.dataApi, function (options) {
  // 接口文件放到
  var local = path.join(config.root(), '/.clam/dataApi/', options.local || '');
  var remote = (options.remote || '').match(exports._reFullURI);
  var type = options.type || 'auto';
  var pathname = options.url;
  if (!pathname || !remote) {
    debug('Failed to build remote %s from %s !', remote, local);
  }
  exports.remotes.push({
...
```

#### <a name="apidoc.element.clam.config.set"></a>[function <span class="apidocSignatureSpan">clam.config.</span>set (key, config)](#apidoc.element.clam.config.set)
- description and source-code
```javascript
function set(key, config){
    if(!PRJROOT){
        init();
    }
    var metaDir = path.join(PRJROOT, META.dir);
    debug('目录:%s', metaDir);
    var metaFileName = path.join(metaDir, key+'.json');
    CONFIG[key] = config;
    if(!fs.existsSync(metaDir)){
        mkdirp.sync(metaDir);
    }
    var configStr = JSON.stringify(config);
    configStr = beautify(configStr);

    if(!fs.existsSync(metaFileName)){
        debug("创建配置文件 %s",metaFileName);
        fs.writeFileSync(metaFileName, configStr);
        createWatch(key+'.json', metaDir);
        return;
    }

    fs.writeFileSync(metaFileName, configStr);
    return;
}
```
- example usage
```shell
...
                line_disable(_name);
            });
            lines.push(ip + ' ' + item.join(' ') + split_char);
        }
    });
    lines.push(endTag + split_char);

    hostFile.set(lines.join(''));
};

/**
 * 恢复HOST并存储
 */
var restore = function () {
    var host = hostFile.get();
...
```



# <a name="apidoc.module.clam.dataApiHandle"></a>[module clam.dataApiHandle](#apidoc.module.clam.dataApiHandle)

#### <a name="apidoc.element.clam.dataApiHandle.dataApiHandle"></a>[function <span class="apidocSignatureSpan">clam.</span>dataApiHandle ()](#apidoc.element.clam.dataApiHandle.dataApiHandle)
- description and source-code
```javascript
dataApiHandle = function () {
    return function (req, res, next) {
        var remotes = exports.remotes;
        // no interfaces defined
        if (!remotes || !remotes.length) {
            next();
            return;
        }
        var url = uri.parse(req.url);
        _.some(remotes, function (options) {
            // equals or matched the option pathname
            if (options.pathname === url.pathname || url.pathname.match(options.pathname)) {
                exports.proxy(req, res, next, options);
                return true;
            }
        }) || next();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.dataApiHandle._local"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>_local (req, res, next, options)](#apidoc.element.clam.dataApiHandle._local)
- description and source-code
```javascript
_local = function (req, res, next, options) {
    fs.stat(options.local, function (err, stats) {
        if (!err && stats.isFile()) {
            var action = require(options.local);
            if ('function' === typeof action.handle) {
                action.handle(req, res, next, options);
                return;
            }
            try {
                // 反回的数据不是模块，就认为是json了。只允许两种。推荐直接返回json。
                // 如果会nodejs。直接操作数据。方便。快捷
                res.setHeader('Content-Type', 'application/json;text/json; charset=' + exports.charset);
                res.write(JSON.stringify(action));
                res.end();
            } catch ( e ) {
                debug('Stringify failed! Data: %o \n\r File: %s', action, options.local);
                res.end(JSON.stringify({
                    "errno": 500,
                    "errmsg": "Stringify failed ! Please check your action file : "+options.local+"! "
                }));
            }
            return;
        }
        if (options.type === 'auto') {
            return exports._remote(req, res, next, options);
        }
        return next();
    });
}
```
- example usage
```shell
...
});
  });
}

exports.handle = exports;
exports.proxy = function (req, res, next, options) {
if (options.type === 'auto' || options.type === 'local') {
    exports._local(req, res, next, options);
}
if (options.type === 'remote') {
    exports._remote(req, res, next, options);
}
};
exports._local = function (req, res, next, options) {
fs.stat(options.local, function (err, stats) {
...
```

#### <a name="apidoc.element.clam.dataApiHandle._remote"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>_remote (req, res, next, options)](#apidoc.element.clam.dataApiHandle._remote)
- description and source-code
```javascript
_remote = function (req, res, next, options) {
    if (options.remote.agreement === 'http') {
        return exports.httpProxy(req, res, next, options);
    }
    if (options.remote.agreement === 'https') {
        return exports.httpsProxy(req, res, next, options);
    }
    if (options.remote.agreement === 'socket') {
        return exports.socketProxy(req, res, next, options);
    }
    debug('Remote failed; Unknown agreement <%s> ', options.agreement);
    next();
}
```
- example usage
```shell
...

exports.handle = exports;
exports.proxy = function (req, res, next, options) {
if (options.type === 'auto' || options.type === 'local') {
    exports._local(req, res, next, options);
}
if (options.type === 'remote') {
    exports._remote(req, res, next, options);
}
};
exports._local = function (req, res, next, options) {
fs.stat(options.local, function (err, stats) {
    if (!err && stats.isFile()) {
        var action = require(options.local);
        if ('function' === typeof action.handle) {
...
```

#### <a name="apidoc.element.clam.dataApiHandle.handle"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>handle ()](#apidoc.element.clam.dataApiHandle.handle)
- description and source-code
```javascript
handle = function () {
    return function (req, res, next) {
        var remotes = exports.remotes;
        // no interfaces defined
        if (!remotes || !remotes.length) {
            next();
            return;
        }
        var url = uri.parse(req.url);
        _.some(remotes, function (options) {
            // equals or matched the option pathname
            if (options.pathname === url.pathname || url.pathname.match(options.pathname)) {
                exports.proxy(req, res, next, options);
                return true;
            }
        }) || next();
    };
}
```
- example usage
```shell
...
}
};
exports._local = function (req, res, next, options) {
fs.stat(options.local, function (err, stats) {
    if (!err && stats.isFile()) {
        var action = require(options.local);
        if ('function' === typeof action.handle) {
            action.handle(req, res, next, options);
            return;
        }
        try {
            // 反回的数据不是模块，就认为是json了。只允许两种。推荐直接返回json。
            // 如果会nodejs。直接操作数据。方便。快捷
            res.setHeader('Content-Type', 'application/json;text/json; charset=' + exports.charset);
            res.write(JSON.stringify(action));
...
```

#### <a name="apidoc.element.clam.dataApiHandle.httpProxy"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>httpProxy (req, res, next, options)](#apidoc.element.clam.dataApiHandle.httpProxy)
- description and source-code
```javascript
httpProxy = function (req, res, next, options) {
    var remote = options.remote;
    var url = uri.parse(req.url);
    var pathname = remote.pathname || url.pathname;
    var querystring = remote.querystring;
    querystring += (url.query ? '&' : '') + (url.query || '');

    var nsreq = http.request({
        host: remote.domain,
        port: remote.port,
        path: pathname + '?' + querystring,
        method: req.method,
        headers: req.headers
    }, function (nsres) {
        res.statusCode = nsres.statusCode;
        // 返回的数据中头信息确保为对方反馈数据
        var headers = nsres.headers;
        var headerItem;
        var header;
        for (header in headers) {
            headerItem = headers[header];
            res.setHeader(header, headerItem);
        }
        var buffs = [];
        // 收到数据，立刻返回。
        nsres.on('data', function (chunk) {
            buffs.push(chunk);
        });
        // 结束同时关闭此次连接
        nsres.on('end', function () {
            buff = joinbuffers(buffs);
            //fix 80% situation bom problem.quick and dirty
            if(buff[0] === 239 && buff[1] === 187 && buff[2] === 191) {
                buff = buff.slice(3, buff.length);
            }
            var buffChatset = isUtf8(buff) ? 'utf8' : 'gbk';
            if (buffChatset !== exports.charset) {
                buff = iconv.encode(iconv.decode(buff, buffChatset), exports.charset);
            }
            res.write(buff);
            res.end();
        });
    });
    req.on('data', function (chunk) {
       nsreq.write(chunk);
    });
    req.on('end', function () {
       nsreq.end();
    });
    nsreq.on('error', function (e) {
        debug(e);
    });
}
```
- example usage
```shell
...
        return exports._remote(req, res, next, options);
    }
    return next();
});
};
exports._remote = function (req, res, next, options) {
if (options.remote.agreement === 'http') {
    return exports.httpProxy(req, res, next, options);
}
if (options.remote.agreement === 'https') {
    return exports.httpsProxy(req, res, next, options);
}
if (options.remote.agreement === 'socket') {
    return exports.socketProxy(req, res, next, options);
}
...
```

#### <a name="apidoc.element.clam.dataApiHandle.httpsProxy"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>httpsProxy (req, res, next, info)](#apidoc.element.clam.dataApiHandle.httpsProxy)
- description and source-code
```javascript
httpsProxy = function (req, res, next, info) {
    // ?
}
```
- example usage
```shell
...
    });
};
exports._remote = function (req, res, next, options) {
    if (options.remote.agreement === 'http') {
        return exports.httpProxy(req, res, next, options);
    }
    if (options.remote.agreement === 'https') {
        return exports.httpsProxy(req, res, next, options);
    }
    if (options.remote.agreement === 'socket') {
        return exports.socketProxy(req, res, next, options);
    }
    debug('Remote failed; Unknown agreement <%s> ', options.agreement);
    next();
};
...
```

#### <a name="apidoc.element.clam.dataApiHandle.proxy"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>proxy (req, res, next, options)](#apidoc.element.clam.dataApiHandle.proxy)
- description and source-code
```javascript
proxy = function (req, res, next, options) {
    if (options.type === 'auto' || options.type === 'local') {
        exports._local(req, res, next, options);
    }
    if (options.type === 'remote') {
        exports._remote(req, res, next, options);
    }
}
```
- example usage
```shell
...
            next();
            return;
        }
        var url = uri.parse(req.url);
        _.some(remotes, function (options) {
            // equals or matched the option pathname
            if (options.pathname === url.pathname || url.pathname.match(options.pathname)) {
                exports.proxy(req, res, next, options);
                return true;
            }
        }) || next();
    };
};
exports.remotes = [];
...
```

#### <a name="apidoc.element.clam.dataApiHandle.socketProxy"></a>[function <span class="apidocSignatureSpan">clam.dataApiHandle.</span>socketProxy (req, res, next, info)](#apidoc.element.clam.dataApiHandle.socketProxy)
- description and source-code
```javascript
socketProxy = function (req, res, next, info) {
    // ?
}
```
- example usage
```shell
...
if (options.remote.agreement === 'http') {
    return exports.httpProxy(req, res, next, options);
}
if (options.remote.agreement === 'https') {
    return exports.httpsProxy(req, res, next, options);
}
if (options.remote.agreement === 'socket') {
    return exports.socketProxy(req, res, next, options);
}
debug('Remote failed; Unknown agreement <%s> ', options.agreement);
next();
};
exports.charset = prjInfo ? prjInfo.charset[0] : "utf-8";
exports.httpProxy = function (req, res, next, options) {
var remote = options.remote;
...
```



# <a name="apidoc.module.clam.hosts"></a>[module clam.hosts](#apidoc.module.clam.hosts)

#### <a name="apidoc.element.clam.hosts.restore"></a>[function <span class="apidocSignatureSpan">clam.hosts.</span>restore ()](#apidoc.element.clam.hosts.restore)
- description and source-code
```javascript
restore = function () {
    var host = hostFile.get();
    var areaReg = new RegExp(beginTag+'[\\s\\S]*?'+endTag+'\\r?\\n?', 'g');
    host = host.replace(areaReg, '');
    hostFile.set(host);
}
```
- example usage
```shell
...
            };
        }

    })();
})();

//test
//NodeHostManager.restore();
exports = module.exports = NodeHostManager;
...
```

#### <a name="apidoc.element.clam.hosts.setHosts"></a>[function <span class="apidocSignatureSpan">clam.hosts.</span>setHosts (pro_hosts)](#apidoc.element.clam.hosts.setHosts)
- description and source-code
```javascript
setHosts = function (pro_hosts) {
    if(_.isString(pro_hosts)){
        pro_hosts = pro_hosts.split(/\n\r?/);
    }
    parse_host();
    lines.push(beginTag + split_char);
    pro_hosts.forEach(function (item, i) {
        var ip ;
        item = item.replace(/^\s+|\s+$/g, '');
        item = item.replace(/\s+/g, ' ');
        item = item.split(' ');
        if (ip_regx.test(item[0]) || ip6_regx.test[item[0]]) {
            ip = item[0];
            item.splice(0,1);
            item.forEach(function (_name, _i) {
                line_disable(_name);
            });
            lines.push(ip + ' ' + item.join(' ') + split_char);
        }
    });
    lines.push(endTag + split_char);

    hostFile.set(lines.join(''));
}
```
- example usage
```shell
...
  var dirs = prjDir.split(path.sep);
  prj.name = dirs[dirs.length - 1];
}


var oldPrj = config.get('project') || prj;
if (oldPrj.hosts && prj.hosts && oldPrj.hosts !== prj.hosts) {
  hostSwitch.setHosts(prj.hosts);
  actions.push({action: '更新hosts文件', content: '操作系统hosts文件'});
}
for (var k in prj) {
  oldPrj[k] = prj[k];
}

config.set('project', oldPrj);
...
```



# <a name="apidoc.module.clam.jsonHandle"></a>[module clam.jsonHandle](#apidoc.module.clam.jsonHandle)

#### <a name="apidoc.element.clam.jsonHandle.json"></a>[function <span class="apidocSignatureSpan">clam.jsonHandle.</span>json ()](#apidoc.element.clam.jsonHandle.json)
- description and source-code
```javascript
function jsonHandle() {
    return function (req, res, next) {
        var prjInfo = config.get('project');
        var url = req.url;
        if(url.indexOf('?') != -1){
            url = url.slice(0, url.indexOf('?'));
        }
        var isJson = false;
        var jsonHandles = prjInfo.json;
        if(!jsonHandles || jsonHandles.length === 0){
            next();
            return;
        }
        for(var i = 0; i < jsonHandles.length; i++){
            var map = jsonHandles[i];
            var re = new RegExp(map.url);
            if (url.match(re)) {
                isJson = true;
                if(map.enabled === 'local'){
                    //到本地找
                    var localFile = path.join(config.root(), '.clam/json', map.local);
                    var localHandle = require(localFile);
                    if(localHandle(req, res)){
                        return;
                    }
                }

                http.get({host:map.remote, port:80, path:req.url},function (resp) {
                    var buffs = [];
                    if (resp.statusCode !== 200) {
                        res.end('File ' + url + ' not found.');
                        return;
                    }
                    resp.on('data', function (chunk) {
                        buffs.push(chunk);
                    });
                    resp.on('end', function () {
                        var buff = joinbuffers(buffs);

                        //fix 80% situation bom problem.quick and dirty
                        if (buff[0] === 239 && buff[1] === 187 && buff[2] === 191) {
                            buff = buff.slice(3, buff.length);
                        }
                        res.setHeader("Content-Type", "text/html");
                        res.end(buff);
                    });
                }).on('error', function (e) {
                        debug(e);
                });
                break;
            }
        }
        if(!isJson){
            next();
        }
    }
}
```
- example usage
```shell
...
var plugBase = require("plug-base");
plugBase.root(basePath ? basePath : "src");
plugBase.config(config_dir);
plugBase
  .use(doji.PACHandle())
  .use(inspector)
  .use(dataApiHandle())
  .use(jsonHandle.json(prjInfo))
  .plug(require("flex-combo"), {filter:{
    '\\/\\$CLAM_VER\\$': ''
  }})
  .plug(require("essi"))
  .listen(port || ports[0] || 80, sport || ports[1] || 443);

var clamApp = plugBase.app;
...
```



# <a name="apidoc.module.clam.mocker"></a>[module clam.mocker](#apidoc.module.clam.mocker)

#### <a name="apidoc.element.clam.mocker.getMixedMockDate"></a>[function <span class="apidocSignatureSpan">clam.mocker.</span>getMixedMockDate (param, url, isRootPage)](#apidoc.element.clam.mocker.getMixedMockDate)
- description and source-code
```javascript
function getMixedMockDate(param, url, isRootPage){
    if(!param){
        param = {};
    }

    if(global){
        for(var prop in global){
            if(param[prop]){
                continue;
            }
            param[prop] = global[prop];
        }
    }
    param['_pageUrl'] = url;
    param['_pageBaseName'] = path.basename(url);
    if(!isRootPage){
        return param;
    }
    if(!ifDatas[url]){
        return param;
    }
    var urlData = ifDatas[url].response;
    if(urlData){
        for(var ifProp in urlData){
            if(param[ifProp]){
                continue;
            }
            param[ifProp] = urlData[ifProp];
        }
    }
    debug('页面最终内容%s',url, util.inspect(param));
    return param;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.mod"></a>[module clam.mod](#apidoc.module.clam.mod)

#### <a name="apidoc.element.clam.mod.add"></a>[function <span class="apidocSignatureSpan">clam.mod.</span>add (modName, description, template)](#apidoc.element.clam.mod.add)
- description and source-code
```javascript
add = function (modName, description, template) {
    var prjInfo = prj();
    var actions = [];

    //只支持几种扩展名，并且默认一个模块必须在子目录中
    var modFileName = computeExt(modName);
    if(modFileName.split('/').length === 1){
        var modNameSet = modFileName.replace(/\..*$/, '');
        modFileName = modNameSet + '/' + modFileName;
    }
    debug(modFileName);
    //如果存在相同模块报错
    var modFilePath = path.join(conf.root(), prjInfo.modsDir, modFileName);
    if (fs.existsSync(modFilePath)) {
        return {
            succeed: false,
            msg: '已存在相同的模块，创建模块失败。',
            data: modFilePath
        };;
    }

    //创建模块HTML文件目录
    var modDir = path.join(modFilePath, '..');
    mkdirp.sync(modDir);

    //修改目录权限为775
    var modDepsdirs = modFileName.split('/');
    var dir = '', j = 0;
    for(var i = 0; i < modDepsdirs.length-1; i++){
        dir = path.join(conf.root(), prjInfo.modsDir);
        j = 0;
        while(j <= i ){
            dir = path.join(dir, modDepsdirs[j]);
            j++;
        }
        debug('修改目录权限%s', dir);
        fs.chmodSync(dir,'775');
    }

    //取得模板路径
    if(!template){
        template = 'default';
    }
    var userHome = process.env.HOME || process.env.HOMEPATH;//兼容windows
    var templateDir = path.join(userHome, '.clamconfig/templates', template,'mod');
    if(!fs.existsSync(templateDir)){
        return {
            succeed: false,
            msg: '模板'+template+'不存在',
            data: ''
        };
    }

    //转换模板
    var bn = modDepsdirs[modDepsdirs.length-1];
    var baseModName = path.basename(bn, path.extname(bn));
    var modInfo = {
        name: baseModName,
        description: description
    };
    var param = {project: prjInfo, mod: modInfo};
    templateCenter.convert(templateDir, modDir, param, baseModName);

    //记录模块元信息
    var metaInfo = conf.get('mod');
    if(!metaInfo){
        metaInfo = {};
    }

    metaInfo[modFileName.replace(/\.(html)$/,'')] = modInfo;
    conf.set('mod', metaInfo);
    actions.push({action:'更新模块元信息', content: '.clam/mod.json'});

    //完成创建后执行回调
    return {
        succeed: true,
        msg: '模块创建',
        data: actions
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.mod.addCore"></a>[function <span class="apidocSignatureSpan">clam.mod.</span>addCore ()](#apidoc.element.clam.mod.addCore)
- description and source-code
```javascript
addCore = function (){
    var prjInfo = prj();
    var name = config.coreName;
    //添加核心模块
    addMod({
        name:name,
        description:"项目核心模块，包含一些不依赖任何库的JS方法和页头页尾等通用模块",
        addjs:true,
        addcss:true,
        jsns:prjInfo.jsns
    },{
        templateDir : config.coreTemplate
    });
    //添加头<head>内容模块
    addMod({
        name:name+"/head",
        description:"项目页面head标签部分内容",
        addjs:false,
        addcss:false
    },{
        templateDir : config.headTemplate
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.mod.del"></a>[function <span class="apidocSignatureSpan">clam.mod.</span>del (data)](#apidoc.element.clam.mod.del)
- description and source-code
```javascript
del = function (data) {
    var prjInfo = prj();
    var dirName = path.dirname(data.name);
    var fileName = path.basename(data.name);
    var modDir = path.join(conf.root(), prjInfo.modsDir, dirName);
    var modPath = path.join(conf.root(), prjInfo.modsDir, dirName, fileName+'.'+prjInfo.pageext[0]);
    var actions = [];
    if(!fs.existsSync(modPath)){
        return {
            succeed:false,
            msg:modPath+"文件不存在"
        }
    }
    //删除页面文件
    fs.unlinkSync(modPath);
    actions.push({action:'删除文件', content: modPath});
    //检查该文件夹下是否还有文件，如果没有的话就删掉
    var list = fs.readdirSync(modDir);
    list = _.filter(list,function(file){
        return _.any(config.suffix, function(value) {
            return file.lastIndexOf(value) !== -1;
        });
    });
    if(list.length==0){
        walk.rmrfSync(modDir);
        actions.push({action:'删除文件目录', content: modDir});
    }
    return {succeed:true,
        msg:'删除页面',
        data:actions
    };

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.mod.list"></a>[function <span class="apidocSignatureSpan">clam.mod.</span>list ()](#apidoc.element.clam.mod.list)
- description and source-code
```javascript
list = function () {
    var prjInfo = prj();

    var modsDir = path.join(conf.root(), prjInfo.modsDir);
    var metaFile = path.join(conf.root(), config.metaDir, config.metaFile);
    var modsFiles = walk.walkSync(modsDir);
    modsFiles = _.filter(modsFiles, function(file) {
        return _.any(config.suffix, function(value) {
            // 改为直接用后缀名判断，防止.vm.swp 这类文件混入
            var fileSuffix = file.match(/.*\/.*\.(\w+)$/)[1];
            return fileSuffix == value;
        });
    });
    //console.log(modsFiles);
    //conf.root() + prjInfo.dir
    var metaInfo = conf.get('mod');

    var info = _.map(modsFiles, function(file) {
        var fileName = file.slice(modsDir.length+1, file.length);
        var modName = file.slice(modsDir.length+1, file.lastIndexOf('.'));
        var description = '';
        if(metaInfo){
            description = metaInfo[modName] ? metaInfo[modName].description : '';
        }

        return {
            name : modName,
            file : fileName,
            description : description
        };
    });
    return {succeed:true,
        msg:'获取模块信息',
        data:info
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.page"></a>[module clam.page](#apidoc.module.clam.page)

#### <a name="apidoc.element.clam.page.add"></a>[function <span class="apidocSignatureSpan">clam.page.</span>add (name, url, description, template)](#apidoc.element.clam.page.add)
- description and source-code
```javascript
function add(name, url, description, template) {
    var prjInfo = conf.get('project');
    var root = conf.root();
    var metaFile = path.join(root, config.metaDir, config.metaFile);
    var actions = [];

    var pageFileName = computeExt(name);

<span class="apidocCodeCommentSpan">    /**
     * 处理单页页面目录和多层页面目录结构，单层结构的都加上
     */
</span>
    var pagePath = path.join(root, prjInfo.pagesDir, pageFileName);

    if (fs.existsSync(pagePath)) {
        return {succeed:false,
            msg:'存在相同的页面，创建页面失败。',
            data:pagePath
        };
    }
    console.log("Creating page:"+pagePath);

    //创建模块HTML文件目录
    var pageDir = path.join(pagePath, '..');
    mkdirp.sync(pageDir);

    //修改目录权限为775
    var pageDepsdirs = pageFileName.split('/');
    var dir = '', j=0;
    for(var i = 0; i < pageDepsdirs.length-1; i++){
        dir = path.join(conf.root(), prjInfo.pagesDir);
        j   = 0;
        while(j <= i ){
            dir = path.join(dir, pageDepsdirs[j]);
            j++;
        }
        debug('修改目录权限%s', dir);
        fs.chmodSync(dir,'775');
    }

    //取得模板路径
    if(!template){
        template = 'default';
    }
    var userHome = process.env.HOME || process.env.HOMEPATH;//兼容windows
    var templateDir = path.join(userHome, '.clamconfig/templates', template,'page');
    if(!fs.existsSync(templateDir)){
        return {
            succeed: false,
            msg: '模板'+template+'不存在',
            data: ''
        };
    }

    //转换模板
    var bn = pageDepsdirs[pageDepsdirs.length-1];
    var pageName = path.basename(bn, path.extname(bn));
    var pageInfo = {
        name: pageName,
        url: url,
        description: description
    };
    debug('变量信息:%s', util.inspect(pageInfo));
    var param = {project: prjInfo, page: pageInfo};
    templateCenter.convert(templateDir, pageDir, param, pageName);

    actions.push({action:'创建页面', content: pagePath});

    //记录page元信息
    var metaInfo = conf.get('page');
    if(!metaInfo){
        metaInfo = {};
    }

    metaInfo[pageFileName.replace(/\.(html)$/,'')] = pageInfo;
    conf.set('page', metaInfo);
    actions.push({action:'更新页面元信息', content: metaFile});

    return {
        succeed: true,
        msg: '创建页面',
        data: actions
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.page.del"></a>[function <span class="apidocSignatureSpan">clam.page.</span>del (data)](#apidoc.element.clam.page.del)
- description and source-code
```javascript
del = function (data) {
    var prjInfo = conf.get('project');
    var root = conf.root();
    var dirName = path.dirname(data.name);
    var fileName = path.basename(data.name);
    var pageDir = path.join(root, 'src', dirName);
    var pagePath = path.join(root, 'src', dirName, fileName + '.html');
    var actions = [];
    //删除页面文件
    fs.unlinkSync(pagePath);
    actions.push({action:'删除页面文件', content: pagePath});
    //检查该文件夹下是否还有文件，如果没有的话就删掉
    var list = fs.readdirSync(pageDir);
    if(list.length==0 && path.basename(pageDir) != path.basename('src')){
        fs.rmdirSync(pageDir);
        actions.push({action:'删除页面文件目录', content: pagePath});
    }
    return {succeed:true,
        msg:'删除页面',
        data:actions
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.page.list"></a>[function <span class="apidocSignatureSpan">clam.page.</span>list ()](#apidoc.element.clam.page.list)
- description and source-code
```javascript
list = function () {
    var prjInfo = conf.get('project');
    var root = conf.root();
    var pageDir = path.join(root, 'src');
    var metaFile = path.join(root, config.metaDir, config.metaFile);
    var pageFiles = walk.walkSync(pageDir);

    //过滤掉非html文件
    var filter_page = new RegExp(path.join(root, prjInfo.pagesDir).replace(/\\/g, '/')+".+\\.html$"),
        filter_root = new RegExp(path.join(root, prjInfo.pagesDir+"/..").replace(/\\/g, '/')+"/([^\/]*?)\\.html$");
    pageFiles = _.filter(pageFiles, function (file) {
        if (file.match(filter_page)) {
            return true;
        }
        else {
            return file.match(filter_root) ? true : false;
        }
    });
    debug('页面%s', util.inspect(pageFiles));
    pageFiles = pageFiles.sort(function (a, b) {
        return a < b;
    });
    var metaInfo = conf.get('page');
    var info = _.map(pageFiles, function (file) {
        var pageName = file.slice(pageDir.length+1, file.lastIndexOf('.'));
        var pageFileName = file.slice(pageDir.length+1, file.length);
        var description = '';
        var onlineurl = '';
        var pagelib = '';
        if(metaInfo){
            description = metaInfo[pageName] ? metaInfo[pageName].description : '';
            onlineurl = metaInfo[pageName] ? metaInfo[pageName].url : '';
            pagelib = metaInfo[pageName] ? metaInfo[pageName].lib : '';
        }

        return {
            name: pageName,
            file: pageFileName,
            description: description,
            url: onlineurl,
            lib: pagelib,
            fileExt: 'html'
        };
    });
    return {
        succeed:true,
        msg:'获取页面信息',
        data:info
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.page.update"></a>[function <span class="apidocSignatureSpan">clam.page.</span>update ()](#apidoc.element.clam.page.update)
- description and source-code
```javascript
update = function () {

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.project"></a>[module clam.project](#apidoc.module.clam.project)

#### <a name="apidoc.element.clam.project.project"></a>[function <span class="apidocSignatureSpan">clam.</span>project (prj)](#apidoc.element.clam.project.project)
- description and source-code
```javascript
project = function (prj) {
  prjDir = config.root();
  debug('项目目录:%s', prjDir);
  var state = prjState(prjDir);
  debug('项目状态:%s', state);
  if (!prj) {
    var info = getProject(prjDir, state);
    return info;
  }

  var actions = [];
  if (state !== 'normal') {
    if (state === 'blank') {
      var pagesFullDir = path.join(prjDir, initConf.pagesDir);
      mkdirp.sync(pagesFullDir);
      actions.push({action: '创建页面目录', content: pagesFullDir});

      var modsFullDir = path.join(prjDir, initConf.modsDir);
      mkdirp.sync(modsFullDir);
      actions.push({action: '创建模块目录', content: modsFullDir});

      var widgetsFullDir = path.join(prjDir, initConf.widgetsDir)
      mkdirp.sync(widgetsFullDir);
      actions.push({action: '创建组件目录', content: widgetsFullDir});

      var buildFullDir = path.join(prjDir, initConf.buildDir);
      mkdirp.sync(buildFullDir);
      actions.push({action: '创建构建目录', content: buildFullDir});

      var testsFullDir = path.join(prjDir, initConf.testsDir);
      mkdirp.sync(testsFullDir);
      actions.push({action: '创建测试目录', content: testsFullDir});
    }
    prj = initConf;
    var dirs = prjDir.split(path.sep);
    prj.name = dirs[dirs.length - 1];
  }


  var oldPrj = config.get('project') || prj;
  if (oldPrj.hosts && prj.hosts && oldPrj.hosts !== prj.hosts) {
    hostSwitch.setHosts(prj.hosts);
    actions.push({action: '更新hosts文件', content: '操作系统hosts文件'});
  }
  for (var k in prj) {
    oldPrj[k] = prj[k];
  }

  config.set('project', oldPrj);
  actions.push({action: '更新项目元文件', content: '.clam/project.json'});

  //getMuiConfig();
  //actions.push({action: '更新项目gconfig文件', content: '.clam/gconfig.json'});

  return {
    succeed: true,
    msg: '更新项目信息',
    data: actions
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.project.setUrls"></a>[function <span class="apidocSignatureSpan">clam.project.</span>setUrls (urls)](#apidoc.element.clam.project.setUrls)
- description and source-code
```javascript
setUrls = function (urls) {
  if (!urls) {
    return {
      succeed: false,
      msg: '更新项目信息',
      data: actions
    };
  }
  prjDir = config.root();
  var prj = config.get('project');
  prj.urls = urls;
  config.set('project', prj);
  config.set('project', prj);
  var actions = [];
  actions.push({action: '更新项目元文件', content: '.clam/project.json'});
  return {
    succeed: true,
    msg: '更新项目信息',
    data: actions
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.proxy"></a>[module clam.proxy](#apidoc.module.clam.proxy)

#### <a name="apidoc.element.clam.proxy.fetch"></a>[function <span class="apidocSignatureSpan">clam.proxy.</span>fetch (url, host, callback)](#apidoc.element.clam.proxy.fetch)
- description and source-code
```javascript
fetch = function (url, host, callback) {
    var filteredUrl = url,
        requestOption = {
            path: url,
            host: host,
            port: 80,
            agent: false
        };

    callback = typeof callback == "function" ? callback : function(code){console.log(code);};

    http.get(requestOption, function(resp) {
        var buffs = [];
        if (resp.statusCode !== 200) {
            var headerHost = requestOption.host;
            cosoleResp('Not found', requestOption.host + requestOption.path + ' (host:'+ reset + yellow + headerHost + reset + ')');
            callback('File ' + requestOption.host + requestOption.path + ' not found.', 404);
            return;
        }
        resp.on('data', function(chunk) {
            buffs.push(chunk);
        });
        resp.on('end', function() {
            var buff = joinbuffers(buffs);

            //fix 80% situation bom problem.quick and dirty
            if(buff[0] === 239 && buff[1] === 187 && buff[2] === 191) {
                buff = buff.slice(3, buff.length);
            }
            if(isBinFile(filteredUrl)){
                cosoleResp('Remote', requestOption.host + requestOption.path);
                callback(buff, 200);
                return;
            }
            cosoleResp('Remote', requestOption.host + requestOption.path);
            var charset = isUtf8(buff) ? 'utf8' : 'gbk';
            var outputCharset = prjInfo.charset[0];

            callback(adaptCharset(buff, outputCharset, charset), 200);
            return;
        });
    }).on('error',function() {
        callback('404 Error, File not found.', 404);
        return;
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.selectfile"></a>[module clam.selectfile](#apidoc.module.clam.selectfile)

#### <a name="apidoc.element.clam.selectfile.getTree"></a>[function <span class="apidocSignatureSpan">clam.selectfile.</span>getTree (root)](#apidoc.element.clam.selectfile.getTree)
- description and source-code
```javascript
function getTree(root) {
    var files = [];
    var fileItems;
    curDir = root?root:curDir;

    if (!fs.existsSync(curDir)) {
        throw "Can't find folder";
        return;
    }
    var stat = fs.statSync(curDir);

    if (stat.isDirectory()) {
        fileItems = fs.readdirSync(curDir);
        if(curDir!="/"){
            files.push({
                name : "..",
                path : path.join(curDir, ".."),
                icon : "icon-arrow-up",
                type : "folder"
            });
        }
        _.each(fileItems, function(name) {
            var p = path.join(curDir, name);
            var s = fs.statSync(p);
            var isD = s.isDirectory();
            var icon = isD ? "icon-folder-open" : "icon-file";
            var type = isD ? "folder" : "file";
            if(name.indexOf(".")==0)return;
            files.push({
                name : name,
                path : p,
                icon : icon,
                type : type
            });
        });
    }

    return {
        files:files,
        cur:curDir
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.clam.template"></a>[module clam.template](#apidoc.module.clam.template)

#### <a name="apidoc.element.clam.template.convert"></a>[function <span class="apidocSignatureSpan">clam.template.</span>convert (src, dest, param, destName)](#apidoc.element.clam.template.convert)
- description and source-code
```javascript
function convert(src, dest, param, destName){
    eachFile(src, function(file){
        var tmplContent = fs.readFileSync(file);

        //探测并转换文本内容编码
        var utf8 = isUtf8(tmplContent);
        if (utf8) {
            tmplContent = tmplContent.toString();
        }
        else {
            tmplContent = iconv.decode(tmplContent, 'gbk');
        }

        //模板处理引擎
        var pageContent = J(tmplContent, param);

        //复制到destDir并且处理编码问题
        var dir = path.dirname(file);
        var relative = path.relative(src, dir);
        var destDir = path.join(dest, relative);
        mkdirp.sync(destDir);
        destName = path.basename(destName);
        var destFilePath = path.basename(file).replace(/template(\..*)/, destName+'$1');
        destFilePath = path.join(destDir, destFilePath);
        var c = iconv.encode(pageContent,config.get('project').charset[0]);
        fs.writeFileSync(destFilePath, c);
        fs.chmodSync(destFilePath, "777");
    });
}
```
- example usage
```shell
...
var bn = modDepsdirs[modDepsdirs.length-1];
var baseModName = path.basename(bn, path.extname(bn));
var modInfo = {
    name: baseModName,
    description: description
};
var param = {project: prjInfo, mod: modInfo};
templateCenter.convert(templateDir, modDir, param, baseModName);

//记录模块元信息
var metaInfo = conf.get('mod');
if(!metaInfo){
    metaInfo = {};
}
...
```

#### <a name="apidoc.element.clam.template.init"></a>[function <span class="apidocSignatureSpan">clam.template.</span>init ()](#apidoc.element.clam.template.init)
- description and source-code
```javascript
function init(){
    var userHome = process.env.HOME || process.env.HOMEPATH;//兼容windows
    var cacheDir = path.join(userHome, '.clamconfig/templates/default');
    if(fs.existsSync(cacheDir)){
        return;
    }
    mkdirp.sync(cacheDir);
    var sourceRoot = path.join(__dirname,'../resource');
    function copyFn(file){
        debug('复制默认模板文件%s', path.basename(file));
        var dir = path.dirname(file);
        var relative = path.relative(sourceRoot, dir);
        var destDir = path.join(cacheDir, relative);
        mkdirp.sync(destDir);
        var srcFile = fs.readFileSync(file);
        var destFilePath = path.join(destDir, path.basename(file));
        fs.writeFileSync(destFilePath, srcFile);
    }
    eachFile(sourceRoot, copyFn);
}
```
- example usage
```shell
...
var template = require('./lib/template.js');
var mod = require('./lib/mod.js');
var page = require('./lib/page.js');
var widget = require('./lib/widget.js');

var clam = module.exports = {
    init: function(){
config.init();
template.init();
var ret = project({});

ret.data.forEach(function (ac) {
    debug(ac.action, ac.content);
});
process.exit(0);
...
```



# <a name="apidoc.module.clam.widget"></a>[module clam.widget](#apidoc.module.clam.widget)

#### <a name="apidoc.element.clam.widget.add"></a>[function <span class="apidocSignatureSpan">clam.widget.</span>add (widgetName, description, template)](#apidoc.element.clam.widget.add)
- description and source-code
```javascript
add = function (widgetName, description, template) {
    var prjInfo = prj();
    var actions = [];

    //如果存在相同模块报错
    var widgetDirPath = path.join(conf.root(), prjInfo.widgetsDir, widgetName);
    if (fs.existsSync(widgetDirPath)) {
        return {
            succeed: false,
            msg: '已存在相同的组件，创建模块失败。',
            data: widgetDirPath
        };
    }

    //创建模块HTML文件目录
    mkdirp.sync(widgetDirPath);

    //修改目录权限为775
    var widgetDepsdirs = widgetName.split('/');
    var dir = '', j = 0;
    for(var i = 0; i < widgetDepsdirs.length-1; i++){
        dir = path.join(conf.root(), prjInfo.widgetsDir);
        j = 0;
        while(j <= i ){
            dir = path.join(dir, widgetDepsdirs[j]);
            j++;
        }
        debug('修改目录权限%s', dir);
        fs.chmodSync(dir,'775');
    }

    //取得模板路径
    if(!template){
        template = 'default';
    }
    var userHome = process.env.HOME || process.env.HOMEPATH;//兼容windows
    var templateDir = path.join(userHome, '.clamconfig/templates', template, 'widget');
    if(!fs.existsSync(templateDir)){
        return {
            succeed: false,
            msg: '模板'+template+'不存在',
            data: ''
        };
    }

    //转换模板
    var widgetBaseName = path.basename(widgetName);
    var widgetInfo = {
        name: widgetBaseName,
        description: description
    };
    var param = {project: prjInfo, widget: widgetInfo};
    templateCenter.convert(templateDir, widgetDirPath, param, widgetBaseName);

    //记录模块元信息
    var metaInfo = conf.get('widget');
    if(!metaInfo){
        metaInfo = {};
    }

    metaInfo[widgetName] = widgetInfo;
    conf.set('widget', metaInfo);

    actions.push({action:'更新组件元信息', content: ''});

    //完成创建后执行回调
    return {
        succeed: true,
        msg: '组件创建',
        data: actions
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.widget.del"></a>[function <span class="apidocSignatureSpan">clam.widget.</span>del (data)](#apidoc.element.clam.widget.del)
- description and source-code
```javascript
del = function (data) {
    var prjInfo = prj();
    var dirName = data.name;
    var widgetDir = path.join(conf.root(), prjInfo.widgetsDir, dirName);
    var actions = [];
    if(!fs.existsSync(widgetDir)){
        return {
            succeed:false,
            msg:"文件不存在"
        }
    }
    //检查该文件夹下是否还有文件，如果没有的话就删掉
    walk.rmrfSync(widgetDir);
    actions.push({action:'删除文件目录', content: widgetDir});

    return {succeed:true,
        msg:'删除组件',
        data:actions
    };

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.clam.widget.list"></a>[function <span class="apidocSignatureSpan">clam.widget.</span>list ()](#apidoc.element.clam.widget.list)
- description and source-code
```javascript
list = function () {
    var prjInfo = prj();

    var widgetsDir = path.join(conf.root(), prjInfo.widgetsDir);
    var metaFile = path.join(conf.root(), config.metaDir, config.metaFile);
    var widgets = fs.readdirSync(widgetsDir);

    //获取widgets目录下所有文件夹
    widgets = _.filter(widgets, function(file) {
        return fs.statSync(path.join(widgetsDir,file)).isDirectory()
    });

    //console.log(widgets);


    //获取组件元数据
    var metaInfo = {};
    try {
        var metaStr = fs.readFileSync(metaFile);
        metaInfo = JSON.parse(metaStr);
    } catch(e) {
        metaInfo = {};
    }

    //console.log(metaInfo);

    //分析组件数据
    var info = _.map(widgets, function(widgetName) {
        var description = metaInfo[widgetName] ? metaInfo[widgetName].description : '';
        return {
            name : widgetName,
            description : description
        };
    });


    return {succeed:true,
        msg:'获取模块信息',
        data:info
    };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
