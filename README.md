# Error when opening the Overlay

``` dtrace
--------- beginning of crash
12-29 16:23:38.406 12192 12192 E AndroidRuntime: FATAL EXCEPTION: main
12-29 16:23:38.406 12192 12192 E AndroidRuntime: Process: com.androidcrashonoverlayopen, PID: 12192
12-29 16:23:38.406 12192 12192 E AndroidRuntime: java.lang.IndexOutOfBoundsException: Index: 3, Size: 3
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at java.util.ArrayList.get(ArrayList.java:437)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.bridge.JavaOnlyArray.getDouble(JavaOnlyArray.java:91)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.RenderableView.setupPaint(RenderableView.java:487)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.RenderableView.setupFillPaint(RenderableView.java:435)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.RenderableView.draw(RenderableView.java:373)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.RenderableView.render(RenderableView.java:339)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.GroupView.drawGroup(GroupView.java:104)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.GroupView.draw(GroupView.java:81)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.RenderableView.render(RenderableView.java:339)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.SvgView.drawChildren(SvgView.java:304)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.SvgView.drawOutput(SvgView.java:255)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.horcrux.svg.SvgView.onDraw(SvgView.java:106)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23901)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23773)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23904)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.widget.ScrollView.draw(ScrollView.java:2876)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.scroll.ReactScrollView.draw(ReactScrollView.java:519)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23773)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.views.view.ReactViewGroup.dispatchDraw(ReactViewGroup.java:743)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23904)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23773)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.facebook.react.ReactRootView.dispatchDraw(ReactRootView.java:223)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23771)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.drawChild(ViewGroup.java:5336)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewGroup.dispatchDraw(ViewGroup.java:5093)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.View.draw(View.java:23904)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at eightbitlab.com.blurview.BlockingBlurController.updateBlur(BlockingBlurController.java:122)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at eightbitlab.com.blurview.BlockingBlurController$1.onPreDraw(BlockingBlurController.java:56)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewTreeObserver.dispatchOnPreDraw(ViewTreeObserver.java:1124)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewRootImpl.performTraversals(ViewRootImpl.java:3854)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewRootImpl.doTraversal(ViewRootImpl.java:2618)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.ViewRootImpl$TraversalRunnable.run(ViewRootImpl.java:9971)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.Choreographer$CallbackRecord.run(Choreographer.java:1010)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.Choreographer.doCallbacks(Choreographer.java:809)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.Choreographer.doFrame(Choreographer.java:744)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.view.Choreographer$FrameDisplayEventReceiver.run(Choreographer.java:995)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.os.Handler.handleCallback(Handler.java:938)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.os.Handler.dispatchMessage(Handler.java:99)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.os.Looper.loop(Looper.java:246)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at android.app.ActivityThread.main(ActivityThread.java:8633)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at java.lang.reflect.Method.invoke(Native Method)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:602)
12-29 16:23:38.406 12192 12192 E AndroidRuntime: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1130)
```
