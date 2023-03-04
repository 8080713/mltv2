# Box
感谢开源的大佬们，感谢宝盒！（所有资源代码均来自大佬们的辛苦付出,本仓只收集整理测试）

提交始于 takagen99_20230227-2248

=== 源代码-编辑应用程序默认设置 ===

/src/main/java/com/github/tvbox/osc/base/App.java

    private void initParams() {

        putDefault(HawkConfig.HOME_REC, 0);       // Home Rec 0=豆瓣, 1=推荐, 2=历史
        putDefault(HawkConfig.PLAY_TYPE, 1);      // Player   0=系统, 1=IJK, 2=Exo
        putDefault(HawkConfig.IJK_CODEC, "硬解码");// IJK Render 软解码, 硬解码
        putDefault(HawkConfig.HOME_SHOW_SOURCE, true);  // true=Show, false=Not show
        putDefault(HawkConfig.HOME_NUM, 2);       // History Number
        putDefault(HawkConfig.DOH_URL, 2);        // DNS
        putDefault(HawkConfig.SEARCH_VIEW, 2);    // Text or Picture

    }

=== 设置配置地址 ===
- 线路或多仓地址 > 输入源URL地址（支持多仓）
- 数据源 > 输入源名称 & 输入源URL地址
- 直播 (Optional) > 输入Live URL（http）地址.如果为空,将从源文件获取Live URL,
- EPG (Optional) > 输入EPG URL（http）地址.如果为空,将从源文件中获取EPG URL,
- 默认EPG > default from http://epg.51zmt.top:8000/api/diyp/