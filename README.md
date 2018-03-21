# CrossDomain


## 第一步

- 将项目git clone到自己的电脑上
- 将开源项目里面的common文件夹拷贝在个人项目需要跨域的thinkphp的application文件夹下

## 第二步

- 修改个人个人项目thinkphp的application文件夹下tags.php
- 修改里面代码：

``` return [
    // 应用初始化
    'app_init'     => [],
    // 应用开始
    'app_begin'    => [
        'app\\common\\behavior\\CronRun'
    ],
    // 模块初始化
    'module_init'  => [],
    // 操作开始执行
    'action_begin' => [],
    // 视图内容过滤
    'view_filter'  => [],
    // 日志写入
    'log_write'    => [],
    // 应用结束
    'app_end'      => [
        'app\\common\\behavior\\CronRun'
    ],
]; ```