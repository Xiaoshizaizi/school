### 仓库说明
* school.js为国内（含台湾）按照省份排列的大学列表。数据类型实例如下：
``` javascript
      test: [
        {
          id: 1,//省份ID
          text: "北京市",//省份或直辖市
          children: [//当前省份下的所有学校
            {
              id: 10000,//学校id
              text: "北京大学"//学校名称
            },
            {
              ......
            }
          ]
        },
        {
          id: 2,
          text: "xx省",
          children: [
            {
              id: 20000,
              name: "xxx大学"
            }
          ]
        }
      ]
```
### 使用说明
* 将school.js保存在自己的项目中
``` javascript
import obj from "path/school";//export default,import对象名任意

```
### 改造json
* 若要改造为json文件仅需将school.js文件中第一行的 const obj = 删掉最后一行的export default obj 删掉，文件重命名为.json即可。
### PR
* 不定时更新,若学校信息有变更，欢迎PR
