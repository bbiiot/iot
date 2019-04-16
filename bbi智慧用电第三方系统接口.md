> 本文档默认采用HTTP/HTTPS传输方式，JSON数据格式，UTF-8编码，
>推送数据类型分为3种任务数据，1种告警数据

# 附1：任务数据帧1
参数 | 类型 | 是否必填 | 描述 | 示例值
-|-|-|-|-
meterNo | String | 是 | 表号
sjsj | String | 是 | 数据时间
axdy | number | 是 |A相电压(V)
bxdy | number | 是 |B相电压(V)
cxdy | number | 是 |C相电压(V)
axdl | number | 是 |A相电流(A)
bxdl | number | 是 |B相电流(A)
cxdl | number | 是 |C相电流(A)
sydl | number | 是 |剩余电流(A)
zyggl | number | 是 |总有功功率(kW)
zglys | number | 是 |总功率因数

> 请求示例：
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "data" : {
                "axdy" : 220,
                "bxdy" : 220,
                "bxdy" : 220,
                 ...
                 // 其他附1所定义的...
                }
    }

# 附2：任务数据帧2
参数 | 类型 | 是否必填 | 描述 | 示例值
-|-|-|-|-
meterNo | String | 是 | 表号
sjsj | String | 是 | 数据时间
axwd | number | 是 |A相温度(℃)
bxwd | number | 是 |B相温度(℃)
cxwd | number | 是 |C相温度(℃)
lxwd | number | 是 |零线温度(℃)
hjwd | number | 是 |环境温度(℃)

> 请求示例：
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "data" : {
                "axwd" : 20,
                "axwd" : 20,
                "axwd" : 20,
                 ...
                 // 其他附2所定义的...
                }
    }
# 附3：日冻结数据
参数 | 类型 | 是否必填 | 描述 | 示例值
-|-|-|-|-
meterNo | String | 是 | 表号
sjsj | String | 是 | 数据时间
zxygzdl | number | 是 |正向有功总电量(kWh)
zxygzdl1 | number | 是 |正向有功费率1电量(kWh)
zxygzdl2 | number | 是 |正向有功费率2电量(kWh)
zxygzdl3 | number | 是 |正向有功费率3电量(kWh)
zxygzdl4 | number | 是 |正向有功费率3电量(kWh)

> 请求示例：
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "data" : {
                "zxygzdl" : 600,
                "zxygzdl1" : 100,
                "zxygzdl2" : 200,
                 ...
                 // 其他附2所定义的...
                }
    }
    
# 附4：告警数据 数据
参数 | 类型 | 是否必填 | 描述 | 示例值
-|-|-|-|-
meterNo | String | 是 | 表号
sjsj | String | 是 | 数据时间
code | String | 是 |告警编码 
data | Json | 否 |部分告警会带当前值

## data参数
参数 | 类型 | 是否必填 | 描述 | 示例值
-|-|-|-|-
axdy | number | 是 |A相电压(V)
bxdy | number | 是 |B相电压(V)
cxdy | number | 是 |C相电压(V)
axdl | number | 是 |A相电流(A)
bxdl | number | 是 |B相电流(A)
cxdl | number | 是 |C相电流(A)
sydl | number | 是 |剩余电流(A)
zyggl | number | 是 |总有功功率(kW)
zglys | number | 是 |总功率因数
axwd | number | 是 |A相温度(℃)
bxwd | number | 是 |B相温度(℃)
cxwd | number | 是 |C相温度(℃)
lxwd | number | 是 |零线温度(℃)
hjwd | number | 是 |环境温度(℃)

> 请求示例：
    
    {
        "meterNo" : "111800000490",
        "sjsj" : "2019-04-16 16:00:00",
        "code" : "10001",
        "data" : {
                "axdy" : 600,
                "bxdy" : 100,
                "cxdy" : 200,
                 ...
                 // 其他data参数所定义的...
                }
    }
      