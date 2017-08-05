
studentManage接口文档
---------------------------


修改记录：
| 序号   | 修改日期       | 修该目录号                           | 修改说明                                     |
| ---- | ---------- | ------------------------------- | ---------------------------------------- |
| 50   | 2016.12.14 | 2.7.3 查看某人主页                    | 修正错误，返回值增加t_count                        |
| 50   | 2016.12.05 | 5.6.13 删除帖子                     | 新增                                       |
| 49   | 2016.11.27 | 2.7.0 获取短信验证码                   | 修改接口：返回值增加sms字段                          |
| 48   | 2016.11.27 | 2.7.1 用户登录                      | 返回值friendList去掉                          |
| 47   | 2016.11.26 | 2.3.5 获取笔记详情，及评价列表              | 返回值新增字段ifSc                              |
| 46   | 2016.11.26 | 2.5.3  获取新闻详情                   | 返回值新增字段ifSc                              |
| 45   | 2016.11.24 | 2.7.24 根据user_id，获取帖子评论列表       | 新增接口                                     |
| 44   | 2016.11.24 | 2.7.25 根据user_id，获取帖子点赞列表       | 新增接口                                     |
| 43   | 2016.11.21 | 2.8.12 取消收藏                     | 新增                                       |
| 42   | 2016.11.21 | 2.8.13 取消关注                     | 新增                                       |
| 41   | 2016.11.21 | 2.8.14 取消点赞                     | 新增                                       |
| 40   | 2016.11.19 | 2.7.1 用户登录                      | 修改。icon返回完整路径                            |
| 39   | 2016.11.19 | 2.6.2 获取热门社区列表                  | 修改。返回值增加字段if_g                           |
| 38   | 2016.11.19 | 2.6.1 获取社区列表                    | 修改。返回值增加字段if_g                           |
| 37   | 2016.11.14 | 2.1.4 获取课程详情，及章节列表              | 修改。返回值courseitemList增加字段course_shared_page_url |
| 36   | 2016.11.14 | 2.7.23 根据账号，获取用户信息              | 新增。根据account list，获取user list            |
| 35   | 2016.11.13 | 2.1.2 评论对象                      | type=post,对接IM消息提醒                       |
| 34   | 2016.11.13 | 2.8.2 点赞对象                      | type= post/comment,对接IM消息提醒              |
| 33   | 2016.11.13 | 2.8.4 关注对象                      | type=user时，对接IM消息提醒                      |
| 32   | 2016.11.13 | 2.7.1 用户登录                      | 返回值增加friendList列表                        |
| 31   | 2016.11.08 | 2.6.5 获取帖子详情，及评论列表              | 修改"ifFocus"返回错误                          |
| 30   | 2016.11.07 | 2.7.0 获取短信验证码                   | 获取验证码接口                                  |
| 29   | 2016.11.07 | 2.7.2 用户注册                      | 输入参数增加字段：code（短信验证码）                     |
| 28   | 2016.11.02 | 2.7.3 查看某人主页                    | 修改"ifFocus"返回错误                          |
| 27   | 2016.11.01 | 2.7.22 获取群组所有成员                 | 对接im                                     |
| 26   | 2016.11.01 | 2.7.21 获取一个用户参与的所有群组            | 对接im                                     |
| 25   | 2016.11.01 | 2.7.20 移除群组成员[单个]               | 对接im                                     |
| 24   | 2016.11.01 | 2.7.19 添加群组成员[单个]               | 对接im                                     |
| 23   | 2016.11.01 | 2.7.18 删除一个群组                   | 对接im                                     |
| 22   | 2016.11.01 | 2.7.17 修改一个群组                   | 对接im                                     |
| 21   | 2016.11.01 | 2.7.16 创建一个群组                   | 对接im                                     |
| 20   | 2016.11.01 | 2.8.13 取消关注社区/用户/新闻栏目           | 对接im                                     |
| 19   | 2016.11.01 | 2.8.4 关注对象                      | 对接im                                     |
| 1    | 2016.11.01 | 2.7.2 用户注册                      | 对接im                                     |
| 18   | 2016.10.30 | 2.8.13 取消关注社区/用户/新闻栏目           | 新增接口                                     |
| 17   | 2016.10.27 | 2.8.10 获取我的错题的科目列表              | 返回值专业及科目列表增加字段t_count                    |
| 16   | 2016.10.27 | 2.8.12 取消收藏错题                   | 新增接口                                     |
| 15   | 2016.10.26 | 2.5.5 获取新闻详情，及评价列表              | 返回值增加评论数量pCount                          |
| 14   | 2016.10.26 | 2.5.3 获取新闻详情                    | 返回值增加评论数量pCount                          |
| 13   | 2016.10.25 | 2.8.10 获取我的错题的科目列表              | 返回树级专业列表和科目列表                            |
| 12   | 2016.10.25 | 2.7.4 修改用户信息                    | 解决报错问题，修改信息后，返回用户所有信息                    |
| 11   | 2016.10.23 | 2.8. 1评论对象                      | 参数及返回值无改动。解决报错“缺少参数”                     |
| 10   | 2016.10.23 | 2.7.3 修改用户信息                    | 参数及返回值无改动。                               |
| 9    | 2016.10.23 | 2.6.6 发帖                        | images分隔符修改为0x01。multiparty代替formidable，字符分割符使用0x01代替逗号 |
| 8    | 2016.10.19 | 2.6.5 获取帖子详情，及评论列表              | 添加字段isFocused（当前登陆用户是否关注发帖用户）            |
| 7    | 2016.10.17 | 2.7.3 修改用户信息                    | 解决修改用户信息，未提交的字段被置空的问题                    |
| 6    | 2016.10.16 | 2.4.3 获取资源列表                    | 返回列表添加shared_page_url字段                  |
| 5    | 2016.10.16 | 2.4.4 根据科目ID，获取资源列表，含收藏量，评论量，分页 | 返回列表添加shared_page_url字段                  |
| 4    | 2016.10.16 | 2.4.5 获取资源详情                    | 返回列表添加shared_page_url字段                  |
| 3    | 2016.10.16 | 2.8.6 用户错题后调用，保存错题              | 解决：收藏试题后不能加入我的错题，提示不能重复操作                |
| 2    | 2016.10.16 | 2.8.10 获取我的错题的科目列表              | 解决：查询我的错题科目列表错误，不含有科目名称，数据中包含其他类别的数据     |
| 1    | 2016.10.16 | 2.8.3 收藏对象                      | 解决：加入错题可以重复提交，插入相通的数据                    |






