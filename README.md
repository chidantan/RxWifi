# RxWifi
基于RX 2.x的wifi操作库
## 功能
- 扫描wifi；
- 开关wifi；
- 显示wifi列表；
- 显示wifi强度；
- 连接wifi。
## 代码示例
在onResume开始扫描，循环得到扫描结果：

        wifiProcessInterface.startScan()
                .subscribe(new Consumer<List<WifiEntity>>() {
                    @Override
                    public void accept(List<WifiEntity> wifiEntities) throws Exception {
			//循环得到wifi列表
                        //todo 得到wifi列表，下面是自己的业务逻辑         
                    }
                });

在onPause结束扫描

	wifiProcessInterface.stopScan();
## 成果展示
![](https://i.imgur.com/Hc1B78b.jpg)
