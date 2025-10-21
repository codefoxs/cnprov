# cnprov
Stata commands for Chinese province name standardization.

## Install

```stata
* Latest version
cap ado uninstall cnprov
net install cnprov, from("https://raw.githubusercontent.com/codefoxs/cnprov/main/") replace

* Old version
cap ado uninstall cnprov
net install cnprov, from("https://raw.githubusercontent.com/codefoxs/cnprov/v#.#.#/") replace
```

## Example

### Standardization

1 Name standardization

    "北京市"           <-   "北京|Beijing|beijing"
    "天津市"           <-   "天津|Tianjin|tianjin"
    "河北省"           <-   "河北|Hebei|hebei"
    "山西省"           <-   "山西|Shanxi|shanxi"
    "内蒙古自治区"     <-   "内蒙|Mongolia|Neimeng|neimeng"
    "辽宁省"           <-   "辽宁|Liaoning|liaoning"
    "吉林省"           <-   "吉林|Jilin|jilin"
    "黑龙江省"         <-   "黑龙|Heilong|heilongjiang"
    "上海市"           <-   "上海|Shanghai|shanghai"
    "江苏省"           <-   "江苏|Jiangsu|jiangsu"
    "浙江省"           <-   "浙江|Zhejiang|zhejiang"
    "安徽省"           <-   "安徽|Anhui|anhui"
    "福建省"           <-   "福建|Fujian|fujian"
    "江西省"           <-   "江西|Jiangxi|jiangxi"
    "山东省"           <-   "山东|Shandong|shandong"
    "河南省"           <-   "河南|Henan|henan"
    "湖北省"           <-   "湖北|Hubei|hubei"
    "湖南省"           <-   "湖南|Hunan|hunan"
    "广东省"           <-   "广东|Guangdong|guangdong"
    "广西壮族自治区"   <-   "广西|Guangxi|guangxi"
    "海南省"           <-   "海南|Hainan|hainan"
    "重庆市"           <-   "重庆|Chongqing|chongqing"
    "四川省"           <-   "四川|Sichuan|sichuan"
    "贵州省"           <-   "贵州|Guizhou|guizhou"
    "云南省"           <-   "云南|Yunnan|yunnan"
    "西藏自治区"       <-   "西藏|Xizang|Tibet|xizang|tibet"
    "陕西省"           <-   "陕西|Shaanxi|shaanxi"
    "甘肃省"           <-   "甘肃|Gansu|gansu"
    "青海省"           <-   "青海|Qinghai|qinghai"
    "宁夏回族自治区"   <-   "宁夏|Ningxia|ningxia"
    "新疆维吾尔自治区" <-   "新疆|Xinjiang|xinjiang"
    "台湾省"           <-   "台湾|Taiwan|taiwan"
    "香港特别行政区"   <-   "香港|Hong Kong|xianggang|hongkong|hong kong|HongKong"
    "澳门特别行政区"   <-   "澳门|Macau|macau|aomen|Aomen"

 2 Code standardization

    110000             <-   "北京|Beijing|beijing"
    120000             <-   "天津|Tianjin|tianjin"
    130000             <-   "河北|Hebei|hebei"
    140000             <-   "山西|Shanxi|shanxi"
    150000             <-   "内蒙|Mongolia|Neimeng|neimeng"
    210000             <-   "辽宁|Liaoning|liaoning"
    220000             <-   "吉林|Jilin|jilin"
    230000             <-   "黑龙|Heilong|heilongjiang"
    310000             <-   "上海|Shanghai|shanghai"
    320000             <-   "江苏|Jiangsu|jiangsu"
    330000             <-   "浙江|Zhejiang|zhejiang"
    340000             <-   "安徽|Anhui|anhui"
    350000             <-   "福建|Fujian|fujian"
    360000             <-   "江西|Jiangxi|jiangxi"
    370000             <-   "山东|Shandong|shandong"
    410000             <-   "河南|Henan|henan"
    420000             <-   "湖北|Hubei|hubei"
    430000             <-   "湖南|Hunan|hunan"
    440000             <-   "广东|Guangdong|guangdong"
    450000             <-   "广西|Guangxi|guangxi"
    460000             <-   "海南|Hainan|hainan"
    500000             <-   "重庆|Chongqing|chongqing"
    510000             <-   "四川|Sichuan|sichuan"
    520000             <-   "贵州|Guizhou|guizhou"
    530000             <-   "云南|Yunnan|yunnan"
    540000             <-   "西藏|Xizang|Tibet|xizang|tibet"
    610000             <-   "陕西|Shaanxi|shaanxi"
    620000             <-   "甘肃|Gansu|gansu"
    630000             <-   "青海|Qinghai|qinghai"
    640000             <-   "宁夏|Ningxia|ningxia"
    650000             <-   "新疆|Xinjiang|xinjiang"
    810000             <-   "台湾|Taiwan|taiwan"
    820000             <-   "香港|Hong Kong|xianggang|hongkong|hong kong|HongKong"
    710000             <-   "澳门|Macau|macau|aomen|Aomen"

## Example

### Quick use

```stata
cnprov province
```

### Name the generated variables

```stata
cnprov province, name(new_prov)
```