<a name="21"></a>
### 2.1 课程相关
* [1.1.1 获取课程专业列表](#211)
* [1.1.2 获取课程列表](#212)
* [1.1.3 获取课程列表，分页，评论量，点赞量，模糊查询](#213)
* [1.1.4 获取课程详情，及章节列表](#214)
* [1.1.5 获取视频详情，课程评价](#215)
* [1.1.6 收藏课程（略，见通用接口：2.8.3 收藏对象）](#288)
* [1.1.7 点赞课程（略，见通用接口：2.8.2 点赞对象）](#282)
* [1.1.8 评价课程（略，见通用接口：2.8. 1评论对象）](#281)
* [1.1.9 课程分享后调用（略，见通用接口：2.8.5 用户分享后调用，增加积分）](#285)
* [1.1.10 根据课程ID，获取评论列表（略，见通用接口：2.8.7 根据对象ID，获取评论列表）](#287)
      <a name="22"></a>
### 2.2 题库相关

* [2.2.1 获取试卷专业列表](#221)
* [2.2.2 获取试卷科目列表](#222)
* [2.2.3 获取试卷列表](#223)
* [2.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询](#224)
* [2.2.5 获取试卷详情，及试题列表](#225)
* [2.2.6 收藏试卷（略，见通用接口：2.8.3 收藏对象）](#283)
* [2.2.7 点赞试卷（略，见通用接口：2.8.2 点赞对象）](#282)
* [2.2.8 评价试题（略，见通用接口：2.8. 1评论对象）](#281)
* [2.2.9 获取试题评价列表（略，见通用接口）](#287)
* [2.2.10 评价试卷（略，见通用接口：2.8. 1评论对象）](#281)
* [2.2.11 收藏试题（略，见通用接口：2.8.3 收藏对象）](#283)
* [2.2.12 根据试卷ID，获取评论列表（略，见通用接口：2.8.9 根据对象ID，获取评论列表）](#287)

  <a name="23"></a>
### 2.3 笔记相关

*  [2.3.1 获取笔记专业列表](#231)
*  [2.3.2 获取笔记科目列表](#232) 
*  [2.3.3 获取笔记列表](#233)
*  [2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询](#234)
*  [2.3.5 获取笔记详情，及评价列表](#235)
*  [2.3.6 收藏笔记（略，见通用接口：2.8.3 收藏对象）](#283)
*  [2.3.7 点赞笔记（略，见通用接口：2.8.2 点赞对象）](#282)
*  [2.3.8 评价笔记（略，见通用接口：2.8. 1评论对象）](#281)
*  [2.3.9 笔记分享（略，见通用接口：2.8.5 用户分享后调用，增加积分）](#285)
*  [2.3.10 根据笔记ID，获取评论列表（略，见通用接口：2.8.9 根据对象ID，获取评论列表）](#2310)
           <a name="24"></a>
### 2.4 资源相关

*  [2.4.1 获取资源专业列表](#241)
*  [2.4.2 获取资源科目列表](#242)
*  [2.4.3 获取资源列表](#243)
*  [2.4.4 获取资源列表，含收藏量，评论量，分页](#244)
*  [2.4.5 获取资源详情](#245)
*  [2.4.6 收藏资源（略，见通用接口：2.8.3 收藏对象）](#246)
*  [2.4.7 点赞资源（略，见通用接口：2.8.2 点赞对象）](#247)
*  [2.4.8 评论资源（略，见通用接口：2.8. 1评论对象）](#248)
*  [2.4.9 资源分享（略，见通用接口：2.8.5 用户分享后调用，增加积分）](#249)
*  [2.4.10 根据资源ID，获取评论列表（略，见通用接口：2.8.9 根据对象ID，获取评论列表）](#2410)

<a name="25"></a>
### 2.5 新闻相关
* [2.5.1 获取新闻标签列表](#251)
* [2.5.2 获取新闻列表](#252)
* [2.5.3 获取新闻详情](#253)
* [2.5.4 获取新闻评论列表](#254)
* [2.5.5 获取新闻详情，及评价列表](#255)
* [2.5.6 添加订阅（略，见通用接口：2.8.4 关注对象）](#256)
* [2.5.7 收藏新闻（略，见通用接口：2.8.3 收藏对象）](#257)
* [2.5.8 点赞新闻（略，见通用接口：2.8.2 点赞对象）](#258)
* [2.5.9 评价新闻（略，见通用接口：2.8. 1评论对象）](#259)
* [2.5.10 新闻分享（略，见通用接口：2.8.5 用户分享后调用，增加积分）](#2510)
* [1.1.11 根据新闻ID，获取评论列表（略，见通用接口：2.8.9 根据对象ID，获取评论列表）](#2511)

<a name="26"></a>
### 2.6 社区相关
* [2.6.1 获取社区列表](#261)
* [2.6.2 获取热门社区列表（用户未关注的）](#262)
* [2.6.3 获取社区详情，及帖子列表](#263)
* [2.6.4 获取帖子列表](#264)
* [2.6.5 获取帖子详情，及评论列表](#265)
* [2.6.6 发帖](#266)
* [2.6.7 获取精选帖列表](#267)
* [2.6.8 根据社区id，获取置顶贴列表](# 268)
* [2.6.8 关注社区（略，见通用接口：2.8.4 关注对象）](#269)
* [2.6.9 点赞帖子（略，见通用接口：2.8.2 点赞对象）](#2610)
* [2.6.10 评论帖子（略，见通用接口：2.8. 1评论对象）](#2611)
* [2.6.11 帖子分享（略，见通用接口：2.8.5 用户分享后调用，增加积分）](#2612)
* [2.6.12 根据帖子ID，获取评论列表（略，见通用接口：2.8.9 根据对象ID，获取评论列表）](#2613)
* [5.6.13 删除帖子](#2613)

<a name="27"></a>
### 2.7 用户相关
* [2.7.0 获取短信验证码](#270)
* [2.7.01 验证短信验证码](#2701)
* [2.7.1 用户登录](#271)
* [2.7.2 用户注册](#272)
* [2.7.3 查看某人主页](#273)
* [2.7.3 修改用户信息](#274)
* [2.7.4 获取我收藏的课程（略，见通用接口：2.8.10 获取我收藏的xxx）](#288)
* [2.7.5 获取我收藏的试卷（略，见通用接口：2.8.10 获取我收藏的xxx）](#288)
* [2.7.6 获取我收藏的笔记（略，见通用接口：2.8.10 获取我收藏的xxx）](#288)
* [2.7.7 获取我收藏的新闻（略，见通用接口：2.8.10 获取我收藏的xxx）](#288)
* [2.7.8 获取我的错题的科目列表（略，见通用接口：获取我的错题的科目列表）](#279)
* [2.7.8 获取我的错题（略，见通用接口：2.8.10 获取我的错题列表）](#2710)
* [2.7.9 获取我关注的社区（略，见通用接口：2.8.11 获取我关注的xxx ）](#2711)
* [2.7.10 获取我关注的新闻标签（略，见通用接口：2.8.11 获取我关注的xxx ）](#2712)
* [2.7.11 获取我关注的用户（略，见通用接口：2.8.11 获取我关注的xxx ）](#2713)
* [2.7.12 关注用户（略，见通用接口：2.8.4 关注对象）](#2714)
* [2.7.13 提交错题，错题后调用（略，见通用接口：2.8.6 用户错题后调用，保存错题）](#2715)
* [2.7.16 创建一个群组](#2716)
* [2.7.17 修改一个群组](#2717)
* [2.7.18 删除一个群组](#2718)
* [2.7.19 添加群组成员[单个] ](#2719)
* [2.7.20 移除群组成员[单个]](#2720)
* [2.7.21 获取用户参与的所有群组](#2721)
* [2.7.22 获取群组所有成员](#2722)
* [2.7.23 根据账号，获取用户信息](#2723)
* [2.7.24 根据user_id，获取帖子评论列表](#2723)
* [2.7.25 根据user_id，获取帖子点赞列表](#2723)




  <a name="28"></a>
### 2.8 通用接口

* [2.8.1 评论对象](#281)
* [2.8.2 点赞对象](#282)
* [2.8.3 收藏对象](#283)
* [2.8.4 关注对象](#284)
* [2.8.5 用户分享后调用，增加积分](#285)
* [2.8.6 用户错题后调用，保存错题](#286)
* [2.8.7 根据对象ID，获取评论列表](#287)
* [2.8.8 获取我收藏的xxx](#288)
* [2.8.9 获取我关注的xxx](#289)
* [2.8.10 获取我的错题的科目列表](#2810)
* [2.8.11 获取我的错题列表](#2811)
* [2.8.12 取消收藏](#2812)
* [2.8.13 取消关注](#2813)
* [2.8.14 取消点赞](#2814)

<a name="29"></a>
### 2.9 H5界面
* [第1章  h5界面](#h5界面)
  *  [1. 视频详情及评论列表页](#291)
  *  [2. 笔记详情及评论列表页](#292)
  *  [3. 新闻详情及评论列表页](#293)
  *  [4. 帖子详情及评论列表页](#294)


  <a name="21"></a>
### 2.1 课程相关

  <a name="211"></a>
#### 2.1.1 获取课程专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=course_major

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=course_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
   {
      "id": 35,
      "type_id": "5558e310-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=1822233235,2188182299&fm=21&gp=0.jpg",
      "name": "中医专业",
      "type": "course_major",
      "parent_id": "",
      "parent_name": "",
      "order": 3,
      "createdAt": "2016-01-17T09:18:55.000Z",
      "updatedAt": "2016-09-17T10:09:33.000Z",
      "child_count": null
    },
    ...
  ]
}
```
  <a name="212"></a>
#### 2.1.2 获取课程列表
##### 接口地址：/studentManage/api/course/getAll
##### 方法：get
参数：
- keyword：关键字

请求实例：http://120.25.124.68:4000/studentManage/api/course/getAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
     {
      "id": 5,
      "course_id": "9b25b220-c443-11e5-b7b8-9b9bf580f0d3",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "生理学",
      "icon": "http://120.25.124.68:4000/upload/image/报告解读科.png",
      "icon_size": null,
      "brief": "本课程为四川大学生理学精品课程教学视频，全套视频共计63讲。\n　  生理学是生物科学的一个分支，是以生物机体的生命活动现象和机体各个组成部分的功能为研究对象的一门学科。人体生理学的任务是研究构成人体各个系统的器官、 组织和细胞的正常活动过程；生理功能的内部机制；不同细胞、组织、器官、系统间的相互联系和相互作用；并阐明人体作为一个整体，其各部分功能活动如何相互协调、相互制约，从而能在复杂多变的环境中维持正常的生命活动。生理学又是一门重要的基础医学课程。学生只有在首先了解人体正常功能活动的基础上，才能理解各种",
      "datems": "1453819366579",
      "createdAt": "2016-01-26T15:43:54.000Z",
      "updatedAt": "2016-10-06T12:23:42.000Z"
    },
    ...
  ],
  "count": 2
}
```
  <a name="213"></a>
#### 2.1.3 获取课程列表，分页，评论量，点赞量，模糊查询
##### 接口地址：/studentManage/api/course/list
##### 方法：get
参数：
- major_id：专业id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：http://120.25.124.68:4000/studentManage/api/course/list?major_id=2d92b270-bcfb-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
   {
      "id": 20,
      "course_id": "38d2e8e0-8bd5-11e6-9225-a1b20c908ec9",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "病理学",
      "icon": "http://120.25.124.68:4000/upload/image/QQ图片20161006225655.png",
      "icon_size": null,
      "brief": "本课程为吉林大学病理学精品课程教学视频，全套视频共51集，视频源自搜狐视频。\n  病理学是用自然科学的方法研究疾病发生、发展和转化规律，从而阐明疾病本质的医学科学，它不仅作为基础理论科学为临床医学科学奠定坚实的基础，而且又作为应用科学直接参与临床实践。它以基础医学中的解剖学、组织胚胎学、生理学、生物化学、细胞生物学、分子生物学、微生物学和免疫学等为基础，探讨疾病发生发展过程中机体的功能代谢和形态结构的变化，以及与临床的联系。病理学是一门由基础医学跨入临床医学的“桥梁”学科，不仅在整个医学和医学教育中具有承",
      "datems": "1475765857902",
      "createdAt": "2016-10-06T14:57:37.000Z",
      "updatedAt": "2016-10-06T14:57:37.000Z",
      "c_count": 51,
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    ...
  ]
}
```
  <a name="214"></a>
#### 2.1.4 获取课程详情，及章节列表
##### 接口地址：/studentManage/api/course/getOne
##### 方法：get
参数：
- user_id：当前登录用户id
- courseid：课程id

请求实例：http://120.25.124.68:4000/studentManage/api/course/getOne?course_id=04328410-3711-11e6-ab7b-4b13ffcc5cad&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "ifDz": "yes",  //是否点赞
  "ifSc": "yes",  //是否收藏
  "item": {
    "id": 18,
    "course_id": "04328410-3711-11e6-ab7b-4b13ffcc5cad",
    "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "title": "生理学",
    "icon": "http://120.25.124.68:3010/image/30c40e020f63f81f-85679ec6a342f6f1-06a07df456c24a947beb67b8c2f8d51d.jpg",
    "brief": "生理学基础视听课程",
    "datems": "1466445690577",
    "createdAt": "2016-06-20T18:01:30.000Z",
    "updatedAt": "2016-06-20T18:01:30.000Z",
    "s_count": 1,
    "d_count": 1,
    "p_count": null
  },
  "courseitemList": [
    {
      "id": 20,
      "courseitem_id": "0805e050-3ebe-11e6-ab7b-4b13ffcc5cad",
      "parent_id": "04328410-3711-11e6-ab7b-4b13ffcc5cad",
      "parent_name": "",
      "title": "搜狐视频",
      "src": "http://tv.sohu.com/upload/static/share/share_play.html#63786587_146116868_0_9001_0",
      "from": "1",
      "video_page_url": "http://120.25.124.68:4000/studentManage/mobile/player?courseitem_id=0805e050-3ebe-11e6-ab7b-4b13ffcc5cad",
      "brief": "搜狐视频测试使用",
      "datems": "1467289658069",
      "createdAt": "2016-06-30T12:27:38.000Z",
      "updatedAt": "2016-09-14T04:51:54.000Z"
    },
   ...
  ]
}
```




  <a name="215"></a>
#### 2.1.5 获取视频详情，课程评价
##### 接口地址：/studentManage/api/courseitem/getOne
##### 方法：get
参数：
- courseid：课程id

请求实例：http://120.25.124.68:4000/studentManage/api/courseitem/getOne?courseitem_id=5f3850f0-bd14-11e5-ace2-11edb9ad68d4

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "courseitem": {
    "id": 12,
    "courseitem_id": "5f3850f0-bd14-11e5-ace2-11edb9ad68d4",
    "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
    "parent_name": "基础医学实验(甲) 陆源 全7讲 浙江大学",
    "title": "第一章 概率",
    "src": "http://120.25.124.68:4000/upload/video/mv1.mp4",
    "src_size": null,
    "from": "0",
    "video_page_url": null,
    "brief": "基础医学课程介绍,基础医学课程介绍 ！",
    "datems": "1453032994594",
    "createdAt": "2016-01-17T12:18:09.000Z",
    "updatedAt": "2016-01-17T12:38:16.000Z",
    "course_shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/course?courseitem_id=5f3850f0-bd14-11e5-ace2-11edb9ad68d4"
  },
   "commentlist": [
    {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "user_name": "wayne",
      "user_account": "18521508353",
      "user_icon": "http://120.25.124.68:4000/upload/image/user_icon_14775547330002983headicon_1477554733712.png",
      "id": 310,
      "comment_id": "7ea58410-9ff1-11e6-9104-75040b4a2b6e",
      "parent_id": "03e52070-9d24-11e6-adb5-1b908bf34c48",
      "parent_type": "post",
      "content": "都冷啊",
      "datems": "1477977024209",
      "createdAt": "2016-11-01T05:10:24.000Z",
      "updatedAt": "2016-11-01T05:10:24.000Z",
      "d_count": null,
      "p_count": null
    }
  ]
}
```

  <a name="22"></a>
### 2.2 题库相关

  <a name="221"></a>
#### 2.2.1 获取试卷专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=exam_major

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=exam_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
  {
      "id": 36,
      "type_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "order": 2,
      "createdAt": "2016-01-17T09:19:54.000Z",
      "updatedAt": "2016-01-27T11:38:44.000Z",
      "child_count": 4
    },
    ...
  ]
}
```
  <a name="222"></a>
#### 2.2.2 获取试卷科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
type=exam_subject
parent_id

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=exam_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
     {
      "id": 45,
      "type_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "药理学",
      "type": "exam_subject",
      "parent_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "order": 1,
      "createdAt": "2016-01-17T09:26:38.000Z",
      "updatedAt": "2016-01-26T15:34:09.000Z",
      "child_count": null
    },
    ...
  ]
}
```
  <a name="223"></a>
#### 2.2.3 获取试卷列表
##### 接口地址：/studentManage/api/exam/findAll
##### 方法：get
参数：
- keyword：关键字

请求实例：http://120.25.124.68:4000/studentManage/api/exam/findAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 11,
      "exam_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "major_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "subject_name": "药理学",
      "icon": null,
      "name": "[药物代谢动力学]",
      "brief": "药理学特色课程",
      "level": null,
      "datems": "1453014632009",
      "createdAt": "2016-01-17T11:53:07.000Z",
      "updatedAt": "2016-01-17T11:53:07.000Z",
      "s_count": null,  //收藏量
      "d_count": null,  //点赞量
      "p_count": null   //评论量
    },
    {
      "id": 12,
      "exam_id": "6dea1280-bd9d-11e5-b900-59869364e3c1",
      "major_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "subject_name": "药理学",
      "icon": null,
      "name": "医学基础知识试题",
      "brief": "百度文库",
      "level": null,
      "datems": "1453091743664",
      "createdAt": "2016-01-18T04:39:15.000Z",
      "updatedAt": "2016-01-18T04:39:15.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
  <a name="224"></a>
#### 2.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询
##### 接口地址：/studentManage/api/exam/list
##### 方法：get
参数：
- subject_id：科目id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：http://120.25.124.68:4000/studentManage/api/exam/list?subject_id=69265b10-bcfc-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 11,
      "exam_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "major_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "subject_name": "药理学",
      "icon": null,
      "name": "[药物代谢动力学]",
      "brief": "药理学特色课程",
      "level": null,
      "datems": "1453014632009",
      "createdAt": "2016-01-17T11:53:07.000Z",
      "updatedAt": "2016-01-17T11:53:07.000Z",
      "s_count": null,  //收藏量
      "d_count": null,  //点赞量
      "p_count": null   //评论量
    },
    {
      "id": 12,
      "exam_id": "6dea1280-bd9d-11e5-b900-59869364e3c1",
      "major_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "subject_name": "药理学",
      "icon": null,
      "name": "医学基础知识试题",
      "brief": "百度文库",
      "level": null,
      "datems": "1453091743664",
      "createdAt": "2016-01-18T04:39:15.000Z",
      "updatedAt": "2016-01-18T04:39:15.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
  <a name="225"></a>
#### 2.2.5 获取试卷详情，及试题列表
##### 接口地址：/studentManage/api/exam/getOne
##### 方法：get
参数：
- exam_id：试卷id

请求实例：http://120.25.124.68:4000/studentManage/api/exam/getOne?exam_id=df8a5720-bd10-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "item": {
    "id": 13,
    "exam_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
    "major_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "subject_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
    "subject_name": "药理学",
    "icon": null,
    "name": "绪论",
    "brief": "绪论",
    "level": null,
    "datems": "1453630457581",
    "createdAt": "2016-01-24T15:38:45.000Z",
    "updatedAt": "2016-02-29T11:44:17.000Z",
    "s_count": null,
    "d_count": null,
    "p_count": null
  },
  "examitemList": [
    {
      "id": 40,
      "examitem_id": "fd0435e0-361a-11e6-a2b5-d34754e75c61",
      "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
      "parent_name": "绪论",
      "type": "2",
      "content": "作为面试官招聘前端开发人员的提问准备",
      "answer": "1.你的简历中罗列了许多你曾经参与过的项目，你能说说你其中你觉得最好的项目么？你所使用的技术，担任的角色？最让你自豪的是哪一点？(如果没有项目，请罗列自己学过哪些内容，最擅长哪些内容？)★★★\r\n提问理由：个人简历中一般都会罗列很多参与过的项目，通过讨论其最自豪的项目可以了解此人的角色、擅长点和自我期望。如果没有项目则至少应该提出学过哪些内容（例如那些自学的或是培训班出来的），否则难以证明此人有足够的经验胜任。\r\n2.我们搞技术的人，总是要面临不断学习的问题。请问你最近看的技术类论坛或者牛人博客是什么？有",
      "analysis": "（略）详见答案",
      "selects": "[{\"$$hashKey\":\"003\",\"answer\":false}]",
      "datems": "1466340022334",
      "createdAt": "2016-06-19T12:40:22.000Z",
      "updatedAt": "2016-06-19T12:40:22.000Z"
    },
    {
      "id": 39,
      "examitem_id": "c864c2e0-3602-11e6-a2b5-d34754e75c61",
      "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
      "parent_name": "绪论",
      "type": "1",
      "content": "你有几只小狗？",
      "answer": "三只，两只金毛，一只牧羊犬。",
      "analysis": "根据自己的实际情况回答即可。",
      "selects": "[{\"$$hashKey\":\"003\",\"answer\":false}]",
      "datems": "1466329626126",
      "createdAt": "2016-06-19T09:47:06.000Z",
      "updatedAt": "2016-06-19T09:47:06.000Z"
    },
    {
      "id": 38,
      "examitem_id": "2c26f7b0-3600-11e6-a2b5-d34754e75c61",
      "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
      "parent_name": "绪论",
      "type": "0",
      "content": "你有几只狗？",
      "answer": "B",
      "analysis": "根据自己的实际情况回答",
      "selects": "[{\"$$hashKey\":\"003\",\"answer\":false,\"question\":\"1\"},{\"$$hashKey\":\"01L\",\"answer\":true,\"question\":\"2\"},{\"$$hashKey\":\"01N\",\"answer\":false,\"question\":\"3\"}]",
      "datems": "1466328505004",
      "createdAt": "2016-06-19T09:28:25.000Z",
      "updatedAt": "2016-06-19T09:28:25.000Z"
    },
    {
      "id": 42,
      "examitem_id": "9cb989b0-361f-11e6-a2b5-d34754e75c61",
      "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
      "parent_name": "绪论",
      "type": "0",
      "content": "你毕业于哪个学校？",
      "answer": "A,C",
      "analysis": "根据自己的实际情况回答啊",
      "selects": "[{\"$$hashKey\":\"003\",\"answer\":true,\"question\":\"东北大学\"},{\"$$hashKey\":\"01L\",\"answer\":false,\"question\":\"北京大学\"},{\"$$hashKey\":\"01N\",\"answer\":true,\"question\":\"南京大学\"}]",
      "datems": "1466342008267",
      "createdAt": "2016-06-19T13:13:28.000Z",
      "updatedAt": "2016-06-19T13:13:28.000Z"
    }
  ],
  "examitem": {
    "id": 39,
    "examitem_id": "c864c2e0-3602-11e6-a2b5-d34754e75c61",
    "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
    "parent_name": "绪论",
    "type": "1",
    "content": "你有几只小狗？",
    "answer": "三只，两只金毛，一只牧羊犬。",
    "analysis": "根据自己的实际情况回答即可。",
    "selects": "[{\"$$hashKey\":\"003\",\"answer\":false}]",
    "datems": "1466329626126",
    "createdAt": "2016-06-19T09:47:06.000Z",
    "updatedAt": "2016-06-19T09:47:06.000Z"
  }
}
```



  <a name="23"></a>
### 2.3 笔记相关

  <a name="231"></a>
#### 2.3.1 获取笔记专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=note_major

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=note_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 41,
      "type_id": "af739930-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=3041013660,671874781&fm=21&gp=0.jpg",
      "name": "临床医学",
      "type": "note_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:21:27.000Z",
      "updatedAt": "2016-01-17T09:21:27.000Z"
    },
    {
      "id": 40,
      "type_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "note_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:21:13.000Z",
      "updatedAt": "2016-01-17T09:21:13.000Z"
    }
  ]
}
```
<a name="232"></a>
#### 2.3.2 获取笔记科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=note_subject

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=note_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 53,
      "type_id": "2858a130-bd18-11e5-ace2-11edb9ad68d4",
      "icon": "http://120.25.124.68:4000/upload/image/u=585329176,2311950479&fm=206&gp=0.jpg",
      "name": "[生理学]",
      "type": "note_subject",
      "parent_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "order": 1,
      "createdAt": "2016-01-17T12:45:15.000Z",
      "updatedAt": "2016-01-17T12:45:15.000Z",
      "child_count": null
    },
    ...
  ]
}
```
<a name="233"></a>
#### 2.3.3 获取笔记列表
##### 接口地址：/studentManage/api/note/getAll
##### 方法：get
参数：
- keyword：关键字

请求实例：http://120.25.124.68:4000/studentManage/api/note/getAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 1,
      "level": 1,
      "note_id": "1",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "笔记",
      "content": "笔记内容",
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:29:29.000Z",
      "updatedAt": "2016-01-17T14:39:03.000Z"
    },
    {
      "id": 2,
      "level": null,
      "note_id": "3",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "笔记1",
      "content": "笔记内容1",
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:30:08.000Z",
      "updatedAt": "2016-01-16T09:30:11.000Z"
    },
    {
      "id": 4,
      "level": 1,
      "note_id": "d46a28e0-bd18-11e5-ace2-11edb9ad68d4",
      "major_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "2858a130-bd18-11e5-ace2-11edb9ad68d4",
      "subject_name": "[生理学]",
      "title": "中医基础理论 ",
      "content": "<p>\r\n<div>第一单元 中医学理论体系的主要特点<br>\r\n<br>\r\n细目一：整体观念<br>\r\n<br>\r\n1、整体观念的概念：整体观念是中医学关于人体自身的完整性及人与自然、社会环境的统<br>\r\n<br>\r\n一性的认识。<br>\r\n<br>\r\n2、整体观念的内容：1.人体是一个有机整体。<br>\r\n<br>\r\n2.人与自然环境的统一性。<br>\r\n<br>\r\n3.人与社会环境的统一性。<br>\t<a target=\"_blank\" rel=\"nofollow\" href=\"http://ww",
      "datems": "1453032994594",
      "createdAt": "2016-01-17T12:50:04.000Z",
      "updatedAt": "2016-01-17T14:39:07.000Z"
    }
  ]
}
```
<a name="234"></a>
#### 2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询
##### 接口地址：/studentManage/api/note/list
##### 方法：get
参数：
- keyword：关键字；
- subject_id：科目id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：http://120.25.124.68:4000/studentManage/api/note/list?subject_id=9039a280-a71b-11e5-b779-99d7f151235d

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 1,
      "level": 1,
      "note_id": "1",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "笔记",
      "content": "笔记内容",
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:29:29.000Z",
      "updatedAt": "2016-01-17T14:39:03.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 2,
      "level": null,
      "note_id": "3",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "笔记1",
      "content": "笔记内容1",
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:30:08.000Z",
      "updatedAt": "2016-01-16T09:30:11.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
<a name="235"></a>
#### 2.3.5 获取笔记详情，及评价列表
##### 接口地址：/studentManage/api/note/getOne
##### 方法：get
参数：
- note_id：笔记id
- user_id：登陆用户ID

请求实例：http://120.25.124.68:4000/studentManage/api/note/getOne?note_id=ca5fbf90-e13f-11e5-8e43-8bea282120fc&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "ifDz": "yes",  //是否点赞
  "ifSc": "yes",  //是否收藏
  "item": {
    "id": 2,
    "level": 0,
    "note_id": "95ffed70-9f70-11e6-9c4f-f55d3e6be065",
    "major_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "subject_id": "2858a130-bd18-11e5-ace2-11edb9ad68d4",
    "subject_name": "[生理学]",
    "title": " 慢性支气管炎和阻塞性肺气肿 ",
    "content": "<p>...</p>",
    "datems": "1477921658311",
    "createdAt": "2016-10-31T13:47:38.000Z",
    "updatedAt": "2016-11-25T01:49:32.000Z",
    "s_count": 1,
    "d_count": 1,
    "p_count": 4,
    "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/note?note_id=95ffed70-9f70-11e6-9c4f-f55d3e6be065"
  },
  "commentlist": [
    {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "user_name": "小明",
      "user_account": "18521508353",
      "user_icon": "http://120.25.124.68:4000/upload/image/user_icon_14791470360003070headicon_1479147028321.png",
      "id": 446,
      "comment_id": "54dd75b0-b389-11e6-938b-812bb1e65230",
      "parent_id": "95ffed70-9f70-11e6-9c4f-f55d3e6be065",
      "parent_type": "note",
      "content": "fdd",
      "datems": "1480131309708",
      "createdAt": "2016-11-26T03:35:09.000Z",
      "updatedAt": "2016-11-26T03:35:09.000Z",
      "d_count": null,
      "p_count": null
    },
    ...
  ]
}
```


  <a name="24"></a>
### 2.4 资源相关

<a name="241"></a>
#### 2.4.1 获取资源专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=resource_major

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=resource_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
     {
      "id": 49,
      "type_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "resource_major",
      "parent_id": "",
      "parent_name": "",
      "order": 1,
      "createdAt": "2016-01-17T09:31:07.000Z",
      "updatedAt": "2016-01-17T09:31:07.000Z",
      "child_count": 2
    },
    ...
  ]
}
```

<a name="242"></a>
#### 3.13 获取资源科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=resource_subject

请求实例：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=resource_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
   {
      "id": 51,
      "type_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "[药理学]",
      "type": "resource_subject",
      "parent_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "order": 1,
      "createdAt": "2016-01-17T09:33:27.000Z",
      "updatedAt": "2016-01-17T09:33:27.000Z",
      "child_count": null
    },
    ...
  ]
}
```

<a name="243"></a>
#### 2.4.3 获取资源列表
##### 接口地址：/studentManage/api/resource/getAll
##### 方法：get
参数：
- keyword：关键字

请求实例：http://120.25.124.68:4000/studentManage/api/resource/getAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 4,
  "list": [
    {
      "id": 13,
      "resource_id": "02b03bd0-8e2f-11e6-9706-31429135dc45",
      "major_id": "914df890-8e21-11e6-bbda-634c5d4f1964",
      "major_name": "22",
      "subject_id": "a28b6c50-8e21-11e6-bbda-634c5d4f1964",
      "subject_name": "22",
      "title": "22",
      "brief": "22",
      "file": "http://120.25.124.68:4000/upload/upload/text/DSC_0005.JPG",
      "file_size": 1776104,
      "icon": "upload/text/DSC_0005.JPG",
      "level": 0,
      "datems": "1476024324109",
      "createdAt": "2016-10-09T14:45:24.000Z",
      "updatedAt": "2016-10-09T14:45:24.000Z",
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/resource?resource_id=02b03bd0-8e2f-11e6-9706-31429135dc45"
    },
   ...
  ]
}
```
<a name="244"></a>
#### 2.4.4 根据科目ID，获取资源列表，含收藏量，评论量，分页
##### 接口地址：/studentManage/api/resource/list
##### 方法：get
参数：
- keyword：关键字；
- subject_id：科目id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：http://120.25.124.68:4000/studentManage/api/resource/list?subject_id=7d6f44a0-bcfd-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 3,
  "list": [
    {
      "id": 12,
      "resource_id": "4cdc65a0-8ddd-11e6-98bf-177009ddf4c3",
      "major_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "7d6f44a0-bcfd-11e5-8cfe-770f2937a8b8",
      "subject_name": "[生理学]",
      "title": "11",
      "brief": "11",
      "file": "http://120.25.124.68:4000/upload/upload/text/DSC_0005.JPG",
      "file_size": null,
      "icon": null,
      "level": 0,
      "datems": "1475989229818",
      "createdAt": "2016-10-09T05:00:29.000Z",
      "updatedAt": "2016-10-09T05:00:29.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null,
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/resource?resource_id=4cdc65a0-8ddd-11e6-98bf-177009ddf4c3"
    },
    ...
  ]
}

```
<a name="245"></a>
#### 2.4.5 获取资源详情
##### 接口地址：/studentManage/api/resource/getOne
##### 方法：get
参数：
- resource_id：资源ID

请求实例：http://120.25.124.68:4000/studentManage/api/resource/getOne?resource_id=adf71a40-bd1a-11e5-9482-4d7e67b0bbbc

```
{
  "code": "200",
  "msg": "获取信息成功！",
 "item": {
    "id": 3,
    "resource_id": "adf71a40-bd1a-11e5-9482-4d7e67b0bbbc",
    "major_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "subject_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
    "subject_name": "[药理学]",
    "title": "基础医学实验教程",
    "brief": "基础医学实验教程 2010版  同济大学出版社",
    "file": "http://120.25.124.68:4000/upload/text/基础医学实验教程.docx",
    "file_size": 1776104,
    "icon": "http://120.25.124.68:4000/upload/image/30b30b6c3013fff8-a807c704bd5a8c80-36898e699787e6d18edd3ff6b1e5d56f.jpg",
    "level": null,
    "datems": "1453035776696",
    "createdAt": "2016-01-17T13:03:19.000Z",
    "updatedAt": "2016-01-17T13:03:19.000Z",
    "s_count": 1,
    "d_count": 1,
    "p_count": null,
    "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/resource?resource_id=adf71a40-bd1a-11e5-9482-4d7e67b0bbbc"
  }
}

```




<a name="25"></a>
### 2.5 新闻相关
<a name="251"></a>
#### 2.5.1 获取新闻标签列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
参数：
- type=subscription

请求实例：
http://120.25.124.68:4000/studentManage/api/type/findListByType?type=subscription

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 22,
      "type_id": "4f72ae90-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "推荐",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:06:11.000Z",
      "updatedAt": "2016-01-04T14:06:11.000Z"
    },
    {
      "id": 23,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "热点",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:06:26.000Z",
      "updatedAt": "2016-01-04T14:06:26.000Z"
    },
    ...
  ]
}
```
<a name="252"></a>
#### 2.5.2 获取新闻列表
##### 接口地址：/studentManage/api/news/list
##### 方法：get
参数：
- type_id：新闻类型id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：http://120.25.124.68:4000/studentManage/api/news/list?type_id=5811dda0-b2ec-11e5-a306-33448f6b146a

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 16,
      "news_id": "1b85d400-36fd-11e6-ab7b-4b13ffcc5cad",
      "level": 0,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热点",
      "title": "喜讯 | 我院医生向护士下跪求婚啦~",
      "brief": "祝贺：又一对医护情人终成眷侣",
      "icon": "http://120.25.124.68:4000/upload/image/640.webp (1).jpg",
      "content": "<!DOCTYPE html><html>...</body></html>",
      "html": null,
      "from": "医生热点",
      "datems": "1466437139777",
      "createdAt": "2016-06-20T15:38:59.000Z",
      "updatedAt": "2016-06-20T15:38:59.000Z",
      "s_count": 1,  //收藏量
      "d_count": 1,  //点赞量
      "p_count": 1  //评论两
    },
    ...
  ]
}
```




<a name="253"></a>
#### 2.5.3  获取新闻详情
##### 接口地址：/studentManage/api/news/getOne
##### 方法：get
参数：
- news_id：新闻id
- user_id：当前登录用户ID（可以为空）

请求实例：http://localhost:4000/studentManage/api/news/getOne?news_id=c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad&user_id=af0aae90-e3a5-11e5-9620-594c23421db2

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "ifDz": "yes",
  "ifSc": "yes",
  "item": {
    "id": 24,
    "news_id": "c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad",
    "level": 1,
    "type_id": "4f72ae90-b2ec-11e5-a306-33448f6b146a",
    "type_name": "推荐",
    "title": "麻醉学",
    "brief": "带你走近麻醉学",
    "icon": "http://120.25.124.68:4000/upload/image/30b30b6c3013fff8-a807c704bd5a8c80-36898e699787e6d18edd3ff6b1e5d56f.jpg",
    "content": "<p>...</p>\r\n",
    "html": null,
    "from": "医学生APP",
    "datems": "1467126774471",
    "createdAt": "2016-06-28T15:12:54.000Z",
    "updatedAt": "2016-06-28T15:12:54.000Z",
    "s_count": 1,
    "d_count": 1,
    "p_count": 6,
    "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/news?news_id=c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad"
  },
  "pCount": 6,
  "commentlist": [
    {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "user_name": "小明",
      "user_account": "18521508353",
      "user_icon": "image/user_icon_14791470360003070headicon_1479147028321.png",
      "id": 431,
      "comment_id": "f87403b0-b10e-11e6-b63f-2bde797ff8f9",
      "parent_id": "c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad",
      "parent_type": "news",
      "content": "测试",
      "datems": "1479858853739",
      "createdAt": "2016-11-22T23:54:13.000Z",
      "updatedAt": "2016-11-22T23:54:13.000Z",
      "d_count": null,
      "p_count": null
    },
  ...
  ]
}
```


<a name="254"></a>
#### 2.5.4  获取新闻评论列表
##### 接口地址：/studentManage/api/comment/list
##### 方法：get
参数：
- parent_id：新闻id

请求实例：http://120.25.124.68:4000/studentManage/api/comment/list?parent_id=df8a5720-bd10-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 1,
  "list": [
    {
      "user_id": "6a3eb1f0-ad2f-11e5-9ec1-cbdc2e34acc2",
      "user_name": "wuwanyu",
      "user_account": "wuwanyu_321@163.com",
      "user_icon": null,
      "id": 1,
      "comment_id": "3cfd8ef0-b47d-11e5-bab5-79e7bf5aabea",
      "parent_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "parent_type": null,
      "content": "试题有点难度",
      "datems": "1451285486224",
      "createdAt": "2016-01-06T14:41:30.000Z",
      "updatedAt": "2016-01-06T14:41:34.000Z"
    }
  ]
}

```


<a name="255"></a>
#### 2.5.5  获取新闻详情，及评价列表
##### 接口地址：/studentManage/api/news/getOneAndCommentList
##### 方法：get
参数：
- news_id：新闻id
- user_id：当前登陆用户ID（可以为空）

请求实例：http://120.25.124.68:4000/studentManage/api/news/getOneAndCommentList?news_id=645442a0-3d3a-11e6-ab7b-4b13ffcc5cad&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "ifDz": "no",
  "pCount": 8,
  "item": {
    "id": 20,
    "news_id": "645442a0-3d3a-11e6-ab7b-4b13ffcc5cad",
    "level": 0,
    "type_id": "4f72ae90-b2ec-11e5-a306-33448f6b146a",
    "type_name": "推荐",
    "title": "2016医师实践技能考试流程介绍及注意事项",
    "brief": "2016临床医师实践技能考试内容及形式",
    "icon": "http://120.25.124.68:4000/upload/image/f5321fbeb49000f3-80ecbc89c4a088aa-dbf42eb628d7d758308d893bfe65bdb5.jpg",
    "content": "<!DOCTYPE html><html><head><meta charset='utf-8'>...</body></html>",
    "html": null,
    "from": "医学生APP",
    "datems": "1467123168202",
    "createdAt": "2016-06-28T14:12:48.000Z",
    "updatedAt": "2016-06-28T14:12:48.000Z",
    "s_count": 0,
    "d_count": 0,
    "p_count": 8,
    "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/news?news_id=645442a0-3d3a-11e6-ab7b-4b13ffcc5cad"
  },
  "commentlist": [
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "Wayne",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 168,
      "comment_id": "e460f8d0-9843-11e6-b84f-e1f157a2941a",
      "parent_id": "645442a0-3d3a-11e6-ab7b-4b13ffcc5cad",
      "parent_type": "news",
      "content": "vhn",
      "datems": "1477132804317",
      "createdAt": "2016-10-22T10:40:04.000Z",
      "updatedAt": "2016-10-22T10:40:04.000Z",
      "d_count": null,
      "p_count": null
    },
   ...
  ]
}
```

<a name="26"></a>
### 2.6 社区相关
<a name="261"></a>
#### 2.6.1 获取社区列表
##### 接口地址：/studentManage/api/community/list
##### 方法：get
参数：
- keyword：关键字
- user_id：当前用户id
- page:页码，默认1
- limit:每页条 ，默认10

请求实例：
http://120.25.124.68:4000/studentManage/api/community/list?user_id=af0aae90-e3a5-11e5-9620-594c23421db2

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 4,
  "list": [
    {
      "id": 9,
      "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "name": "医学生",
      "title": "白衣天使医学生",
      "icon": "http://120.25.124.68:4000/upload/image/u=3017883673,869767310&fm=11&gp=0.jpg",
      "level": null,
      "createdAt": "2016-01-04T14:10:02.000Z",
      "updatedAt": "2016-01-04T14:10:02.000Z",
      "if_g": 1,  //if_g>0:已关注
      "g_count": 1, //关注量
      "t_count": 12  //发帖量
    },
    ...
  ]
}
```

<a name="262"></a>
#### 2.6.2 获取热门社区列表
##### 接口地址：/studentManage/api/community/hotList
##### 方法：get
参数：
- user_id：登陆用户id（可为空）

请求实例：
http://120.25.124.68:4000/studentManage/api/community/hotList?user_id=af0aae90-e3a5-11e5-9620-594c23421db2

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 3,
  "list": [
    {
      "id": 9,
      "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "name": "医学生",
      "title": "白衣天使医学生",
      "icon": "http://120.25.124.68:4000/upload/image/u=3017883673,869767310&fm=11&gp=0.jpg",
      "level": null,
      "createdAt": "2016-01-04T14:10:02.000Z",
      "updatedAt": "2016-01-04T14:10:02.000Z",
      "if_g": 1,  //if_g>0：当前用户已关注
      "g_count": 1,  //关注量
      "t_count": 12  //发帖量
    },
    {
      "id": 16,
      "community_id": "d27636c0-7986-11e6-b4da-816d0a14741c",
      "name": "测试社区2",
      "title": "测试发帖",
      "icon": "http://120.25.124.68:4000/upload/image/DSC_0005.JPG",
      "level": null,
      "createdAt": "2016-09-13T07:51:04.000Z",
      "updatedAt": "2016-09-13T07:51:04.000Z",
      "if_g": 1,
      "g_count": 1,
      "t_count": 6
    },
    {
      "id": 14,
      "community_id": "5b507080-7731-11e6-b88a-bd8872b6f557",
      "name": "测试",
      "title": "测试专用社区",
      "icon": "http://120.25.124.68:4000/upload/image/001owIUPzy72KTT1bBj3d&690.jpg",
      "level": null,
      "createdAt": "2016-09-10T08:34:15.000Z",
      "updatedAt": "2016-09-10T08:34:15.000Z",
      "if_g": 1,
      "g_count": 1,
      "t_count": 5
    }
  ]
}
```


<a name="263"></a>
#### 2.6.3 获取社区详情，及帖子列表
##### 接口地址：/studentManage/api/community/getOne
##### 方法：get
参数：
- community_id：社区id
- user_id：用户id(可选)

请求实例：
http://120.25.124.68:4000/studentManage/api/community/getOne?community_id=95e8d500-bcfd-11e5-8cfe-770f2937a8b8&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "ifFocused": "",
  "community": {
    "id": 9,
    "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "name": "医学生",
    "title": "白衣天使医学生",
    "icon": "http://120.25.124.68:4000/upload/image/u=3017883673,869767310&fm=11&gp=0.jpg",
    "level": null,
    "createdAt": "2016-01-04T14:10:02.000Z",
    "updatedAt": "2016-01-04T14:10:02.000Z",
    "g_count": 1,
    "t_count": 12
  },
  "postlist": [
    {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "user_name": "小明",
      "user_account": "18521508353",
      "user_icon": "http://120.25.124.68:4000/upload/image/user_icon_14791470360003070headicon_1479147028321.png",
      "id": 99,
      "post_id": "57735490-aafe-11e6-b027-250086f3cabb",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "发帖试试",
      "content": "",
      "images": "http://120.25.124.68:4000/upload/image/post_icon_147919200400030969c1300088762eaca9bea_27970.jpg",
      "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
      "datems": "1479192004698",
      "createdAt": "2016-11-15T06:40:04.000Z",
      "updatedAt": "2016-11-15T06:40:04.000Z",
      "f_count": 7,
      "d_count": 1,
      "p_count": 7,
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/post?post_id=57735490-aafe-11e6-b027-250086f3cabb"
    },
   ...
  ]
}
```

<a name="264"></a>
#### 2.6.4 获取帖子列表
##### 接口地址：/studentManage/api/post/list
##### 方法：get
参数：
-user_id：当前登陆用户id（非必需）
- community_id：社区id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

请求实例：
http://120.25.124.68:4000/studentManage/api/post/list?community_id=d8d4d140-b2ec-11e5-a306-33448f6b146a&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 8,
  "list": [
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 70,
      "post_id": "c38799f0-83d7-11e6-a0ef-7b1aeef20292",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试多图发送",
      "content": "测试多图上传",
      "images": "http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20160311_145723_868699.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269236IMG_20160522_171043_1834480.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20131203_171414_224177.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20160404_105918_3455481.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20151129_160805_230829.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269236IMG_20160326_130636_4139133.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20150725_113727_656976.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269236IMG_20160326_131343_2339385.jpg,http://120.25.124.68:4000/upload/image/post_icon_1474887269237IMG_20150321_144151_206803.jpg",
      "level": 0,
      "datems": "1474887340303",
      "createdAt": "2016-09-26T10:55:40.000Z",
      "updatedAt": "2016-09-26T10:55:40.000Z",
       "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
      "if_d": 1,   //是否点赞，>1为当前用户点赞了
      "f_count": null, //分享量
      "d_count": 1, //点赞量
      "p_count": null, //评论量
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/post?post_id=c38799f0-83d7-11e6-a0ef-7b1aeef20292"   //分享链接
    }
  ]
}
```

<a name="265"></a>
#### 2.6.5 获取帖子详情，及评论列表
##### 接口地址：/studentManage/api/post/getOne
##### 方法：get
参数：
- post_id：帖子id
- user_id：登陆用户ID

请求实例：
http://120.25.124.68:4000/studentManage/api/post/getOne?post_id=d8d4d140-b2ec-11e5-a306-33448f6b146a&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5
```
{
  "code": "200",
  "msg": "获取信息成功！",
  "isFocused": "no",
  "ifDz": "no",
  "post": {
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "name": "哈利波特",
    "account": "herrypoter@163.com",
    "icon": "http://120.25.124.68:4000/upload/image/halibote_391073_m.jpg",
    "id": 76,
    "post_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "parent_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
    "parent_name": "晒身边",
    "title": "宝宝心里苦",
    "content": "宝宝心里苦，但宝宝不说",
    "images": "http://120.25.124.68:4000/upload/image/post_icon_14758941890001295412_6410.png\u0001http://120.25.124.68:4000/upload/image/post_icon_14758941900001785514_11151.png\u0001http://120.25.124.68:4000/upload/image/post_icon_14758941900001299313_11762.png\r\n",
    "level": 0,
    "datems": "1475894187035",
    "createdAt": "2016-10-08T02:36:27.000Z",
    "updatedAt": "2016-10-08T02:36:27.000Z",
     "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
    "f_count": 0,
    "s_count": 0,
    "d_count": 0,
    "p_count": 13,
    "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/post?post_id=d8d4d140-b2ec-11e5-a306-33448f6b146a"
  },
  "commentlist": [ 
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "哈利波特",
      "user_account": "herrypoter@163.com",
      "user_icon": "http://120.25.124.68:4000/upload/image/halibote_391073_m.jpg",
      "id": 31,
      "comment_id": "60ff8ef0-800d-11e6-b2ab-d3775a327855",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_type": "post",
      "content": "凑多少",
      "datems": "1474470563167",
      "createdAt": "2016-09-21T15:09:23.000Z",
      "updatedAt": "2016-09-21T15:09:23.000Z",
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "哈利波特",
      "user_account": "herrypoter@163.com",
      "user_icon": "http://120.25.124.68:4000/upload/image/halibote_391073_m.jpg",
      "id": 15,
      "comment_id": "f2696f80-7e48-11e6-98b6-ad8bf8beb992",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_type": "post",
      "content": "测试回帖",
      "datems": "1474276245112",
      "createdAt": "2016-09-19T09:10:45.000Z",
      "updatedAt": "2016-09-19T09:10:45.000Z",
      "d_count": null,
      "p_count": null
    }
  ]
}
```


<a name="266"></a>
#### 2.6.6 发帖

##### 接口地址：/studentManage/api/post/add
##### 方法：post
参数：(form-data)
- parent_id：所属社区id
- parent_name：所属社区
- title：帖子标题
- content：帖子内容
- images: 上传图片
- user_id:用户id

```
{
  "code": "200",
  "msg": "创建成功！",
  "post": {
    "post_id": "00c5fa30-eaab-11e5-85f8-05ebc4dc7db8",
    "parent_id": "1",
    "parent_name": "1",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "user_name": "HerryPoter",
    "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
    "images": "public/file/3bd870116ff9708f5141aa8a374aeabf.jpg\u0001public/file/3bd870116ff9708f5141aa8a374aeabf.jpg",
    "title": "1",
    "content": "1",
    "level": 0,
    "datems": "1458045290883",
    "createdAt": "2016-03-15T12:39:47.802Z",
    "updatedAt": "2016-03-15T12:39:47.802Z",
     "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
    "id": 22
    
  }
}
```



<a name="268"></a>
#### 2.6.7 获取精选帖列表
##### 接口地址：/studentManage/api/post/goodlist
##### 方法：get
参数：
- user_id：当前登陆用户id（可以为空）

测试接口：
http://120.25.124.68:4000/studentManage/api/post/goodlist?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "name": "HerryPoter",
      "account": "HerryPoter@163.com",
      "icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 10,
      "post_id": "e4007ba0-e541-11e5-85a9-b5063fca5f8b",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 2,
      "datems": "1457450512284",
      "createdAt": "2016-03-08T15:24:46.000Z",
      "updatedAt": "2016-03-08T15:24:46.000Z",
       "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
      "if_d": 1,
      "f_count": null,
      "d_count": 1,
      "p_count": null,
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/post?post_id=e4007ba0-e541-11e5-85a9-b5063fca5f8b"
    },
   ...
  ]
}
```

<a name="269"></a>
#### 2.6.8 根据社区id，获取置顶贴列表
##### 接口地址：/studentManage/api/post/toplist
##### 方法：get

参数：
- community_id：社区id

返回值：
```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 4,
      "post_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "我的苦逼考研日记",
      "content": "我的苦逼考研日记内容",
      "images": null,
      "level": 1,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "杨梅",
      "user_icon": null,
      "datems": "1450521352744",
      "createdAt": "2015-12-19T10:36:45.000Z",
      "updatedAt": "2016-03-13T10:50:12.000Z",
       "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 11,
      "post_id": "ea1619a0-e541-11e5-85a9-b5063fca5f8b",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 1,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "user_icon": null,
      "datems": "1457450512284",
      "createdAt": "2016-03-08T15:24:56.000Z",
      "updatedAt": "2016-03-13T10:50:15.000Z",
       "zd": 1,  //zd=1:置顶
      "jx": 1, //zd=1:精选
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ],
  "count": 2
}
```


<a name="2613"></a>
#### 5.6.13 删除帖子
##### 接口地址：/studentManage/api/post/delete
##### 方法：get

参数：
- post_id：帖子id

返回值：
```
{
  "code": "200",
  "msg": "删除成功！",
  "item": [
    {
      "id": 108,
      "post_id": "9e9a9100-b7cc-11e6-b3f1-737665d66528",
      "parent_id": null,
      "parent_name": null,
      "title": null,
      "content": null,
      "images": null,
      "level": 0,
      "user_id": null,
      "datems": "1480600014352",
      "createdAt": "2016-12-01T13:46:54.000Z",
      "updatedAt": "2016-12-01T13:46:54.000Z"
    }
  ]
}
```


<a name="27"></a>
### 2.7 用户相关

<a name="270"></a>
#### 2.7.0 获取短信验证码
##### 接口地址：/studentManage/system/sms
##### 方法：get
参数：
mobile:发送至手机号


```
{
  "code": "200",
  "msg": "验证码发送成功",
  "sms": "759827", //验证码
  "sms_result": {
    "reason": "操作成功",
    "result": {
      "sid": "125321480238177446",
      "fee": 1,
      "count": 1
    },
    "error_code": 0
  }
}
```

<a name="271"></a>
#### 2.7.1 用户登录
##### 接口地址：/studentManage/api/user/login
##### 方法：post
参数：
account: 账号（例如：18521508353）；
psw: 密码（例如： 111111）

请求实例：
http://120.25.124.68:4000/studentManage/api/user/login

- 登录成功
```

{
  "code": "200",
  "msg": "登录成功！",
  "user": {
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "name": "小明",
    "psw": "111111",
    "account": "18521508353",
    "school": "医学院",
    "major": "doctor",
    "points": 37,
    "datems": "1457270203490",
    "type": "student",
    "icon": "http://120.25.124.68:4000/upload/image/user_icon_14791470360003070headicon_1479147028321.png",
    "sex": "女",
    "age": "22",
    "desc": "医学生呵呵哒哈哈哈",
    "createdAt": "2016-03-06T14:14:05.000Z",
    "updatedAt": "2016-03-06T14:14:05.000Z",
    "id": 15
  }
}
```
- 登录失败：密码输入错误
```
{
  "code": "203",
  "msg": "密码输入错误！"
}
```
- 登录失败：账号不存在
```
{
  "code": "202",
  "msg": "账号不存在！"
}
```



<a name="272"></a>
#### 2.7.2 用户注册
##### 接口地址：/studentManage/api/user/reg
##### 方法：post
参数：(form-data)

account: 账号，例如：HerryPoter@163.com
name: 用户名，例如：HerryPoter
psw:密码，例如： 111111
school: 学校，例如：哈佛大学（非必须）
major: 专业，例如：魔法专业（非必须）
icon: 用户头像，图片文件


请求实例：
http://120.25.124.68:4000/studentManage/api/user/reg

- 注册成功
```
{
  "code": "200",
  "msg": "注册成功！",
  "im_code": 200,
  "im_result": {
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/users",
    "uri": "https://a1.easemob.com/1154161025115110/medic/users",
    "entities": [
      {
        "uuid": "f91c9df0-a032-11e6-b8bc-b1a2c3b64604",
        "type": "user",
        "created": 1478005146959,
        "modified": 1478005146959,
        "username": "1823351902",
        "activated": true
      }
    ],
    "timestamp": 1478005146968,
    "duration": 0,
    "organization": "1154161025115110",
    "applicationName": "medic"
  },
  "item": {
    "account": "1823351902",
    "name": "测试",
    "psw": "111111",
    "school": "东北大学000",
    "major": "通信",
    "icon": "http://120.25.124.68:4000/upload/image/u=890810284,2099347886&fm=21.jpg",
    "user_id": "f924db50-a032-11e6-af98-3f184bdd8625",
    "points": 10,
    "datems": "1478005147014",
    "type": "student",
    "createdAt": "2016-11-01T12:59:07.023Z",
    "updatedAt": "2016-11-01T12:59:07.023Z",
    "id": 38
  }
}
```
- 注册失败：账号已经存在
```
{
  "code": "400",
  "msg": "该账号已经注册！"
}
```






<a name="273"></a>
#### 2.7.3 查看某人主页
##### 接口地址：/studentManage/api/user/getOneHomePage
##### 方法：get
参数：
   user_id：我的id
   obj_id : 对方用户ID（当前登录用户id，可为空）



请求实例：
http://120.25.124.68:4000/studentManage/api/user/getOneHomePage?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&obj_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "isFocused": "no",
  "userInfo": [
    {
      "user_id": "f37ddf20-dbf2-11e6-8e30-072b40dc304a",
      "name": "姚名颜",
      "psw": "199605215122",
      "account": "15700700774",
      "school": "长沙医学院",
      "major": "预防医学",
      "points": 16,
      "datems": "1484574719506",
      "type": "student",
      "icon": "http://120.25.124.68:4000/upload/image/user_icon_14845759770004143headicon_1484575966416.png",
      "sex": "女",
      "age": null,
      "desc": null,
      "createdAt": "2017-01-16T13:51:59.000Z",
      "updatedAt": "2017-01-16T13:51:59.000Z",
      "ID": 101,
      "g_count": 3, //关注量
      "f_count": 3, //粉丝量
      "t_count": 2,//发帖量
      "d_count": 9//点赞量
    }
  ],
  "postList": [
    {
      "user_id": "f37ddf20-dbf2-11e6-8e30-072b40dc304a",
      "user_name": "姚名颜",
      "user_account": "15700700774",
      "user_icon": "image/user_icon_14845759770004143headicon_1484575966416.png",
      "id": 154,
      "post_id": "3f3cb650-e4f6-11e6-88a2-ed44363469b8",
      "parent_id": "71e6ea90-dbae-11e6-8e30-072b40dc304a",
      "parent_name": "医学生",
      "title": "新年快乐*^_^*",
      "content": "我的祝福从延髓出发，沿着迷走神经穿过颈静脉孔，出颅绕左锁骨下动脉，越主动脉经左肺根，达第六胸椎左前方那个叫心脏的角落汹涌而出：新年快乐！ 空气分子振动通过鼓膜，顺着听小骨，通过内耳毛细胞点燃蜗螺旋神经节内的双极细胞，沿着蜗神经经蜗神经腹核和背核经蜗神经腹核和背核经斜方体并交叉上行，经下丘，内侧膝状体，经听辐射，通过内囊到达颞叶颞横回，让我们听到了新年的钟声。夜幕中的光线打到视网膜，经视锥细胞和视杆细胞，双极细胞，来到节细胞，通过视神经，视交叉，视束，外侧膝状体，视辐射止于距状沟周围皮质，绚丽的焰火展现在我",
      "images": null,
      "level": 0,
      "datems": "1485565695541",
      "createdAt": "2017-01-28T01:08:15.000Z",
      "updatedAt": "2017-01-28T01:08:15.000Z",
      "f_count": 0,//分享量
      "d_count": 2,//点赞量
      "p_count": 0,//评论量
      "if_d": null//是否点赞
    },
    ...
  ]
}

```





<a name="274"></a>
#### 2.7.4 修改用户信息
##### 接口地址：/studentManage/api/user/update
##### 方法：post
参数：
user_id：我的id
psw: 密码
name: 用户名
account: 账户
icon:头像
sex: 性别
age: 年龄
desc: 介绍
school：学校
major：专业


请求实例：
http://120.25.124.68:4000/studentManage/api/user/update

```
{
  "code": "200",
  "msg": "操作成功！！",
  "item": {
    "user_id": "2ec86d80-943a-11e6-bdd4-0b564ad60957",
    "name": "武皖豫",
    "psw": "111111",
    "account": "wuwanyu@qq.com",
    "school": "东北大学",
    "major": "通信工程",
    "points": 46,
    "datems": "1476688829529",
    "type": "student",
    "icon": "http://120.25.124.68:4000/upload/image/u=890810284,2099347886&fm=21.jpg",
    "sex": "女",
    "age": "20",
    "desc": "傻瓜",
    "createdAt": "2016-10-17T07:20:29.000Z",
    "updatedAt": "2016-10-17T07:20:29.000Z",
    "ID": 22,
    "g_count": 0,
    "d_count": null
  }
}
```





<a name="2716"></a>
#### 2.7.16 创建一个群组
##### 接口地址：/studentManage/system/im_group_add
##### 方法：post
参数：
groupname:群名称
desc:群描述
owner:管理员账号
members:["wuwanyu","14911111111"]

```
成功返回：
{
  "status": 200,
  "result": {
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "uri": "https://a1.easemob.com/1154161025115110/medic",
    "entities": [],
    "data": {
      "groupid": "259583311825864260"
    },
    "timestamp": 1478003749588,
    "duration": 110,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```

```
失败返回：
{
  "status": 400,
  "result": {
    "error": "illegal_argument",
    "timestamp": 1478003787699,
    "duration": 0,
    "exception": "java.lang.IllegalArgumentException",
    "error_description": "the owner doesn't exist"
  }
}
```

<a name="2717"></a>
#### 2.7.17 修改一个群组
##### 接口地址：/studentManage/system/im_group_edit
##### 方法：post
参数：
group_id:群组id，必填
groupname:群名
desc:描述
maxusers:群组成员最大数（包括群主）


```
成功返回：
{
  "status": 200,
  "result": {
    "action": "put",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "uri": "https://a1.easemob.com/1154161025115110/medic",
    "entities": [],
    "data": {
      "maxusers": false,
      "groupname": false
    },
    "timestamp": 1478003818635,
    "duration": 12,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```


<a name="2718"></a>
#### 2.7.18 删除一个群组
##### 接口地址：/studentManage/system/im_group_delete
##### 方法：post
参数：
group_id:群组id，必填



```
成功返回：
{
  "status": 200,
  "result": {
    "action": "delete",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "uri": "https://a1.easemob.com/1154161025115110/medic",
    "entities": [],
    "data": {
      "success": true,
      "groupid": "259583311825864260"
    },
    "timestamp": 1478004650883,
    "duration": 84,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```

<a name="2719"></a>
#### 2.7.19 添加群组成员[单个] 
##### 接口地址：/studentManage/system/im_group_addUser
##### 方法：post
参数：
group_id:群组id，必填
username:

```
成功返回：
{
  "status": 200,
  "result": {
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "uri": "https://a1.easemob.com/1154161025115110/medic",
    "entities": [],
    "data": {
      "result": true,
      "action": "add_member",
      "user": "15511111111",
      "groupid": "259569979702116780"
    },
    "timestamp": 1478004521924,
    "duration": 65,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```

```
失败返回（群不存在）：
{
  "status": 404,
  "result": {
    "error": "service_resource_not_found",
    "timestamp": 1478004250544,
    "duration": 0,
    "exception": "org.apache.usergrid.services.exceptions.ServiceResourceNotFoundException",
    "error_description": "Service resource not found"
  }
}
失败返回（用户不存在）：
{
  "status": 400,
  "result": {
    "error": "illegal_argument",
    "timestamp": 1478004383519,
    "duration": 0,
    "exception": "java.lang.IllegalArgumentException",
    "error_description": "user 18233561200 doesn't exist"
  }
}
```


<a name="2720"></a>
#### 2.7.20 移除群组成员[单个]
##### 接口地址：/studentManage/system/im_group_deleteUser
##### 方法：post
参数：
group_id:群组id，必填
username:

```
成功返回：
{
  "status": 200,
  "result": {
    "action": "delete",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "uri": "https://a1.easemob.com/1154161025115110/medic",
    "entities": [],
    "data": {
      "result": true,
      "action": "remove_member",
      "user": "15511111111",
      "groupid": "259569979702116780"
    },
    "timestamp": 1478004566892,
    "duration": 27,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```

<a name="2721"></a>
#### 2.7.21 获取一个用户参与的所有群组
##### 接口地址：/studentManage/system/im_group_getGroupListByUser
##### 方法：get
参数：
username:

例如：http://localhost:4000/studentManage/system/im_group_getGroupListByUser?username=1823351900 

```
成功返回：
{
  "status": 200,
  "result": {
    "action": "get",
    "uri": "http://a1.easemob.com/1154161025115110/medic/chatgroups/259565549028116036,259569979702116780",
    "entities": [],
    "data": [
      {
        "membersonly": true,
        "allowinvites": false,
        "public": true,
        "name": "测试群0",
        "description": "server create group",
        "affiliations": [
          {
            "owner": "1823351900"
          },
          {
            "member": "1823351901"
          }
        ],
        "id": "259565549028116036",
        "maxusers": 100,
        "affiliations_count": 2
      },
      {
        "membersonly": true,
        "allowinvites": false,
        "public": true,
        "name": "测试群",
        "description": "server create group",
        "affiliations": [
          {
            "owner": "1823351900"
          },
          {
            "member": "1823351901"
          },
          {
            "member": "wuwanyu"
          }
        ],
        "id": "259569979702116780",
        "maxusers": 300,
        "affiliations_count": 3
      }
    ],
    "timestamp": 1478006388427,
    "duration": 14,
    "count": 2
  }
}
```

<a name="2722"></a>
#### 2.7.22 获取群组所有成员
##### 接口地址：/studentManage/system/im_group_getUserListByGroupId
##### 方法：get
参数：
group_id:群组id，必填

例如：http://localhost:4000/studentManage/system/im_group_getUserListByGroupId?group_id=259569979702116780 

```
成功返回：
{
  "status": 200,
  "result": {
    "action": "get",
    "uri": "http://a1.easemob.com/1154161025115110/medic/chatgroups/259569979702116780/users",
    "entities": [],
    "data": [
      {
        "owner": "1823351900"
      },
      {
        "member": "1823351901"
      },
      {
        "member": "wuwanyu"
      }
    ],
    "timestamp": 1478004036134,
    "duration": 9,
    "count": 3
  }
}
```

<a name="2723"></a>
#### 2.7.23 根据账号，获取用户信息
##### 接口地址：/studentManage/api/user/getUserListByAccount
##### 方法：get
参数：
accountStr:账号列表，英文逗号分隔

例如：http://localhost:4000/studentManage/api/user/getUserListByAccount?accountStr=wuwanyu@qq.com,18521508353

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "result": [
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "name": "wuwanyu",
      "psw": "111111",
      "account": "wuwanyu@qq.com",
      "school": "东北大学",
      "major": "软件工程",
      "points": 4,
      "datems": "1450514441486",
      "type": "student",
      "icon": "http://120.25.124.68:4000/upload/image/halibote_391073_m.jpg",
      "sex": null,
      "age": null,
      "desc": null,
      "createdAt": "2015-12-19T08:42:31.000Z",
      "updatedAt": "2016-10-17T06:33:59.000Z",
      "ID": 3
    },
    {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "name": "小明",
      "psw": "111111",
      "account": "18521508353",
      "school": "医学院",
      "major": "doctor",
      "points": 37,
      "datems": "1457270203490",
      "type": "student",
      "icon": "http://120.25.124.68:4000/upload/image/user_icon_14791470360003070headicon_1479147028321.png",
      "sex": "女",
      "age": "22",
      "desc": "医学生呵呵哒哈哈哈",
      "createdAt": "2016-03-06T14:14:05.000Z",
      "updatedAt": "2016-03-06T14:14:05.000Z",
      "ID": 15
    }
  ]
}
```


<a name="2724"></a>
#### 2.7.24 根据user_id，获取帖子评论列表
##### 接口地址：/studentManage/api/user/getPostCommentListByUserId
##### 方法：get
参数：
user_id:
page:页数，首页为1，默认为1
limit:每页条数，默认10

例如：http://localhost:4000/studentManage/api/user/getPostCommentListByUserId?user_id=af0aae90-e3a5-11e5-9620-594c23421db2

```
{
  "code": "200",
  "msg": "获取成功",
  "count": 45,
  "pList": [
    {
      "comment_id": "e91c87c0-b460-11e6-9092-57b40ba951d8", //评论id
      "content": "好冷啊！好冷，冻成狗",   //帖子内容
      "p_content": "体检",//评论内容
      "p_datems": "1480223900221",
      "p_createdAt": "2016-12-04T03:51:14.000Z",//评论时间
      "p_updatedAt": "2016-12-04T03:51:14.000Z",
      "f_user_id": "67152890-a48e-11e6-b4ca-57cc6867759e",  //点赞人用户id
      "f_user_name": "武皖豫",//点赞人用户名
      "f_user_account": "18321987395", //点赞人用户账户
      "f_user_icon":  "http://120.25.124.68:4000/upload/image/u=890810284,2099347886&fm=21.jpg", //点赞人用户头像
      "post_id": "03e52070-9d24-11e6-adb5-1b908bf34c48",  //帖子id
      "title": "某某某", //帖子标题
      "images": "http://120.25.124.68:4000/upload/image/post_icon_147766886700041636S60405-210850_196031_41366_41469.jpg\u0001http://120.25.124.68:4000/upload/image/post_icon_1477668867000125050P51214-154058_4984509_124061_124572.jpg\u0001http://120.25.124.68:4000/upload/image/post_icon_147766886700070322S60506-163831_511746_70146_70152.jpg",  //帖子图片
      "datems": "1477668869111"
    },
   ...
  ]
}
```



<a name="2725"></a>
#### 2.7.25 根据user_id，获取帖子点赞列表
##### 接口地址：/studentManage/api/user/getPostOperationListByUserId
##### 方法：get
参数：
user_id:
page:页数，首页为1，默认为1
limit:每页条数，默认10

例如：http://localhost:4000/studentManage/api/user/getPostOperationListByUserId?user_id=af0aae90-e3a5-11e5-9620-594c23421db2

```
{
  "code": "200",
  "msg": "获取成功",
  "count": 9,
  "dList": [
    {
      "operation": "d",
      "d_datems": "1480528388309",
      "d_createdAt": "2016-12-07T14:24:45.000Z",
      "d_updatedAt": "2016-12-07T14:24:45.000Z",
      "f_user_id": "b3dfaa30-b6e3-11e6-b698-eb14acb174ac",
      "f_user_name": "北医超哥",
      "f_user_account": "18711183626",
      "f_user_icon": null,
      "post_id": "57735490-aafe-11e6-b027-250086f3cabb",
      "title": "发帖试试",
      "content": "",
      "images": "http://120.25.124.68:4000/upload/image/post_icon_147919200400030969c1300088762eaca9bea_27970.jpg",
      "datems": "1479192004698"
    },
    ...
  ]
}
```

<a name="28"></a>
### 2.8 通用接口
  <a name="281"></a>
#### 2.1.2 评论对象
##### 接口地址：/studentManage/api/comment/add
##### 方法：post
参数：
parent_id：评论对象ID(必填)
parent_type：对象类型，参考下表
user_id：评论人ID(必填)
content：评论内容(必填)

| 序号       |   parent_type | 释义|状态
| ---- | :---------: | ---: | ---: |
| 1      |   course         |  课程||
| 2      |   exam   | 试卷|弃用|
| 2      |   examitem   | 试题||
| 6      |   news       |  新闻||
| 3      |   note     |  笔记||
| 4      |  resource  | 资源||
| 5    | post | 帖子   |     评论后，IM给用户发送消息提醒 |



```
评论帖子返回值：
说明：评论帖子时，会给发帖用户发消息提醒
{
  "code": "200",
  "msg": "评论成功！",
  "result": {
    "parent_id": "03e52070-9d24-11e6-adb5-1b908bf34c48",
    "parent_type": "post",
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "content": "冻成狗也是极好的",
    "comment_id": "8d3d4650-a980-11e6-bfb2-a75446933e60",
    "datems": "1479028027189",
    "createdAt": "2016-11-13T09:07:07.213Z",
    "updatedAt": "2016-11-13T09:07:07.213Z",
    "id": 333
  },
  "im_status": 200,
  "im_result": {
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/messages",
    "uri": "https://a1.easemob.com/1154161025115110/medic/messages",
    "data": {
      "18521508353": "success"
    },
    "timestamp": 1479028028042,
    "duration": 0,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}

```



  <a name="282"></a>
#### 2.8.2 点赞对象
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
参数：
user_id: 用户id
obj_id: 评论id
type：对象类型，参考下表（非必需）
operation = d


| 序号   | parent_type |                 释义 |
| ---- | :---------: | -----------------: |
| 1    |   course    |                 课程 |
| 2    |    exam     |                 试卷 |
| 6    |    news     |                 新闻 |
| 3    |    note     |                 笔记 |
| 4    |  resource   |                 资源 |
| 5    |    post     | 帖子，点赞后，IM给用户发送消息提醒 |
| 5    |   comment   | 评论，点赞后，IM给用户发送消息提醒 |


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "course",
    "operation": "d",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```

```
点赞帖子/评论：
{
  "code": "200",
  "msg": "操作成功！",
  "im_message_code": 200,  //发送提醒消息
  "im_message_result": {
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/messages",
    "uri": "https://a1.easemob.com/1154161025115110/medic/messages",
    "data": {
      "15511111111": "success"
    },
    "timestamp": 1479034422925,
    "duration": 0,
    "organization": "1154161025115110",
    "applicationName": "medic"
  }
}
```


  <a name="283"></a>
#### 2.8.3 收藏对象
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
参数：
- user_id: 用户id
- obj_id: 评论id
- type：对象类型，参考下表（非必需）
- operation = s


| 序号   | parent_type |   释义 |   状态 |
| ---- | :---------: | ---: | ---: |
| 1    |   course    |   课程 |      |
| 2    |    exam     |   试卷 |   弃用 |
| 2    |  examitem   |   试题 |      |
| 6    |    news     |   新闻 |      |
| 3    |    note     |   笔记 |      |
| 4    |  resource   |   资源 |      |

```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "course",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```



  <a name="384"></a>
#### 2.8.4 关注对象
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
参数：
user_id: 用户id
obj_id: 评论id
type：对象类型，参考下表（非必需）
operation = g


| 序号   | parent_type  |              释义 |
| ---- | :----------: | --------------: |
| 1    |  community   |              社区 |
| 2    |     user     | 用户，关注后im发送消息给对方 |
| 6    | subscription |            新闻栏目 |


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "course",
    "operation": "g",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```
```
关注用户：
{
  "code": "200",
  "msg": "操作成功！",
  "im_code": 200,  //同步好友到im
  "im_result": {  //同步好友到im
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/users/ad53d6a0-9a9b-11e6-b088-359c97ea08e8/contacts",
    "uri": "https://a1.easemob.com/1154161025115110/medic/users/ad53d6a0-9a9b-11e6-b088-359c97ea08e8/contacts",
    "entities": [
      {
        "uuid": "52c77090-9f49-11e6-bede-c195a858a893",
        "type": "user",
        "created": 1477904795161,
        "modified": 1477904795161,
        "username": "1823351900",
        "activated": true
      }
    ],
    "timestamp": 1479029072505,
    "duration": 105,
    "organization": "1154161025115110",
    "applicationName": "medic"
  },
  "im_message_code": 200,  //发消息提醒用户被关注了
  "im_message_result": {  //发消息提醒用户被关注了
    "action": "post",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/messages",
    "uri": "https://a1.easemob.com/1154161025115110/medic/messages",
    "data": {
      "1823351900": "success"
    },
    "timestamp": 1479029072784,
    "duration": 0,
    "organization": "1154161025115110",
    "applicationName": "medic"
  },
  "item": {
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "obj_id": "f0202900-9f48-11e6-ad4e-555563142dca",
    "type": "user",
    "operation": "g",
    "datems": "1479029071838",
    "fcount": 0,
    "createdAt": "2016-11-13T09:24:31.849Z",
    "updatedAt": "2016-11-13T09:24:31.849Z",
    "id": 290
  }
}
```

  <a name="285"></a>
#### 2.8.5 用户分享后调用，增加积分
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
参数：
- user_id: 用户id
- obj_id: 评论id
- type：对象类型，参考下表
- operation = f
- parent_id:收藏错题时必需

| 序号   | parent_type |   释义 |
| ---- | :---------: | ---: |
| 1    |   course    |   课程 |
| 2    |    note     |   笔记 |
| 6    |    news     |   新闻 |
| 6    |    post     |   帖子 |
| 6    |  resource   |   资源 |



```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "course",
    "operation": "f",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```

  <a name="286"></a>
#### 2.8.6 用户错题后调用，保存错题
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
参数：
user_id: 用户id
obj_id: 评论id
parent_id: 科目id
type = wrong
operation = s

实例：
http://120.25.124.68:4000/studentManage/api/obj_operation/myWrongSubjectList?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong&operation=s

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 8,
  "list": [
   {
      "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
      "user_name": "小明",
      "user_account": "18521508353",
      "user_icon": "http://120.25.124.68:4000/upload/image/user_icon_14791470360003070headicon_1479147028321.png",
      "id": 99,
      "post_id": "57735490-aafe-11e6-b027-250086f3cabb",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "发帖试试",
      "content": "",
      "images": "http://120.25.124.68:4000/upload/image/post_icon_147919200400030969c1300088762eaca9bea_27970.jpg",
      "level": 0,
      "datems": "1479192004698",
      "createdAt": "2016-11-15T06:40:04.000Z",
      "updatedAt": "2016-11-15T06:40:04.000Z",
      "f_count": 6,
      "d_count": 1,
      "p_count": 2,
      "shared_page_url": "http://120.25.124.68:4000/studentManage/mobile/post?post_id=57735490-aafe-11e6-b027-250086f3cabb"
    },
    ...
  ]
}
```



  <a name="287"></a>
#### 2.8.7 根据对象ID，获取评论列表
##### 接口地址：/studentManage/api/comment/getListByObjId
##### 方法：get
参数：
- obj_id：根据对象id，获取该对象评论列表

##### 请求实例：http://120.25.124.68:4000/studentManage/api/comment/getListByObjId?obj_id=d8d4d140-b2ec-11e5-a306-33448f6b146a


```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 13,
  "list": [
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "user_name": "wuwanyu",
      "user_account": "18233561907",
      "user_icon": null,
      "id": 2,
      "comment_id": "1f2f9c30-7d48-11e6-ad58-a5b719e717c1",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_type": "post",
      "content": "哈哈，，苦逼的楼主",
      "datems": "1474165939571",
      "createdAt": "2016-09-18T02:32:19.000Z",
      "updatedAt": "2016-09-18T02:32:19.000Z"
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 11,
      "comment_id": "e0f10180-7e3b-11e6-a53b-c9ff55515e47",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_type": "post",
      "content": "测试",
      "datems": "1474270632344",
      "createdAt": "2016-09-19T07:37:12.000Z",
      "updatedAt": "2016-09-19T07:37:12.000Z"
    }
  ]
}
```


  <a name="288"></a>
#### 2.8.8 获取我收藏的xxx
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
参数：
- user_id： 用户id；
- type：类别，见下表
- operation = s
- parent_id = 科目id（type=wrong时有）


| 序号   |   type   |   释义 |                                       实例 |
| ---- | :------: | ---: | ---------------------------------------: |
| 1    |  course  |   课程 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=course&operation=s |
| 2    |   exam   |   试卷 |                                       弃用 |
| 2    | examitem |   试题 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=examitem&operation=s |
| 6    |   news   |   新闻 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=news&operation=s |
| 3    |   note   |   笔记 |                                       暂无 |
| 4    | resource |   资源 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=resource  &operation=s |
| 4    |  wrong   |   错题 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong&operation=s&parent_id=3d4e5f80-c34e-11e5-bb5f-afd956debbb5 |






 <a name="289"></a>
#### 2.8.9 获取我关注的xxx 
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
参数：
- user_id: 用户id；
- type：类别，见下表
- operation = g


| 序号   | parent_type  |   释义 | 实例                                       |
| ---- | :----------: | ---: | ---------------------------------------- |
| 1    |  community   |   社区 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=community&operation=g |
| 2    |     user     |   用户 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=user&operation=g |
| 3    | subscription | 新闻栏目 | http://120.25.124.68:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=subscription&operation=g |


```
// community 社区
//示例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=af0aae90-e3a5-11e5-9620-594c23421db2&type=community&operation=g
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 13,
      "community_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "name": "晒身边",
      "title": "晒晒更健康",
      "icon": "http://120.25.124.68:4000/upload/image/u=890810284,2099347886&fm=21.jpg",
      "level": null,
      "createdAt": "2016-01-17T09:35:03.000Z",
      "updatedAt": "2016-09-13T08:55:53.000Z"
    },
   ...
  ]
}
```

```
// user 用户
//示例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=af0aae90-e3a5-11e5-9620-594c23421db2&type=user&operation=g
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "user_id": "67152890-a48e-11e6-b4ca-57cc6867759e",
      "name": "武皖豫",
      "psw": "111111",
      "account": "18321987395",
      "school": "东北大学",
      "major": "通信工程",
      "points": 10,
      "datems": "1478484220314",
      "type": "student",
      "icon": "http://120.25.124.68:4000/upload/image/u=890810284,2099347886&fm=21.jpg",
      "sex": null,
      "age": null,
      "desc": null,
      "createdAt": "2016-11-07T02:03:40.000Z",
      "updatedAt": "2016-11-07T02:03:40.000Z",
      "ID": 39
    },
   ...
  ]
}
```



  <a name="2810"></a>
#### 2.8.10 获取我的错题的科目列表
##### 接口地址：/studentManage/api/obj_operation/myWrongSubjectList
##### 方法：get
参数：
- user_id： 用户id；
- type =  wrong
- operation = s

实例：
http://120.25.124.68:4000/studentManage/api/obj_operation/myWrongSubjectList?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong&operation=s

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "majorList": [
    {
      "id": 36,
      "type_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "http://120.25.124.68:4000/upload/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "order": 1,
      "createdAt": "2016-01-17T09:19:54.000Z",
      "updatedAt": "2016-01-27T11:38:44.000Z",
      "t_count": 1,  //专业下的题目数量
      "subjectList": [
        {
          "t_count": 1, //科目下的题目数量
          "id": 45,
          "type_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
          "icon": "http://120.25.124.68:4000/upload/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
          "name": "药理学",
          "type": "exam_subject",
          "parent_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
          "parent_name": "基础医学",
          "order": 1,
          "createdAt": "2016-01-17T09:26:38.000Z",
          "updatedAt": "2016-01-26T15:34:09.000Z"
        }
      ]
    }
  ]
}
```



  <a name="2811"></a>
#### 2.8.11 获取我的错题列表
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
参数：
user_id： 用户id；
type =  wrong
operation = s
parent_id：科目ID


```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 136,
      "parent_id": "3d4e5f80-c34e-11e5-bb5f-afd956debbb5",
      "obj_id": "18b6fc80-59ef-11e6-87ee-276ad5664adf",
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "operation": "s",
      "type": "wrong",
      "fcount": 0,
      "datems": "1476193106437",
      "createdAt": "2016-10-11T13:38:26.000Z",
      "updatedAt": "2016-10-11T13:38:26.000Z"
    },
    {
      "id": 133,
      "parent_id": null,
      "obj_id": "073026e0-59f3-11e6-87ee-276ad5664adf",
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "operation": "s",
      "type": "wrong",
      "fcount": 0,
      "datems": "1476088591302",
      "createdAt": "2016-10-10T08:36:31.000Z",
      "updatedAt": "2016-10-10T08:36:31.000Z"
    }
  ]
}
```

 

  <a name="2812"></a>
#### 2.8.12 取消收藏
##### 接口地址：/studentManage/api/obj_operation/delete
##### 方法：get

参数：
- user_id: 用户id
- obj_id: 评论id
- type：对象类型，参考下表
- operation = s


| 序号   |   type   |   释义 |   状态 |
| ---- | :------: | ---: | ---: |
| 1    |  course  |   课程 |      |
| 2    |   exam   |   试卷 |   弃用 |
| 2    | examitem |   试题 |      |
| 6    |   news   |   新闻 |      |
| 3    |   note   |   笔记 |      |
| 4    | resource |   资源 |      |

实例：http://localhost:4000/studentManage/api/obj_operation/delete?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong&operation=s&obj_id=2e66cb40-59ff-11e6-87ee-276ad5664adf

```
{
  "code": "200",
  "msg": "操作成功！！",
  "item": {
      "id": 129,
      "parent_id": null,
      "obj_id": "2e66cb40-59ff-11e6-87ee-276ad5664adf",
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "operation": "s",
      "type": "wrong",
      "fcount": 0,
      "datems": "1476084727050",
      "createdAt": "2016-10-10T07:32:07.000Z",
      "updatedAt": "2016-10-10T07:32:07.000Z"
    }
}
```


  <a name="2813"></a>
#### 2.8.13 取消关注
##### 接口地址：/studentManage/api/obj_operation/delete
##### 方法：get
参数：
user_id:用户ID
type:对象类型，参考下表
operation:g
obj_id:

| 序号   |     type     |   释义 |
| ---- | :----------: | ---: |
| 1    |  community   |   社区 |
| 2    |     user     |   用户 |
| 6    | subscription | 新闻栏目 |


实例：http://localhost:4000/studentManage/api/obj_operation/delete?user_id=af0aae90-e3a5-11e5-9620-594c23421db2&type=community&operation=g&obj_id=d8d4d140-b2ec-11e5-a306-33448f6b146a

```
{
  "code": "200",
  "msg": "取消关注/收藏成功！！",
  "item": {
    "id": 41,
    "parent_id": null,
    "obj_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "operation": "g",
    "type": "community",
    "fcount": null,
    "datems": null,
    "createdAt": "2016-09-10T07:54:28.000Z",
    "updatedAt": "2016-09-10T07:54:28.000Z"
  }
}
```
```
取消关注用户
{
  "code": "200",
  "msg": "取消关注/收藏成功！！",
  "im_code": 200,
  "im_result": {
    "action": "delete",
    "application": "9b674910-9a99-11e6-84b4-8f32a891bcf8",
    "path": "/users/52c77090-9f49-11e6-bede-c195a858a893/contacts",
    "uri": "https://a1.easemob.com/1154161025115110/medic/users/52c77090-9f49-11e6-bede-c195a858a893/contacts",
    "entities": [
      {
        "uuid": "400c3470-9f5f-11e6-9dcc-ad5521e8cf4d",
        "type": "user",
        "created": 1477914212663,
        "modified": 1477914212663,
        "username": "1823351901",
        "activated": true
      }
    ],
    "timestamp": 1478005280533,
    "duration": 135,
    "organization": "1154161025115110",
    "applicationName": "medic"
  },
  "item": {
    "id": 227,
    "parent_id": null,
    "obj_id": "40ba9ce0-9f5f-11e6-b5c1-61a7274c1ee2",
    "user_id": "f0202900-9f48-11e6-ad4e-555563142dca",
    "operation": "g",
    "type": "user",
    "fcount": 0,
    "datems": "1478005215990",
    "createdAt": "2016-11-01T13:00:15.000Z",
    "updatedAt": "2016-11-01T13:00:15.000Z"
  }
}
```

 <a name="2814"></a>
#### 2.8.14 取消点赞
##### 接口地址：/studentManage/api/obj_operation/delete
##### 方法：get
参数：
user_id: 用户id
obj_id: 对象id
type：对象类型，参考下表
operation:d

| 序号   | parent_type |                 释义 |
| ---- | :---------: | -----------------: |
| 1    |   course    |                 课程 |
| 2    |    exam     |                 试卷 |
| 6    |    news     |                 新闻 |
| 3    |    note     |                 笔记 |
| 4    |  resource   |                 资源 |
| 5    |    post     | 帖子，点赞后，IM给用户发送消息提醒 |
| 5    |   comment   | 评论，点赞后，IM给用户发送消息提醒 |

实例：

```
{
  "code": "200",
  "msg": "取消点赞/关注/收藏成功！",
  "item": {
    "id": 286,
    "parent_id": null,
    "obj_id": "03e52070-9d24-11e6-adb5-1b908bf34c48",
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "operation": "d",
    "type": "post",
    "fcount": 0,
    "datems": "1478942898516",
    "createdAt": "2016-11-12T09:28:18.000Z",
    "updatedAt": "2016-11-12T09:28:18.000Z"
  }
}
```

<a name="29"></a>
## 2.9 H5界面

  <a name="291"></a>
#### 1. 视频详情及评论列表页
##### 路径：/studentManage/mobile/course
##### 方法：get
参数：
- courseitem_id : 课程章节id

请求实例：
http://120.25.124.68:4000/studentManage/mobile/course?courseitem_id=5f3850f0-bd14-11e5-ace2-11edb9ad68d4




  <a name="292"></a>
#### 2. 笔记详情及评论列表页
##### 路径：/studentManage/mobile/note
##### 方法：get
参数：
- note_id: 笔记id

请求实例：
http://120.25.124.68:4000/studentManage/mobile/note?note_id=ca5fbf90-e13f-11e5-8e43-8bea282120fc


  <a name="293"></a>
#### 3. 新闻详情及评论列表页
##### 路径：/studentManage/mobile/news
##### 方法：get
参数：
- news_id: 新闻id

请求实例：
http://120.25.124.68:4000/studentManage/mobile/news?news_id=c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad



  <a name="294"></a>
#### 4. 帖子详情及评论列表页
##### 路径：/studentManage/mobile/post
##### 方法：get
参数：
- note_id: 笔记id

请求实例：
http://120.25.124.68:4000/studentManage/mobile/post?post_id=d8d4d140-b2ec-11e5-a306-33448f6b146a



















































