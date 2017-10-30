# CoocaaVR 手柄SDK

## SDK使用注意事项：

跳转场景的时候需要调以下代码重置下角度
AndroidServiceControllerProvider.ResetRightYawRotation();
AndroidServiceControllerProvider.ResetLeftYawRotation();

同步的话在跳转语句后面调用；
异步的话需要判断下加载的进度，在进度大于0.9的时候调；（因为跳转场景有回中操作,所以手柄也要有对应的处理）
