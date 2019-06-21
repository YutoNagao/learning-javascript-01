# learning-javascript-01

テクノロジー（藤原）JavaScriptの練習 (1)  

## Q1の回答「コメントを解除したことで、どう変化しましたか？」

ダイアログボックスに「こんにちは！」と表示された。  

## Q2の回答「エラーの原因は何でしょうか？（調べてみましょう）」

ReferenceError→関数が定義されていない状態  
window is not defined→ウィンドウが定義されていない  
エラーの原因はwindows.aleartを実行するウィンドウがないこと

## Chromeデベロッパーツール：Consoleの実行結果

```
VM13 contentScript.bundle.js:36 [CS]  start
index.html:18 おはよう！
index.html:56 Live reload enabled.
VM13 contentScript.bundle.js:259 [CS] [DpScriptPageHandle] enter
VM13 contentScript.bundle.js:274 [CS] wait for document ready to inject script
VM13 contentScript.bundle.js:204 [CS] [injectScript] enter
VM13 contentScript.bundle.js:191 [CS] [createScoutScriptElement] enter
contentScript.bundle.js:36 [CS]  start
contentScript.bundle.js:278 [CS] [ExtensionFrameHandle] enter
contentScript.bundle.js:292 [CS] wait for extension frame ready to inject div
contentScript.bundle.js:176 [CS] [injectDiv] enter
contentScript.bundle.js:137 [CS] [afterInjectDiv] enter
VM13 contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:71 [CS] [extensionFrameMessageHandler] enter
contentScript.bundle.js:73 [CS] [extensionFrameMessageHandler] relay message:  Object
VM13 contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:36 [CS]  start
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
VM34 contentScript.bundle.js:36 [CS]  start
Navigated to http://127.0.0.1:5500/index.html
VM34 contentScript.bundle.js:259 [CS] [DpScriptPageHandle] enter
VM34 contentScript.bundle.js:274 [CS] wait for document ready to inject script
index.html:18 おはよう！
VM34 contentScript.bundle.js:204 [CS] [injectScript] enter
VM34 contentScript.bundle.js:191 [CS] [createScoutScriptElement] enter
contentScript.bundle.js:36 [CS]  start
contentScript.bundle.js:278 [CS] [ExtensionFrameHandle] enter
contentScript.bundle.js:292 [CS] wait for extension frame ready to inject div
contentScript.bundle.js:176 [CS] [injectDiv] enter
contentScript.bundle.js:137 [CS] [afterInjectDiv] enter
VM34 contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:71 [CS] [extensionFrameMessageHandler] enter
contentScript.bundle.js:73 [CS] [extensionFrameMessageHandler] relay message:  {messageObject: {…}}
VM34 contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:36 [CS]  start
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
index.html:52 [Intervention] Blocked attempt to show a 'beforeunload' confirmation panel for a frame that never had a user gesture since its load. https://www.chromestatus.com/feature/5082396709879808
socket.onmessage @ index.html:52
contentScript.bundle.js:36 [CS]  start
Navigated to http://127.0.0.1:5500/index.html
contentScript.bundle.js:259 [CS] [DpScriptPageHandle] enter
contentScript.bundle.js:274 [CS] wait for document ready to inject script
index.html:18 おはよう！
contentScript.bundle.js:204 [CS] [injectScript] enter
contentScript.bundle.js:191 [CS] [createScoutScriptElement] enter
contentScript.bundle.js:36 [CS]  start
contentScript.bundle.js:278 [CS] [ExtensionFrameHandle] enter
contentScript.bundle.js:292 [CS] wait for extension frame ready to inject div
contentScript.bundle.js:176 [CS] [injectDiv] enter
contentScript.bundle.js:137 [CS] [afterInjectDiv] enter
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:71 [CS] [extensionFrameMessageHandler] enter
contentScript.bundle.js:73 [CS] [extensionFrameMessageHandler] relay message:  {messageObject: {…}}
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:45 [CS] onMessageHandler start with id extensionMessagingForPostingToExtensionFrame
contentScript.bundle.js:36 [CS]  start
```

## ターミナルの実行結果

```
You have new mail.
MacBook-Pro-2:~ yutonagao$ cd fujiwara
MacBook-Pro-2:fujiwara yutonagao$ git clone git@github.com:YutoNagao/learning-javascript-01.git
Cloning into 'learning-javascript-01'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 10 (delta 0), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (10/10), done.
MacBook-Pro-2:fujiwara yutonagao$ cd learning-javascript-01/
MacBook-Pro-2:learning-javascript-01 yutonagao$ code .
MacBook-Pro-2:learning-javascript-01 yutonagao$ node node-main.js
/Users/yutonagao/Documents/fujiwara/learning-javascript-01/node-main.js:1
window.alert("Hello, Node.js!!");
^

ReferenceError: window is not defined
    at Object.<anonymous> (/Users/yutonagao/Documents/fujiwara/learning-javascript-01/node-main.js:1:1)
    at Module._compile (internal/modules/cjs/loader.js:774:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
    at Module.load (internal/modules/cjs/loader.js:641:32)
    at Function.Module._load (internal/modules/cjs/loader.js:556:12)
    at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
    at internal/main/run_main_module.js:17:11
MacBook-Pro-2:learning-javascript-01 yutonagao$ node node-main.js
Goodmorning, Node.js!!

```

