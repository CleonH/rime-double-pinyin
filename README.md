# 雙拼

配方： ℞ **double-pinyin**

[Rime](https://rime.im) 雙拼輸入方案

已收錄以下雙拼方案：

  - 自然碼雙拼
  - 智能ABC雙拼
  - 小鶴雙拼
  - MSPY雙拼
  - 拼音加加雙拼

## 安裝

本方案依賴於

  - [朙月拼音](https://github.com/rime/rime-luna-pinyin) ℞ **`luna-pinyin`**

[東風破](https://github.com/rime/plum) 安裝口令： `bash rime-install double-pinyin`

授權條款：見 [LICENSE](LICENSE)


## 个人设定 - 双拼

微软双拼 default.custom.yaml

词库引用 double_pinyin_mspy.my.dict.yaml

（简易方法：引用luna_pinyin，深蓝转化词库文本，直接导入luna_pinyin)


### 导入搜狗词库
1 下载搜狗标准词库 https://pinyin.sogou.com/dict/detail/index/11640
2 下载深蓝词库转换 https://github.com/studyzy/imewlconverter
3 转化成功保存txt本地即可
4 复制txt文件到Rime 配置目录下，并重命名 sg-ciku1.dict.yaml 然后打开在最上面添加
```
---
name: sg-ciku1
version: "1.0"
sort: by_weight
use_preset_vocabulary: true
...
```
5 打开luna_pinyin.my.dict.yaml ，import_tables增加搜狗词库
```
import_table:
 - sg-ciku1
```
