项目名称：学生端管理系统/studentManage
---------------------------

* [项目介绍](#项目介绍)
* [第1章 数据库表设计](#数据库表设计)
  * [1.1 课程：tb_course](#tb_course)
  * [1.2 课程章节：tb_courseitem](#tb_courseitem)
  *  [1.3 试卷：tb_exam](#tb_exam)
  * [1.4 试题：tb_examitem](#tb_examitem)
  * [1.5 笔记：tb_note](#tb_note)
  * [1.6 资源：tb_resource](#tb_resource)
  * [1.7 社区：tb_community](#tb_community)
  * [1.8 帖子：tb_post](#tb_post)
  * [1.9 评论：tb_comment](#tb_comment)
  * [1.10 类型：tb_type](#tb_type)
  * [1.11 用户关系表：tb_obj_operation](#tb_obj_operation)
* [第2章 接口设计](#接口设计)
  *  [2.1 课程相关](#课程相关)
	  * [2.1.1 获取课程专业列表](#获取课程专业列表)
	  * [2.1.2 获取课程列表](#获取课程列表)
	  * [2.1.3 获取课程列表，分页，评论量，点赞量，模糊查询](#获取课程列表1)
	  * [2.1.4 获取课程详情，及章节列表](#获取课程详情)
 *  [2.2 题库相关](#题库相关)
	  * [2.2.1 获取试卷专业列表](#获取试卷专业列表)
	  * [2.2.2 获取试卷科目列表](#获取试卷科目列表)
	  * [2.2.3 获取试卷列表](#获取试卷列表)
	  * [2.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询](#获取试卷列表1)
	  * [2.2.5 获取试卷详情，及试题列表](#获取试卷详情)
	  * [2.2.6 收藏试卷](#收藏试卷)
	  * [2.2.7 点赞试卷](#点赞试卷)
 *  [2.3 笔记相关](#笔记相关)
	  *  [2.3.1 获取笔记专业列表](#获取笔记专业列表)
	  * [2.3.2 获取笔记科目列表](#获取笔记科目列表) 
	  * [2.3.3 获取笔记列表](#获取笔记列表)
	  * [2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询](#获取笔记列表1)
	  * [2.3.5 获取笔记详情](#获取笔记详情)
	  * [2.3.6 收藏笔记](#收藏笔记)
	  * [2.3.7 点赞笔记](#点赞笔记)
  *  [2.4 资源相关](#资源相关)
	  *  [2.4.1 获取资源专业列表](#获取资源专业列表)
	  * [2.4.2 获取资源科目列表](#获取资源科目列表)
	  * [2.4.3 获取资源列表](#获取资源列表)
	  * [2.4.4 获取资源列表，含收藏量，评论量，分页](#获取资源列表1)
	  * [2.4.5 获取资源详情](#获取资源详情)
	  * [2.4.6 收藏资源](#收藏资源)
	  * [2.4.7 点赞资源](#点赞资源)
  *  [2.5 新闻相关](#新闻相关)
	  * [2.5.1 获取新闻标签列表](#获取新闻标签列表)
	  * [2.5.2 获取新闻列表](#获取新闻列表)
	  * [2.5.3 获取新闻详情](#获取新闻详情)
	  * [2.5.4 添加订阅](#添加订阅)
	  * [2.5.5 收藏新闻](#收藏新闻)
	  * [2.5.6 点赞新闻](#点赞新闻)
  *  [2.6 社区相关](#社区相关)
	  * [2.6.1 获取社区列表](#获取社区列表)
	  *  [2.6.2 获取社区详情，及帖子列表](#获取社区详情)
	  * [2.6.3 获取帖子列表](#获取帖子列表)
	  * [2.6.4 获取帖子详情，及评论列表](#获取帖子详情)
	  * [2.6.5 发帖](#发帖)
	  * [2.6.6 关注社区](#关注社区)
 *  [2.7 用户相关](#用户相关)
	  * [2.7.1 获取我收藏的课程](#获取我收藏的课程)
	  * [2.7.2 获取我收藏的试卷](#获取我收藏的试卷)
	  * [2.7.3 获取我收藏的笔记](#获取我收藏的笔记)
	  * [2.7.4 获取我收藏的新闻](#获取我收藏的新闻)
	  * [2.7.5 获取我的错题](#获取我的错题)
	  * [2.7.6 获取我关注的社区](#获取我关注的社区)
	  * [2.7.7 获取我关注的新闻标签](#获取我关注的新闻标签)
	  * [2.7.8 用户登录](#用户登录)
	  * [2.7.9 用户注册](#用户注册)
	  
### 最新添加(2016.3.13)：
- 2.6.5 发帖
- 2.5.4 添加订阅




<a name="项目介绍"></a>
### 项目介绍
##### ip地址：120.25.124.68
##### 接口访问地址：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=course_major

<a name="数据库表设计"></a>
### 数据库表设计

<a name="tb_course"></a>
#### 1.1 课程：tb_course

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   course_id| String    |课程id|
| 3      |   major_id|  String   |专业id|
| 4      |   major_name| String  |专业名称|
| 1      |   title|  String   |课程标题|
| 2      |   icon| String    |课程图标|
| 3      |   brief|  String   |课程简介|
| 4      |   datems| String  |时间戳|

<a name="tb_courseitem"></a>
#### 1.2 课程章节：tb_courseitem

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   courseitem_id| String    |课程章节id|
| 3      |   parent_id|  String   |课程id|
| 4      |   parent_name| String  |课程名称|
| 1      |   title|  String   |课程章节标题|
| 2      |   src| String    |视频路径|
| 3      |   brief|  String   |课程简介|
| 4      |   datems| String  |时间戳|

<a name="tb_exam"></a>
#### 1.3 试卷：tb_exam

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   exam_id| String    |试卷id|
| 3      |   major_id|  String   |专业id|
| 4      |   major_name| String  |专业名称|
| 3      |   subject_id|  String   |科目id|
| 4      |   subject_name| String  |科目名称|
| 1      |   name|  String   |标题|
| 2      |   icon| String    |图标|
| 3      |   brief|  String   |简介|
| 3      |   level|  String   |等级（普通：0，精选：1）|
| 4      |   datems| String  |时间戳|

<a name="tb_examitem"></a>
#### 1.4 试题：tb_examitem

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   examitem_id| String    |试题id|
| 3      |   parent_id|  String   |试卷id|
| 4      |   parent_name| String  |试卷名称|
| 1      |   type |  String   |类型（选择题：0，填空：1，简答：2）|
| 2      |   content  | String    |试题内容|
| 3      |   answer  |  String   |试题答案|
| 3      |   analysis  |  String   |试题解析|
| 3      |   selects|  String   |试题选项|
| 4      |   datems| String  |时间戳|

<a name="tb_note"></a>
#### 1.5 笔记：tb_note

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   note_id| String    |笔记id|
| 3      |   major_id|  String   |专业id|
| 4      |   major_name| String  |专业名称|
| 3      |   subject_id|  String   |科目id|
| 4      |   subject_name| String  |科目名称|
| 1      |   title|  String   |笔记标题|
| 2      |   content| String    |笔记内容|
| 3      |   level|  String   |等级（普通：0，精选：1）|
| 4      |   datems| String  |时间戳|


<a name="tb_resource"></a>
#### 1.6 资源：tb_resource

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   resource_id| String    |资源id|
| 3      |   major_id|  String   |专业id|
| 4      |   major_name| String  |专业名称|
| 3      |   subject_id|  String   |科目id|
| 4      |   subject_name| String  |科目名称|
| 1      |   title|  String   |笔记标题|
| 2      |   brief| String    |笔记内容|
| 2      |   file| String    |资源地址|
| 3      |   level|  String   |等级（普通：0，精选：1）|
| 4      |   datems| String  |时间戳|

<a name="tb_community"></a>
#### 1.7 社区：tb_community

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   community_id| String    |社区id|
| 1      |   name|  String   |社区名称|
| 1      |   title|  String   |社区标语|
| 2      |   icon| String    |社区图标|

<a name="tb_post"></a>
#### 1.8 帖子：tb_post

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   post_id| String    |帖子id|
| 3      |   parent_id|  String   |所属社区id|
| 4      |   parent_name| String  |所属社区名称|
| 1      |   title|  String   |帖子标题|
| 2      |   content| String    |帖子内容|
| 3      |   user_id|  String   |发帖人id|
| 4      |   user_name| String  |发帖人名称|
| 3      |   level|  String   |等级（普通：0，置顶：1，精选：2）|
| 4      |   datems| String  |时间戳|

<a name="tb_comment"></a>
#### 1.9 评论：tb_comment

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   comment_id| String    |评论id|
| 3      |   parent_id|  String   |评论帖子id|
| 4      |   parent_name| String  |评论帖子的标题|
| 3      |   user_id|  String   |评论人id|
| 4      |   user_name| String  |评论人名称|
| 2      |   content| String    |评论内容|
| 4      |   datems| String  |时间戳|

<a name="tb_type"></a>
#### 2.0 类型：tb_type

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   type_id| String    |类型id|
| 1      |   icon|  int   |图标|
| 2      |   name| String    |名称|
| 2      |   type| String    |类型|
| 3      |   parent_id|  String   |父类型id|
| 4      |   parent_name| String  |付雷星名称|

<a name="tb_obj_operation"></a>
#### 2.1 用户关系表：tb_obj_operation

| 序号       |    参数名 | 类型  |释义|
| -----|:----:| ----:| ----:|
| 1      |   id|  int   |id|
| 2      |   obj_id| String    |对象id|
| 3      |   user_id|  String   |操作人id|
| 2      |   operation| String  |操作名称|
| 4      |   type| String  |对象类型|


----------


<a name="接口设计"></a>
## 接口设计
<a name="课程相关"></a>
### 2.1 课程相关
  <a name="获取课程专业列表"></a>
#### 2.1.1 获取课程专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=course_major

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=course_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 35,
      "type_id": "5558e310-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=1822233235,2188182299&fm=21&gp=0.jpg",
      "name": "中医专业",
      "type": "course_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:18:55.000Z",
      "updatedAt": "2016-01-17T09:18:55.000Z"
    },
    {
      "id": 34,
      "type_id": "49c664a0-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=935180124,1843516422&fm=21&gp=0.jpg",
      "name": "护理专业",
      "type": "course_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:18:36.000Z",
      "updatedAt": "2016-01-17T09:18:36.000Z"
    },
    {
      "id": 32,
      "type_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "course_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:17:49.000Z",
      "updatedAt": "2016-01-17T09:17:49.000Z"
    },
    {
      "id": 33,
      "type_id": "426c38b0-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=3041013660,671874781&fm=21&gp=0.jpg",
      "name": "临床医学",
      "type": "course_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:18:24.000Z",
      "updatedAt": "2016-01-17T09:18:24.000Z"
    }
  ]
}
```
  <a name="获取课程列表"></a>
#### 2.1.2 获取课程列表
##### 接口地址：/studentManage/api/course/getAll
##### 方法：get
##### 参数：
- keyword：关键字

##### 请求实例：http://localhost:4000/studentManage/api/course/getAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 1,
      "course_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "brief": "主讲人（\r\n\r\n陆源 浙江大学\r\n\r\n）",
      "datems": "1453032631713",
      "createdAt": "2016-01-17T12:12:04.000Z",
      "updatedAt": "2016-01-17T12:33:53.000Z"
    },
    {
      "id": 2,
      "course_id": "e50b6d20-bd9b-11e5-bfd4-dbfa9e5ccea7",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学导论视频教程",
      "icon": "/files/image/1.jpg",
      "brief": "浙江大学",
      "datems": "1453090908594",
      "createdAt": "2016-01-18T04:28:16.000Z",
      "updatedAt": "2016-01-18T04:28:16.000Z"
    }
  ],
  "count": 2
}
```
  <a name="获取课程列表1"></a>
#### 2.1.3 获取课程列表，分页，评论量，点赞量，模糊查询
##### 接口地址：/studentManage/api/course/list
##### 方法：get
##### 参数：
- major_id：专业id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/course/list?major_id=2d92b270-bcfb-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 1,
      "course_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "brief": "主讲人（\r\n\r\n陆源 浙江大学\r\n\r\n）",
      "datems": "1453032631713",
      "createdAt": "2016-01-17T12:12:04.000Z",
      "updatedAt": "2016-01-17T12:33:53.000Z",
      "s_count": null,  //收藏量
      "d_count": null, //点赞量
      "p_count": null  //评论量
    },
    {
      "id": 2,
      "course_id": "e50b6d20-bd9b-11e5-bfd4-dbfa9e5ccea7",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学导论视频教程",
      "icon": "/files/image/1.jpg",
      "brief": "浙江大学",
      "datems": "1453090908594",
      "createdAt": "2016-01-18T04:28:16.000Z",
      "updatedAt": "2016-01-18T04:28:16.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
  <a name="获取课程详情"></a>
#### 2.1.4 获取课程详情，及章节列表
##### 接口地址：/studentManage/api/course/getOne
##### 方法：get
##### 参数：
- courseid：课程id

##### 请求实例：http://localhost:4000/studentManage/api/course/getOne?course_id=85ad17d0-bd13-11e5-9a2d-27445d93409c

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "item": {
    "id": 1,
    "course_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
    "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "title": "基础医学实验(甲) 陆源 全7讲 浙江大学",
    "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
    "brief": "主讲人（\r\n\r\n陆源 浙江大学\r\n\r\n）",
    "datems": "1453032631713",
    "createdAt": "2016-01-17T12:12:04.000Z",
    "updatedAt": "2016-01-17T12:33:53.000Z",
    "s_count": null,
    "d_count": null,
    "p_count": null
  },
  "courseitemList": [
    {
      "id": 12,
      "courseitem_id": "5f3850f0-bd14-11e5-ace2-11edb9ad68d4",
      "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "parent_name": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "title": "第一章 概率",
      "src": "/files/video/mv1.mp4",
      "brief": "基础医学课程介绍,基础医学课程介绍 ！",
      "datems": "1453032994594",
      "createdAt": "2016-01-17T12:18:09.000Z",
      "updatedAt": "2016-01-17T12:38:16.000Z"
    },
    {
      "id": 13,
      "courseitem_id": "387039f0-bd15-11e5-ace2-11edb9ad68d4",
      "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "parent_name": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "title": "第二章  基础医学的意义",
      "src": "/files/video/mv1.mp4",
      "brief": "基础医学的意义,基础医学的意义",
      "datems": "1453032994594",
      "createdAt": "2016-01-17T12:24:14.000Z",
      "updatedAt": "2016-01-17T12:24:14.000Z"
    },
    {
      "id": 14,
      "courseitem_id": "261b9ef0-bd17-11e5-ace2-11edb9ad68d4",
      "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "parent_name": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "title": "第三章 解剖学入门",
      "src": "/files/video/mv1.mp4",
      "brief": "解剖学是基础医学的重点部分",
      "datems": "1453032994594",
      "createdAt": "2016-01-17T12:38:02.000Z",
      "updatedAt": "2016-01-17T12:38:02.000Z"
    }
  ]
}
```
<a name="题库相关"></a>
### 2.2 题库相关
  <a name="获取试卷专业列表"></a>
#### 2.2.1 获取试卷专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=exam_major

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=exam_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 36,
      "type_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:19:54.000Z",
      "updatedAt": "2016-01-17T09:19:54.000Z"
    },
    {
      "id": 37,
      "type_id": "82cca110-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=3041013660,671874781&fm=21&gp=0.jpg",
      "name": "临床医学",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:20:12.000Z",
      "updatedAt": "2016-01-17T09:20:12.000Z"
    },
    {
      "id": 39,
      "type_id": "97e74f00-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=1822233235,2188182299&fm=21&gp=0.jpg",
      "name": "中医专业",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:20:47.000Z",
      "updatedAt": "2016-01-17T09:20:47.000Z"
    },
    {
      "id": 38,
      "type_id": "893fc860-bcfb-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=935180124,1843516422&fm=21&gp=0.jpg",
      "name": "护理专业",
      "type": "exam_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:20:23.000Z",
      "updatedAt": "2016-01-17T09:20:23.000Z"
    }
  ]
}
```
  <a name="获取试卷科目列表"></a>
#### 2.2.2 获取试卷科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=exam_subject

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=exam_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 45,
      "type_id": "69265b10-bcfc-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "药理学",
      "type": "exam_subject",
      "parent_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:26:38.000Z",
      "updatedAt": "2016-01-17T09:26:38.000Z"
    },
    {
      "id": 46,
      "type_id": "a7edd3f0-bcfc-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=585329176,2311950479&fm=206&gp=0.jpg",
      "name": "[生理学]",
      "type": "exam_subject",
      "parent_id": "780d5120-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:28:23.000Z",
      "updatedAt": "2016-01-17T09:28:23.000Z"
    }
  ]
}
```
  <a name="获取试卷列表"></a>
#### 2.2.3 获取试卷列表
##### 接口地址：/studentManage/api/exam/findAll
##### 方法：get
##### 参数：
- keyword：关键字

##### 请求实例：http://localhost:4000/studentManage/api/exam/findAll

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
  <a name="获取试卷列表1"></a>
#### 2.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询
##### 接口地址：/studentManage/api/exam/list
##### 方法：get
##### 参数：
- subject_id：科目id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/exam/list?subject_id=69265b10-bcfc-11e5-8cfe-770f2937a8b8

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
  <a name="获取试卷详情"></a>
#### 2.2.5 获取试卷详情，及试题列表
##### 接口地址：/studentManage/api/exam/getOne
##### 方法：get
##### 参数：
- exam_id：试卷id

##### 请求实例：http://localhost:4000/studentManage/api/exam/getOne?exam_id=df8a5720-bd10-11e5-8cfe-770f2937a8b8

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "item": {  //试卷信息
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
    "s_count": null,
    "d_count": null,
    "p_count": 2
  },
  "examitemList": [   //试题列表
    {
      "id": 23,
      "examitem_id": "3278f630-bd11-11e5-8cfe-770f2937a8b8",
      "parent_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "parent_name": "[药物代谢动力学]",
      "type": "0",  //试题类型，选择：0；填空：1；简答：2
      "content": "某弱酸药物pka=3.4,在血浆中解离百分率约：",
      "answer": "4",
      "analysis": "17865200985: ，PH-PKa=7.4-3.4=4, 离子型/非离子型=10的4次方=10000 解离百分率=离子型/（离子型+非离子型）=10000/10001=99.99%",
      "selects": "10%,90%,99%,99.9%,99.99%",  //选项
      "datems": "1453014632009",
      "createdAt": "2016-01-17T11:55:26.000Z",
      "updatedAt": "2016-01-17T12:03:52.000Z"
    },
    {
      "id": 24,
      "examitem_id": "8c0c5e70-bd12-11e5-8cfe-770f2937a8b8",
      "parent_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "parent_name": "[药物代谢动力学]",
      "type": "0",
      "content": "阿司匹林的pKa是3.5,它在pH为7.5肠液中可吸收约：",
      "answer": "$index",
      "analysis": "Jyphh: 详解：对于弱酸性药物而言，离子型/非离子型=10的（PH-PKa）次方 血浆的PH为7.4，PH-PKa=7.4-3.4=4, 离子型/非离子型=10的4次方=10000 解离百分率=离子型/（离子型+非离子型）=10000/10001=99.99%",
      "selects": "1%,0.1%,0.01%,10%,99%",
      "datems": "1453014632009",
      "createdAt": "2016-01-17T12:05:06.000Z",
      "updatedAt": "2016-01-17T12:05:06.000Z"
    }
  ]
}
```



  <a name="收藏试卷"></a>
#### 2.2.6 收藏试卷
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 试卷id
- user_id: 用户id
- type = exam
- operation = s


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "exam",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```

 <a name="点赞试卷"></a>
#### 2.2.7 点赞试卷
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 试卷id
- user_id: 用户id
- type = exam
- operation = d


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "exam",
    "operation": "d",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```




<a name="笔记相关"></a>
### 2.3 笔记相关
  <a name="获取笔记专业列表"></a>
#### 2.3.1 获取笔记专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=note_major

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=note_major

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
<a name="获取笔记科目列表"></a>
#### 2.3.2 获取笔记科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=note_subject

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=note_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 53,
      "type_id": "2858a130-bd18-11e5-ace2-11edb9ad68d4",
      "icon": "/files/image/u=585329176,2311950479&fm=206&gp=0.jpg",
      "name": "[生理学]",
      "type": "note_subject",
      "parent_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T12:45:15.000Z",
      "updatedAt": "2016-01-17T12:45:15.000Z"
    },
    {
      "id": 56,
      "type_id": "53bf0300-bd18-11e5-ace2-11edb9ad68d4",
      "icon": "/files/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "[药理学]",
      "type": "note_subject",
      "parent_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T12:46:28.000Z",
      "updatedAt": "2016-01-17T12:46:28.000Z"
    }
  ]
}
```
<a name="获取笔记列表"></a>
#### 2.3.3 获取笔记列表
##### 接口地址：/studentManage/api/note/getAll
##### 方法：get
##### 参数：
- keyword：关键字

##### 请求实例：http://localhost:4000/studentManage/api/note/getAll

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
<a name="获取笔记列表1"></a>
#### 2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询
##### 接口地址：/studentManage/api/note/list
##### 方法：get
##### 参数：
- keyword：关键字；
- subject_id：科目id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/note/list?subject_id=9039a280-a71b-11e5-b779-99d7f151235d

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
<a name="获取笔记详情"></a>
#### 2.3.5 获取笔记详情
##### 接口地址：/studentManage/api/note/getOne
##### 方法：get
##### 参数：
- note_id：笔记id

##### 请求实例：http://localhost:4000/studentManage/api/note/getOne?note_id=d46a28e0-bd18-11e5-ace2-11edb9ad68d4

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "item": {
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
    "updatedAt": "2016-01-17T14:39:07.000Z",
    "s_count": null,
    "d_count": null,
    "p_count": null
  }
}
```


<a name="收藏笔记"></a>
#### 2.3.6 收藏笔记
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 笔记id
- user_id: 用户id
- type = note
- operation = s


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "note",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
``` 


<a name="点赞笔记"></a>
#### 2.3.7 点赞笔记
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 笔记id
- user_id: 用户id
- type = note
- operation = d

```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "note",
    "operation": "d",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
``` 


<a name="资源相关"></a>
### 2.4 资源相关
<a name="获取资源专业列表"></a>
#### 2.4.1 获取资源专业列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=resource_major

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_major

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 49,
      "type_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "name": "基础医学",
      "type": "resource_major",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-17T09:31:07.000Z",
      "updatedAt": "2016-01-17T09:31:07.000Z"
    }
  ]
}
```

<a name="获取资源科目列表"></a>
#### 3.13 获取资源科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=resource_subject

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 51,
      "type_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "[药理学]",
      "type": "resource_subject",
      "parent_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:33:27.000Z",
      "updatedAt": "2016-01-17T09:33:27.000Z"
    },
    {
      "id": 52,
      "type_id": "7d6f44a0-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=585329176,2311950479&fm=206&gp=0.jpg",
      "name": "[生理学]",
      "type": "resource_subject",
      "parent_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:34:22.000Z",
      "updatedAt": "2016-01-17T09:34:22.000Z"
    }
  ]
}
```
<a name="获取资源科目列表"></a>
#### 2.4.2 获取资源科目列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=resource_subject

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_subject

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 51,
      "type_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=1471746691,2350104888&fm=206&gp=0.jpg",
      "name": "[药理学]",
      "type": "resource_subject",
      "parent_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:33:27.000Z",
      "updatedAt": "2016-01-17T09:33:27.000Z"
    },
    {
      "id": 52,
      "type_id": "7d6f44a0-bcfd-11e5-8cfe-770f2937a8b8",
      "icon": "/files/image/u=585329176,2311950479&fm=206&gp=0.jpg",
      "name": "[生理学]",
      "type": "resource_subject",
      "parent_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "基础医学",
      "createdAt": "2016-01-17T09:34:22.000Z",
      "updatedAt": "2016-01-17T09:34:22.000Z"
    }
  ]
}
```
<a name="获取资源列表"></a>
#### 2.4.3 获取资源列表
##### 接口地址：/studentManage/api/resource/getAll
##### 方法：get
##### 参数：
- keyword：关键字

##### 请求实例：http://localhost:4000/studentManage/api/resource/getAll

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 1,
      "resource_id": "1",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "资源",
      "brief": "资源简介",
      "file": null,
      "level": 1,
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:45:25.000Z",
      "updatedAt": "2016-01-17T14:31:18.000Z"
    },
    {
      "id": 2,
      "resource_id": "22",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "资源1",
      "brief": "资源简介",
      "file": null,
      "level": null,
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:46:12.000Z",
      "updatedAt": "2016-01-16T09:46:15.000Z"
    },
    {
      "id": 3,
      "resource_id": "adf71a40-bd1a-11e5-9482-4d7e67b0bbbc",
      "major_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
      "subject_name": "[药理学]",
      "title": "基础医学实验教程",
      "brief": "基础医学实验教程 2010版  同济大学出版社",
      "file": "/files/text/基础医学实验教程.docx",
      "level": null,
      "datems": "1453035776696",
      "createdAt": "2016-01-17T13:03:19.000Z",
      "updatedAt": "2016-01-17T13:03:19.000Z"
    },
    {
      "id": 6,
      "resource_id": "affef730-bd25-11e5-ac08-2509145d5986",
      "major_id": "0942f900-bcfd-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "subject_id": "5c9a6c00-bcfd-11e5-8cfe-770f2937a8b8",
      "subject_name": "[药理学]",
      "title": "1",
      "brief": "11",
      "file": "/files/image/bg.png",
      "level": 1,
      "datems": "1453040487398",
      "createdAt": "2016-01-17T14:22:06.000Z",
      "updatedAt": "2016-01-17T14:31:19.000Z"
    }
  ]
}
```
<a name="获取资源列表1"></a>
#### 2.4.4 获取资源列表，含收藏量，评论量，分页
##### 接口地址：/studentManage/api/resource/list
##### 方法：get
##### 参数：
- keyword：关键字；
- subject_id：科目id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/resource/list?subject_id=9039a280-a71b-11e5-b779-99d7f151235d

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 1,
      "resource_id": "1",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "资源",
      "brief": "资源简介",
      "file": null,
      "level": 1,
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:45:25.000Z",
      "updatedAt": "2016-01-17T14:31:18.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 2,
      "resource_id": "22",
      "major_id": "0ae184e0-b2d8-11e5-be5c-dd779e20ce46",
      "major_name": "基础医学",
      "subject_id": "9039a280-a71b-11e5-b779-99d7f151235d",
      "subject_name": "内科",
      "title": "资源1",
      "brief": "资源简介",
      "file": null,
      "level": null,
      "datems": "1450515801809",
      "createdAt": "2016-01-16T09:46:12.000Z",
      "updatedAt": "2016-01-16T09:46:15.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}

```
<a name="获取资源详情"></a>
#### 2.4.5 获取资源详情
##### 接口地址：/studentManage/api/resource/getOne
##### 方法：get
##### 参数：
- resource_id：资源ID

##### 请求实例：http://localhost:4000/studentManage/api/resource/getOne?resource_id=adf71a40-bd1a-11e5-9482-4d7e67b0bbbc

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
    "file": "/files/text/基础医学实验教程.docx",
    "level": null,
    "datems": "1453035776696",
    "createdAt": "2016-01-17T13:03:19.000Z",
    "updatedAt": "2016-01-17T13:03:19.000Z",
    "s_count": null,
    "d_count": null,
    "p_count": null
  }
}

```



<a name="收藏资源"></a>
#### 2.4.6 收藏资源
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 资源id
- user_id: 用户id
- type = resource
- operation=s



```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "resource",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}

``` 



<a name="点赞资源"></a>
#### 2.4.7 点赞资源
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 资源id
- user_id: 用户id
- type = resource
- operation = d



```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "resource",
    "operation": "d",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}

``` 


<a name="新闻相关"></a>
### 2.5 新闻相关
<a name="获取新闻标签列表"></a>
#### 2.5.1 获取新闻标签列表
##### 接口地址：/studentManage/api/type/findListByType
##### 方法：get
##### 参数：
- type=subscription

##### 请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=subscription

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
    {
      "id": 24,
      "type_id": "5f8de970-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "医学最前沿",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:06:38.000Z",
      "updatedAt": "2016-01-04T14:06:38.000Z"
    },
    {
      "id": 25,
      "type_id": "673ac940-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "医学考研",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:06:51.000Z",
      "updatedAt": "2016-01-04T14:06:51.000Z"
    },
    {
      "id": 26,
      "type_id": "6ef98360-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "临床医考",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:07:04.000Z",
      "updatedAt": "2016-01-04T14:07:04.000Z"
    },
    {
      "id": 27,
      "type_id": "7498dff0-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "护理医考",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:07:14.000Z",
      "updatedAt": "2016-01-04T14:07:14.000Z"
    },
    {
      "id": 28,
      "type_id": "7b2ef890-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "口腔医考",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:07:25.000Z",
      "updatedAt": "2016-01-04T14:07:25.000Z"
    }
  ]
}
```
<a name="获取新闻列表"></a>
#### 2.5.2 获取新闻列表
##### 接口地址：/studentManage/api/news/list
##### 方法：get
##### 参数：
- type_id：新闻类型id；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/news/list?type_id=5811dda0-b2ec-11e5-a306-33448f6b146a

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 2,
  "list": [
    {
      "id": 1,
      "news_id": "35087d60-a85a-11e5-aa1d-11c0314c8644",
      "level": 1,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热门",
      "title": "新闻标题",
      "brief": "新闻简介",
      "icon": "http://icon.com",
      "content": "新闻内容：本课程通过总结常见的分页样式以及分析对比分页原理以及实现方式，通过代码实例，让你轻松学会分页功能的开发。通过学习本课程，你也能轻松的实现fac",
      "html": "0",
      "from": "网易新闻",
      "datems": "1450754109494",
      "createdAt": "2015-12-22T03:23:08.000Z",
      "updatedAt": "2016-01-17T14:02:27.000Z",
      "s_count": 1,
      "d_count": 1,
      "p_count": null
    },
    {
      "id": 2,
      "news_id": "91a46ab0-a85b-11e5-97b9-87d706f510eb",
      "level": 1,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热门",
      "title": "78岁老太网上卖叶子:每天早8点抢订单 分秒必争",
      "brief": "在彩公司(irodori)社长横石知二指导下,乡村的阿婆做起上网卖叶子的生意,",
      "icon": "/files/image/Koala.jpg",
      "content": "环球网  2015年12月21日 19:00 在彩公司(irodori)社长横石知二指导下,乡村的阿婆做起上网卖叶子的生意,有人年收入逾1000万日圆。 “被钱围绕着,天天都开心”,住在日本德岛县上胜町78岁",
      "html": null,
      "from": "环球网",
      "datems": "1452243620863",
      "createdAt": "2015-12-22T03:24:54.000Z",
      "updatedAt": "2016-01-17T14:03:33.000Z",
      "s_count": 1,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
<a name="获取新闻详情"></a>
#### 2.5.3 获取新闻详情
##### 接口地址：/studentManage/api/news/getOne
##### 方法：get
##### 参数：
- news_id：新闻id

##### 请求实例：http://localhost:4000/studentManage/api/news/getOne?news_id=35087d60-a85a-11e5-aa1d-11c0314c8644

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "item": [
    {
      "id": 1,
      "news_id": "35087d60-a85a-11e5-aa1d-11c0314c8644",
      "level": 1,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热门",
      "title": "新闻标题",
      "brief": "新闻简介",
      "icon": "http://icon.com",
      "content": "新闻内容：本课程通过总结常见的分页样式以及分析对比分页原理以及实现方式，通过代码实例，让你轻松学会分页功能的开发。通过学习本课程，你也能轻松的实现fac",
      "html": "0",
      "from": "网易新闻",
      "datems": "1450754109494",
      "createdAt": "2015-12-22T03:23:08.000Z",
      "updatedAt": "2016-01-17T14:02:27.000Z",
      "s_count": 1,
      "d_count": 1,
      "p_count": null
    }
  ]
}
```





<a name="添加订阅"></a>
#### 2.5.4 添加订阅
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id：新闻标签id
- user_id：用户
- type=subscription
- operation=g

```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "49c664a0-bcfb-11e5-8cfe-770f2937a8b8",
    "user_id": "af0aae90-e3a5-11e5-9620-594c23421db2",
    "type": "subscription",
    "operation": "g",
    "createdAt": "2016-03-13T11:09:54.954Z",
    "updatedAt": "2016-03-13T11:09:54.955Z",
    "id": 39
  }
}
```


<a name="收藏新闻"></a>
#### 2.4.6 收藏新闻
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 新闻id
- user_id: 用户id
- type = news
- operation=s



```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "news",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}

``` 

<a name="点赞新闻"></a>
#### 2.4.5 点赞新闻
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id: 新闻id
- user_id: 用户id
- type = news
- operation = d



```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "news",
    "operation": "d",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}

``` 



<a name="社区相关"></a>
### 2.6 社区相关
<a name="获取社区列表"></a>
#### 2.6.1 获取社区列表
##### 接口地址：/studentManage/api/community/list
##### 方法：get
##### 参数：
- keyword：关键字

##### 请求实例：http://localhost:4000/studentManage/api/community/list

```
{
  "count": 2,
  "list": [
    {
      "id": 9,
      "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "name": "医学生",
      "title": "白衣天使医学生",
      "icon": "/files/image/u=3017883673,869767310&fm=11&gp=0.jpg",
      "createdAt": "2016-01-04T14:10:02.000Z",
      "updatedAt": "2016-01-04T14:10:02.000Z",
      "g_count": null,  //关注量
      "t_count": null   //累计发帖量
    },
    {
      "id": 13,
      "community_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "name": "晒身边",
      "title": "晒晒更健康",
      "icon": "/files/image/u=890810284,2099347886&fm=21.jpg",
      "createdAt": "2016-01-17T09:35:03.000Z",
      "updatedAt": "2016-01-17T09:35:03.000Z",
      "g_count": null,
      "t_count": null
    }
  ]
}
```
<a name="获取社区详情"></a>
#### 2.6.2 获取社区详情，及帖子列表
##### 接口地址：/studentManage/api/community/getOne
##### 方法：get
##### 参数：
- community_id：社区id

##### 请求实例：http://localhost:4000/studentManage/api/community/getOne?community_id=d8d4d140-b2ec-11e5-a306-33448f6b146a

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "community": {  //社区信息
    "id": 9,
    "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "name": "医学生",
    "title": "白衣天使医学生",
    "icon": "/files/image/u=3017883673,869767310&fm=11&gp=0.jpg",
    "createdAt": "2016-01-04T14:10:02.000Z",
    "updatedAt": "2016-01-04T14:10:02.000Z",
    "s_count": null,
    "t_count": 2
  },
  "postlist": [  //帖子列表
    {
      "id": 4,
      "post_id": "4732fa80-a63c-11e5-bda2-a16c423e1024",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "我的苦逼考研日记",
      "content": "我的苦逼考研日记内容",
      "level": 0,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "杨梅",
      "datems": "1450521352744",
      "createdAt": "2015-12-19T10:36:45.000Z",
      "updatedAt": "2016-01-17T13:29:48.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 5,
      "post_id": "223efcd0-bd1e-11e5-8867-73161ac92107",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "关于基础医学的一些疑问",
      "content": "今天学了基础医学的一些课程，发现自己好多不懂得...",
      "level": 1,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "datems": "1453037282590",
      "createdAt": "2016-01-17T13:34:49.000Z",
      "updatedAt": "2016-01-17T13:37:17.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```
<a name="获取帖子列表"></a>
#### 2.6.3 获取帖子列表
##### 接口地址：/studentManage/api/post/list
##### 方法：get
##### 参数：
- community_id：社区id；
- keyword：关键字；
- page：页码（默认为1）；
- limit：每页条数（默认为10）

##### 请求实例：http://localhost:4000/studentManage/api/post/list?community_id=d8d4d140-b2ec-11e5-a306-33448f6b146a

```
{
  "count": 2,
  "list": [
    {
      "id": 4,
      "post_id": "4732fa80-a63c-11e5-bda2-a16c423e1024",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "我的苦逼考研日记",
      "content": "我的苦逼考研日记内容",
      "level": 0,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "杨梅",
      "datems": "1450521352744",
      "createdAt": "2015-12-19T10:36:45.000Z",
      "updatedAt": "2016-01-17T13:29:48.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 5,
      "post_id": "223efcd0-bd1e-11e5-8867-73161ac92107",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "关于基础医学的一些疑问",
      "content": "今天学了基础医学的一些课程，发现自己好多不懂得...",
      "level": 1,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "datems": "1453037282590",
      "createdAt": "2016-01-17T13:34:49.000Z",
      "updatedAt": "2016-01-17T13:37:17.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}

```
<a name="获取帖子详情"></a>
#### 2.6.4 获取帖子详情，及评论列表
##### 接口地址：/studentManage/api/post/getOne
##### 方法：get
##### 参数：
- post_id：帖子id

##### 请求实例：http://localhost:4000/studentManage/api/post/getOne?post_id=4732fa80-a63c-11e5-bda2-a16c423e1024

```
{
  "code": "200",
  "msg": "获取信息成功！",
  "post": {  //帖子信息
    "id": 4,
    "post_id": "4732fa80-a63c-11e5-bda2-a16c423e1024",
    "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "parent_name": "医学生",
    "title": "我的苦逼考研日记",
    "content": "我的苦逼考研日记内容",
    "level": 0,
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "user_name": "杨梅",
    "datems": "1450521352744",
    "createdAt": "2015-12-19T10:36:45.000Z",
    "updatedAt": "2016-01-17T13:29:48.000Z",
    "s_count": null,
    "d_count": null,
    "p_count": null
  },
  "commentlist": [  //评论列表
    {
      "id": 3,
      "comment_id": "3cfd8ef0-b47d-11e5-bab5-79e7bf5aabee",
      "parent_id": "4732fa80-a63c-11e5-bda2-a16c423e1024",
      "parent_name": "我的苦逼考研日记",
      "user_id": "6a3eb1f0-ad2f-11e5-9ec1-cbdc2e34acc2",
      "user_name": "wuwanyu",
      "content": "考研是人生的必修课",
      "datems": "1451285486224",
      "createdAt": null,
      "updatedAt": null,
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}
```



<a name="发帖"></a>
#### 2.6.5 发帖
##### 接口地址：/studentManage/api/post/add
##### 方法：post(form-data)
##### 参数：
- parent_id：所属社区id
- parent_name：所属社区
- title：帖子标题
- content：帖子内容
- images: 上传图片


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
    "images": "public/file/3bd870116ff9708f5141aa8a374aeabf.jpg,public/file/3bd870116ff9708f5141aa8a374aeabf.jpg",
    "title": "1",
    "content": "1",
    "level": 0,
    "datems": "1458045290883",
    "createdAt": "2016-03-15T12:39:47.802Z",
    "updatedAt": "2016-03-15T12:39:47.802Z",
    "id": 22
  }
}
```



<a name="关注社区"></a>
#### 2.6.6 关注社区
##### 接口地址：/studentManage/api/obj_operation/add
##### 方法：post
##### 参数：
- obj_id = 社区id
- user_id = 用户id
- type = coummunity
- operation = g


```
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "coummunity",
    "operation": "g",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}
```



<a name="用户相关"></a>
### 2.7 用户相关

<a name="获取我收藏的课程"></a>
#### 2.7.1 获取我收藏的课程
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
##### 参数：
- user_id: 用户id；
- type= course

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=course

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 2,
      "course_id": "e50b6d20-bd9b-11e5-bfd4-dbfa9e5ccea7",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学导论视频教程",
      "icon": "/files/image/1.jpg",
      "brief": "浙江大学",
      "datems": "1453090908594",
      "createdAt": "2016-01-18T04:28:16.000Z",
      "updatedAt": "2016-01-18T04:28:16.000Z"
    },
    {
      "id": 1,
      "course_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "major_id": "2d92b270-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "基础医学",
      "title": "基础医学实验(甲) 陆源 全7讲 浙江大学",
      "icon": "/files/image/u=350803863,768178692&fm=21&gp=0 (1).jpg",
      "brief": "主讲人（\r\n\r\n陆源 浙江大学\r\n\r\n）",
      "datems": "1453032631713",
      "createdAt": "2016-01-17T12:12:04.000Z",
      "updatedAt": "2016-01-17T12:33:53.000Z"
    }
  ]
}
```
<a name="获取我收藏的试卷"></a>
#### 2.7.2 获取我收藏的试卷
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
##### 参数：
- user_id: 用户id；
- type=exam

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=exam

```
{
  "code": "200",
  "msg": "获取列表成功！",
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
      "updatedAt": "2016-01-17T11:53:07.000Z"
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
      "updatedAt": "2016-01-18T04:39:15.000Z"
    }
  ]
}
```
<a name="获取我收藏的笔记"></a>
#### 2.7.3 获取我收藏的笔记
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
##### 参数：
- user_id: 用户id；
- type=note

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=note

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
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
<a name="获取我收藏的新闻"></a>
#### 2.7.4 获取我收藏的新闻
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
##### 参数：
- user_id: 用户id；
- type=news

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=news

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 1,
      "news_id": "35087d60-a85a-11e5-aa1d-11c0314c8644",
      "level": 1,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热门",
      "title": "新闻标题",
      "brief": "新闻简介",
      "icon": "http://icon.com",
      "content": "新闻内容：本课程通过总结常见的分页样式以及分析对比分页原理以及实现方式，通过代码实例，让你轻松学会分页功能的开发。通过学习本课程，你也能轻松的实现fac",
      "html": "0",
      "from": "网易新闻",
      "datems": "1450754109494",
      "createdAt": "2015-12-22T03:23:08.000Z",
      "updatedAt": "2016-01-17T14:02:27.000Z"
    },
    {
      "id": 2,
      "news_id": "91a46ab0-a85b-11e5-97b9-87d706f510eb",
      "level": 1,
      "type_id": "5811dda0-b2ec-11e5-a306-33448f6b146a",
      "type_name": "热门",
      "title": "78岁老太网上卖叶子:每天早8点抢订单 分秒必争",
      "brief": "在彩公司(irodori)社长横石知二指导下,乡村的阿婆做起上网卖叶子的生意,",
      "icon": "/files/image/Koala.jpg",
      "content": "环球网  2015年12月21日 19:00 在彩公司(irodori)社长横石知二指导下,乡村的阿婆做起上网卖叶子的生意,有人年收入逾1000万日圆。 “被钱围绕着,天天都开心”,住在日本德岛县上胜町78岁",
      "html": null,
      "from": "环球网",
      "datems": "1452243620863",
      "createdAt": "2015-12-22T03:24:54.000Z",
      "updatedAt": "2016-01-17T14:03:33.000Z"
    }
  ]
}
```

<a name="获取我的错题"></a>
#### 2.7.5 获取我的错题
##### 接口地址：/studentManage/api/obj_operation/myCollection
##### 方法：get
##### 参数：
- user_id: 用户id；
- type=wrong

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 25,
      "examitem_id": "a81e47a0-bd9d-11e5-b900-59869364e3c1",
      "parent_id": "6dea1280-bd9d-11e5-b900-59869364e3c1",
      "parent_name": "医学基础知识试题",
      "type": "0",
      "content": "人的呼吸系统包括呼吸道和     (C)",
      "answer": "2,",
      "analysis": "",
      "selects": "心   ,肝,肺   ,脾",
      "datems": "1453091743664",
      "createdAt": "2016-01-18T04:40:53.000Z",
      "updatedAt": "2016-01-18T04:40:53.000Z"
    },
    {
      "id": 23,
      "examitem_id": "3278f630-bd11-11e5-8cfe-770f2937a8b8",
      "parent_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "parent_name": "[药物代谢动力学]",
      "type": "0",
      "content": "某弱酸药物pka=3.4,在血浆中解离百分率约：",
      "answer": "4",
      "analysis": "17865200985: ，PH-PKa=7.4-3.4=4, 离子型/非离子型=10的4次方=10000 解离百分率=离子型/（离子型+非离子型）=10000/10001=99.99%",
      "selects": "10%,90%,99%,99.9%,99.99%",
      "datems": "1453014632009",
      "createdAt": "2016-01-17T11:55:26.000Z",
      "updatedAt": "2016-01-17T12:03:52.000Z"
    }
  ]
}
```


<a name="获取我关注的社区"></a>
#### 2.7.6 获取我关注的社区
##### 接口地址：/studentManage/api/obj_operation/myFocus
##### 方法：get
##### 参数：
- user_id: 用户id；
-  type=coummunity

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myFocus?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=coummunity

```
{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 9,
      "community_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "name": "医学生",
      "title": "白衣天使医学生",
      "icon": "/files/image/u=3017883673,869767310&fm=11&gp=0.jpg",
      "createdAt": "2016-01-04T14:10:02.000Z",
      "updatedAt": "2016-01-04T14:10:02.000Z"
    },
    {
      "id": 13,
      "community_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "name": "晒身边",
      "title": "晒晒更健康",
      "icon": "/files/image/u=890810284,2099347886&fm=21.jpg",
      "createdAt": "2016-01-17T09:35:03.000Z",
      "updatedAt": "2016-01-17T09:35:03.000Z"
    }
  ]
}
```

<a name="获取我关注的新闻标签"></a>
#### 2.7.7 获取我关注的新闻标签
##### 接口地址：/studentManage/api/obj_operation/myFocus
##### 方法：get
##### 参数：
- user_id: 用户id；
- type=subscription

##### 请求实例：http://localhost:4000/studentManage/api/obj_operation/myFocus?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=subscription

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
      "id": 24,
      "type_id": "5f8de970-b2ec-11e5-a306-33448f6b146a",
      "icon": "",
      "name": "医学最前沿",
      "type": "subscription",
      "parent_id": "",
      "parent_name": "",
      "createdAt": "2016-01-04T14:06:38.000Z",
      "updatedAt": "2016-01-04T14:06:38.000Z"
    }
  ]
}
```


<a name="用户登录"></a>
#### 2.7.8 用户登录
##### 接口地址：/studentManage/api/user/login
##### 方法：post
##### 参数：
- account: 账号（例如：wuwanyu_321@163.com）；
- psw: 密码（例如： 123）

##### 请求实例：http://localhost:4000/studentManage/api/user/login

- 登录成功
```
{
  "code": "200",
  "msg": "登录成功！",
  "user": {
    "user_id": "6a3eb1f0-ad2f-11e5-9ec1-cbdc2e34acc2",
    "name": "wuwanyu",
    "psw": "123",
    "account": "wuwanyu_321@163.com",
    "school": "西北大学",
    "major": "软件工程",
    "points": "10",
    "datems": null,
    "type": "student",
    "icon": "/files/image/Tulips.jpg",
    "desc": null,
    "createdAt": "2015-12-28T06:52:57.000Z",
    "updatedAt": "2015-12-28T06:52:57.000Z",
    "id": 4
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



<a name="用户注册"></a>
#### 2.7.9 用户注册
##### 接口地址：/studentManage/api/user/reg
##### 方法：post
##### 参数：
- account: 账号，例如：HerryPoter@163.com
- psw:密码，例如： 111111
- name: 用户名，例如：HerryPoter
- school: 学校，例如：哈佛大学（非必须）
- major: 专业，例如：魔法专业（非必须）
- icon:：头像，例如： http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg（非必须）

##### 请求实例：http://localhost:4000/studentManage/api/user/reg

- 注册成功
```
{
  "code": "200",
  "msg": "注册成功！",
  "item": {
    "account": "HerryPoter@163.com",
    "psw": "111111",
    "name": "HerryPoter",
    "school": "哈佛大学",
    "major": "魔法专业",
    "icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
    "user_id": "c7318520-dbd0-11e5-85bf-7b6030e90180",
    "points": "10",
    "datems": "1456412200184",
    "type": "student",
    "createdAt": "2016-02-25T15:02:24.629Z",
    "updatedAt": "2016-02-25T15:02:24.629Z",
    "id": 10
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






























































