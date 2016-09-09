接口说明
=============

&copy; 相江 方文浩


## - Card 相关接口

- ### 卡片查询接口

- ###### 功能说明：根据日期查询
    *   Content-Type: application/json
    *   请求方式：HTTP POST
    *   Path：[domain]/metis/article/card/findByPage.shtml

- ######  请求元素 

| 参数名    |   类型   | 描述 |  是否必须 |
| :-------: |  :----:  | :--: |  :-----:  |
| startTime | Date     | 起始时间，默认当前 |  no    |
| endTime   | Date     | 截止时间，默认当前 |  no    |

- ######  响应元素示例
``` JSON
{
    "status": 200,
    "msg": "success",
    "data": [
        {
            "pageNumber": 0,
            "pageSize": 0,
            "status": 1,
            "operatorId": 999,
            "validTime": 1456848000000,
            "invalidTime": null,
            "updateTime": 1454342400000,
            "createTime": 1451664000000,
            "id": 1,
            "imgUrl": "http://pic23.nipic.com/20120917/10076134_112929387108_2.jpg",
            "desc": "black colorful",
            "sid": null,
            "linkUrl": null,
            "linkType": 1,
            "dailyTime": "2016-07-02",
            "publishTime": null,
            "online": true,
            "validTimeStr": "2016-03-02 00:00:00",
            "invalidTimeStr": "",
            "updateTimeStr": "2016-02-02 00:00:00",
            "createTimeStr": "2016-01-02"
        },
        {
            "pageNumber": 0,
            "pageSize": 0,
            "status": 1,
            "operatorId": 999,
            "validTime": 1473317381000,
            "invalidTime": null,
            "updateTime": 1473317381000,
            "createTime": 1473317381000,
            "id": 2,
            "imgUrl": null,
            "desc": null,
            "sid": "5hceqrjl7od4",
            "linkUrl": null,
            "linkType": 1,
            "dailyTime": "2016-08-21",
            "publishTime": 1473317381000,
            "online": true,
            "validTimeStr": "2016-09-08 14:49:41",
            "invalidTimeStr": "",
            "updateTimeStr": "2016-09-08 14:49:41",
            "createTimeStr": "2016-09-08"
        },
        {
            "pageNumber": 0,
            "pageSize": 0,
            "status": 1,
            "operatorId": 999,
            "validTime": null,
            "invalidTime": null,
            "updateTime": 1473318395000,
            "createTime": 1473317948000,
            "id": 5,
            "imgUrl": "http://www.pptbz.com/pptpic/UploadFiles_6909/201206/2012060823384357.jpg",
            "desc": null,
            "sid": "5hceqrjl7od4",
            "linkUrl": null,
            "linkType": 2,
            "dailyTime": "2016-08-21",
            "publishTime": 1473318395000,
            "online": true,
            "validTimeStr": "",
            "invalidTimeStr": "",
            "updateTimeStr": "2016-09-08 15:06:35",
            "createTimeStr": "2016-09-08"
        }  
    ]
}
```

- ### 卡片更新接口

- ###### 功能说明：根据卡片ID确定更新记录
    *   Content-Type: application/json
    *   请求方式：HTTP POST
    *   Path：[domain]/metis/article/card/saveOrUpdate.shtml

- ######  请求元素 

| 参数名    |   类型   | 描述 |  是否必须 |
| :-------: |  :----:  | :--: |  :-----:  |
| id          | int      | 卡片ID               |  yes   |

- ######  响应元素示例
``` JSON
{
    "status": 200,
    "msg": "success",
    "data": null
}
```

## - Banner 相关接口

- ### Banner查询接口

- ###### 功能说明：查询所有记录
    *   Content-Type: application/json
    *   请求方式：HTTP POST
    *   Path：[domain]/metis/article/banner/findByPage.shtml

- ######  请求元素 

| 参数名    |   类型   | 描述 |  是否必须 |
| :-------: |  :----:  | :--: |  :-----:  |
| null | null | 无 |  null |

- ######  响应元素示例
``` JSON
{
    "status": 200,
    "msg": "success",
    "data": [
        {
            "pageNumber": 0,
            "pageSize": 0,
            "status": 1,
            "operatorId": 999,
            "validTime": 1473320855000,
            "invalidTime": null,
            "updateTime": 1473320855000,
            "createTime": 1473320855000,
            "id": 1,
            "imgUrl": "http://img3.imgtn.bdimg.com/it/u=2163251846,48390253&fm=21&gp=0.jpg",
            "position": 4,
            "title": null,
            "sid": "5hceqrjl7od4",
            "linkUrl": null,
            "linkType": 0,
            "publishTime": 1473322112000,
            "online": true,
            "validTimeStr": "2016-09-08 15:47:35",
            "invalidTimeStr": "",
            "updateTimeStr": "2016-09-08 15:47:35",
            "createTimeStr": "2016-09-08"
        },
        {
            "pageNumber": 0,
            "pageSize": 0,
            "status": 1,
            "operatorId": 999,
            "validTime": 1473320998000,
            "invalidTime": null,
            "updateTime": 1473323657000,
            "createTime": 1473320998000,
            "id": 2,
            "imgUrl": "http://pic23.nipic.com/20120917/10076134_112929387108_2.jpg",
            "position": 2,
            "title": null,
            "sid": "5hceqrjl7od4",
            "linkUrl": null,
            "linkType": 0,
            "publishTime": 1473320998000,
            "online": true,
            "validTimeStr": "2016-09-08 15:49:58",
            "invalidTimeStr": "",
            "updateTimeStr": "2016-09-08 16:34:17",
            "createTimeStr": "2016-09-08"
        }
    ]
}
```

- ### Banner各字段更新接口

- ###### 功能说明：根据ID确定更新记录
    *   Content-Type: application/json
    *   请求方式：HTTP POST
    *   Path：[domain]/metis/article/banner/saveOrUpdate.shtml

- ######  请求元素 

| 参数名    |   类型   | 描述 |  是否必须 |
| :-------: |  :----:  | :--: |  :-----:  |
| id          | int      | 横幅广告(Banner) ID   |  yes   |

- ######  响应元素示例

``` JSON
{
    "status": 200,
    "msg": "success",
    "data": null
}
```

- ### Banner位置字段更新接口

- ###### 功能说明：根据ID和位置列表确定更新Banner记录的位置字段
    *   Content-Type: application/json
    *   请求方式：HTTP POST
    *   Path：[domain]/metis/article/banner/updateBanners.shtml

- ######  请求元素 

| 参数名    |   类型   | 描述 |  是否必须 |
| :-------: |  :----:  | :--: |  :-----:  |
| ids         | List<Integer>      | 横幅广告(Banner)ID列表   |  yes   |
| positions   | List<Integer>      | Banner对应的需求位置列表 |  yes   |

- ######  响应元素示例

``` JSON
{
    "status": 200,
    "msg": "success",
    "data": null
}
```
