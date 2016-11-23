# VaryViewHepler
切换不同布局的帮助类

# 初始化helper
```java
mVaryViewHelper = new VaryViewHelper.Builder()
                .setDataView(findViewById(R.id.vary_content))
                .setLoadingView(LayoutInflater.from(this).inflate(R.layout.layout_loadingview,null))
                .setEmptyView(LayoutInflater.from(this).inflate(R.layout.layout_emptyview, null))
                .setErrorView(LayoutInflater.from(this).inflate(R.layout.layout_errorview,null))
                .setRefreshListener(new ErrorClickListener())
                .build() ;
```
# 切换不同的布局
```java
mVaryViewHelper.showDataView();                
mVaryViewHelper.showEmptyView();
mVaryViewHelper.showErrorView();
mVaryViewHelper.showLoadingView();
```
![image](https://github.com/corerzhang/VaryViewHepler/blob/master/screenshot/device-2015-10-18-160712.png?raw=true)
![image](https://github.com/corerzhang/VaryViewHepler/blob/master/screenshot/device-2015-10-18-160829.png?raw=true)
