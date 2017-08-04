 开源项目 代码片段 企业版 特惠 我的码云
 
搜索...
   wuwanyu
 Unwatch 2   Fork 0
 wuwanyu / studentJavaScript
 代码  Issues 0  Pull Requests 0  附件 0  Wiki 0  统计  服务    管理
医学生 -- 编辑
 3 Commits
 1 Branches
 0 Tags
 0 Releases
 1 Contributors
克隆/下载 master   student /  README.md
一键复制编辑原始数据按行查看历史
 README.md 95.00 KB →  wuwanyu wuwanyu 提交于 2017-07-31 14:01 . first commit
<<<<<<< HEAD

studentManage接口文档
项目介绍
第1章 h5界面
1.1 课程相关
1.1.1 视频详情及评论列表页
1.1.2 第三方视频源播放页
1.2 笔记相关
1.2.1 笔记详情及评论列表页
1.3 新闻相关
1.3.1 新闻详情及评论列表页
1.4 社区相关
1.4.1 帖子详情及评论列表页 *
第1章 接口设计
11 课程相关
1.1.1 获取课程专业列表
1.1.2 获取课程列表
1.1.3 获取课程列表，分页，评论量，点赞量，模糊查询
1.1.4 获取课程详情，及章节列表
1.1.4 获取视频详情，课程评价
1.1.5 收藏课程
1.1.6 点赞课程
1.1.7 评价课程
1.2 题库相关
1.2.1 获取试卷专业列表
1.2.2 获取试卷科目列表
1.2.3 获取试卷列表
1.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询
1.2.5 获取试卷详情，及试题列表
1.2.6 收藏试卷
1.2.7 点赞试卷
1.2.8 评价试卷
1.2.8 收藏试题
2.2.9 获取我收藏试题的试卷列表
2.2.10 根据试卷id，获取我收藏试题的列表
2.3 笔记相关
2.3.1 获取笔记专业列表
2.3.2 获取笔记科目列表
2.3.3 获取笔记列表
2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询
2.3.5 获取笔记详情，及评价列表
2.3.6 收藏笔记
2.3.7 点赞笔记
2.3.8 评价笔记
2.4 资源相关
2.4.1 获取资源专业列表
2.4.2 获取资源科目列表
2.4.3 获取资源列表
2.4.4 获取资源列表，含收藏量，评论量，分页
2.4.5 获取资源详情
2.4.6 收藏资源
2.4.7 点赞资源
2.4.8 评论资源
2.5 新闻相关
2.5.1 获取新闻标签列表
2.5.2 获取新闻列表
2.5.3 获取新闻详情，及评价列表
2.5.4 添加订阅
2.5.5 收藏新闻
2.5.6 点赞新闻
2.5.7 评价新闻
2.6 社区相关
2.6.1 获取社区列表
2.6.2 获取社区详情，及帖子列表
2.6.3 获取帖子列表
2.6.4 获取帖子详情，及评论列表
2.6.5 发帖
2.6.6 关注社区
2.6.7 获取精选帖列表
2.6.8 根据社区id，获取置顶贴列表
2.6.9 点赞帖子
2.6.10 评论帖子
2.7 用户相关
2.7.1 获取我收藏的课程
2.7.2 获取我收藏的试卷
2.7.3 获取我收藏的笔记
2.7.4 获取我收藏的新闻
2.7.5 获取我的错题
2.7.6 获取我关注的社区
2.7.7 获取我关注的新闻标签
2.7.8 用户登录
2.7.9 用户注册
2.7.10 查看某人主页

项目介绍

ip地址：120.25.124.68

接口访问地址：http://120.25.124.68:4000/studentManage/api/type/findListByType?type=course_major


H5界面

1.1 课程相关


1.1.1 视频详情及评论列表页

路径：/studentManage/mobile/course

方法：get

参数：

courseitem_id : 课程章节id
请求实例：http://localhost:4000/studentManage/mobile/course?courseitem_id=5f3850f0-bd14-11e5-ace2-11edb9ad68d4


1.2 笔记相关


1.2.1 笔记详情及评论列表页

路径：/studentManage/mobile/note

方法：get

参数：

note_id: 笔记id
请求实例：http://localhost:4000/studentManage/mobile/note?note_id=ca5fbf90-e13f-11e5-8e43-8bea282120fc


1.3 新闻相关


1.3.1 新闻详情及评论列表页

路径：/studentManage/mobile/news

方法：get

参数：

news_id: 新闻id
请求实例：http://localhost:4000/studentManage/mobile/news?news_id=c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad


1.4 社区相关


1.4.1 帖子详情及评论列表页

路径：/studentManage/mobile/post

方法：get

参数：

post_id: 帖子id
请求实例：http://localhost:4000/studentManage/mobile/post?post_id=d8d4d140-b2ec-11e5-a306-33448f6b146a#left-link


接口设计

2.1 课程相关


2.1.1 获取课程专业列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=course_major
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=course_major

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

2.1.2 获取课程列表

接口地址：/studentManage/api/course/getAll

方法：get

参数：

keyword：关键字
请求实例：http://localhost:4000/studentManage/api/course/getAll

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

2.1.3 获取课程列表，分页，评论量，点赞量，模糊查询

接口地址：/studentManage/api/course/list

方法：get

参数：

major_id：专业id；
keyword：关键字；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/course/list?major_id=2d92b270-bcfb-11e5-8cfe-770f2937a8b8

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

2.1.4 获取课程详情，及章节列表

接口地址：/studentManage/api/course/getOne

方法：get

参数：

courseid：课程id
请求实例：http://localhost:4000/studentManage/api/course/getOne?course_id=85ad17d0-bd13-11e5-9a2d-27445d93409c

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

2.1.4 获取视频详情，课程评价

接口地址：/studentManage/api/courseitem/getOne

方法：get

参数：

courseid：课程id
请求实例：http://localhost:4000/studentManage/api/courseitem/getOne?courseitem_id=5f3850f0-bd14-11e5-ace2-11edb9ad68d4

{
  "code": "200",
  "msg": "获取信息成功！",
  "courseitem": {
    "id": 12,
    "courseitem_id": "5f3850f0-bd14-11e5-ace2-11edb9ad68d4",
    "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
    "parent_name": "基础医学实验(甲) 陆源 全7讲 浙江大学",
    "title": "第一章 概率",
    "src": "http://120.25.124.68:3010/video/mv1.mp4",
    "from": "0",
    "video_page_url": null,
    "brief": "基础医学课程介绍,基础医学课程介绍 ！",
    "datems": "1453032994594",
    "createdAt": "2016-01-17T12:18:09.000Z",
    "updatedAt": "2016-01-17T12:38:16.000Z"
  },
  "commentlist": [
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "user_name": "wuwanyu",
      "user_account": "18233561907",
      "user_icon": null,
      "id": 3,
      "comment_id": "43791740-7d4a-11e6-ad58-a5b719e717c1",
      "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
      "parent_type": "course",
      "content": "中医很实用",
      "datems": "1474166859445",
      "createdAt": "2016-09-18T02:47:39.000Z",
      "updatedAt": "2016-09-18T02:47:39.000Z",
      "d_count": null,
      "p_count": null
    }
  ]
}

2.1.5 收藏课程

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 课程id
user_id: 用户id
type = course
operation = s
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

1.1.6 点赞课程

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 课程id
user_id: 用户id
type = course
operation = d
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

1.1.7 评价课程

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id:课程id
parent_type:course
user_id:评论人id
content:评论内容
{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "85ad17d0-bd13-11e5-9a2d-27445d93409c",
    "parent_type": "course",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "中医很实用",
    "comment_id": "43791740-7d4a-11e6-ad58-a5b719e717c1",
    "datems": "1474166859445",
    "createdAt": "2016-09-18T02:47:39.451Z",
    "updatedAt": "2016-09-18T02:47:39.451Z",
    "id": 3
  }
}

2.2 题库相关


2.2.1 获取试卷专业列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=exam_major
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=exam_major

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

2.2.2 获取试卷科目列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=exam_subject
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=exam_subject

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

2.2.3 获取试卷列表

接口地址：/studentManage/api/exam/findAll

方法：get

参数：

keyword：关键字
请求实例：http://localhost:4000/studentManage/api/exam/findAll

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

2.2.4 获取试卷列表，含点赞数量、收藏数量，分页，模糊查询

接口地址：/studentManage/api/exam/list

方法：get

参数：

subject_id：科目id；
keyword：关键字；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/exam/list?subject_id=69265b10-bcfc-11e5-8cfe-770f2937a8b8

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

2.2.5 获取试卷详情，及试题列表

接口地址：/studentManage/api/exam/getOne

方法：get

参数：

exam_id：试卷id
请求实例：http://localhost:4000/studentManage/api/exam/getOne?exam_id=df8a5720-bd10-11e5-8cfe-770f2937a8b8

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

2.2.6 收藏试卷

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 试卷id
user_id: 用户id
type = exam
operation = s
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

2.2.7 点赞试卷

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 试卷id
user_id: 用户id
type = exam
operation = d
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

1.2.8 评价试卷

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id:试卷id
parent_type:exam
user_id:评论人id
content:评论内容
{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "8dc79c90-c2b0-11e5-8a20-8f644d73d409",
    "parent_type": "exam",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "药理学被老师讲解的好极了",
    "comment_id": "b3a3b0c0-7d4a-11e6-ad58-a5b719e717c1",
    "datems": "1474167047628",
    "createdAt": "2016-09-18T02:50:47.629Z",
    "updatedAt": "2016-09-18T02:50:47.629Z",
    "id": 4
  }
}

2.2.8 收藏试题

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 试题id
exam_id: 试卷id
user_id: 用户id
type = collect_examitem
operation = s
{
  "code": "200",
  "msg": "创建成功！",
  "item": {
     "parent_id": "ba8201d0-c733-11e5-aefe-9bbbaef0bed1",
    "obj_id": "726d2480-e8dd-11e5-9620-594c23421db2",
    "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
    "type": "collect_examitem",
    "operation": "s",
    "createdAt": "2016-03-14T12:25:11.806Z",
    "updatedAt": "2016-03-14T12:25:11.806Z",
    "id": 40
  }
}

2.2.9 获取我收藏试题的试卷列表

接口地址：/studentManage/api/obj_operation/getCollectExamByUserId

方法：get

参数：

user_id: 用户id
type = collect_examitem
实例：http://localhost:4000/studentManage/api/obj_operation/getCollectExamByUserId?type=collect_examitem&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
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
      "updatedAt": "2016-02-29T11:44:17.000Z"
    },
    {
      "id": 21,
      "exam_id": "ba8201d0-c733-11e5-aefe-9bbbaef0bed1",
      "major_id": "82cca110-bcfb-11e5-8cfe-770f2937a8b8",
      "major_name": "临床医学",
      "subject_id": "50ee0630-c34e-11e5-bb5f-afd956debbb5",
      "subject_name": "内科学",
      "icon": null,
      "name": "肺炎",
      "brief": "",
      "level": null,
      "datems": "1454075656910",
      "createdAt": "2016-01-30T09:27:49.000Z",
      "updatedAt": "2016-02-29T11:56:23.000Z"
    }
  ]
}

2.2.10 根据试卷id，获取我收藏试题的列表

接口地址：/studentManage/api/obj_operation/getCollectExamitemListByExamId

方法：get

参数：

user_id: 用户id
type = collect_examitem
exam_id:试卷id
实例：http://localhost:4000/studentManage/api/obj_operation/getCollectExamitemListByExamId?type=collect_examitem&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&exam_id=ba8201d0-c733-11e5-aefe-9bbbaef0bed1

{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 27,
      "examitem_id": "4168e210-c354-11e5-bb5f-afd956debbb5",
      "parent_id": "26e42a50-c352-11e5-bb5f-afd956debbb5",
      "parent_name": "常见症状",
      "type": "0",
      "content": "2/176. 下列哪项是错误的",
      "answer": "1,",
      "analysis": "稽留热是指体温恒定的维持在39~40℃以上的高水平，达数天或数周，24小时内体温波动范围不超过1℃。常见于大叶性肺炎、斑疹伤寒及伤寒高热期。",
      "selects": "稽留热指体温常在39℃以上，达数天或数周，24小时内体温波动范围不超过1℃,弛张热指体温常在39℃以上，24小时内波动范围不超过1℃，且都在正常水平以上,间歇热指体温升高达高峰后持续数小时，又迅速降至正常水平，无热期（间歇期）可持续1天至数天，如此高热期与无热期反复交替出现。,波状热指体温逐渐上升达39℃或以上，数天后又逐渐下降至正常水平，持续数天后又逐渐升高，如此反复多次,不规则热指发热体温曲线无一定规律性",
      "datems": "1453713901105",
      "createdAt": "2016-01-25T11:10:34.000Z",
      "updatedAt": "2016-01-25T11:10:34.000Z"
    },
    {
      "id": 27,
      "examitem_id": "4168e210-c354-11e5-bb5f-afd956debbb5",
      "parent_id": "26e42a50-c352-11e5-bb5f-afd956debbb5",
      "parent_name": "常见症状",
      "type": "0",
      "content": "2/176. 下列哪项是错误的",
      "answer": "1,",
      "analysis": "稽留热是指体温恒定的维持在39~40℃以上的高水平，达数天或数周，24小时内体温波动范围不超过1℃。常见于大叶性肺炎、斑疹伤寒及伤寒高热期。",
      "selects": "稽留热指体温常在39℃以上，达数天或数周，24小时内体温波动范围不超过1℃,弛张热指体温常在39℃以上，24小时内波动范围不超过1℃，且都在正常水平以上,间歇热指体温升高达高峰后持续数小时，又迅速降至正常水平，无热期（间歇期）可持续1天至数天，如此高热期与无热期反复交替出现。,波状热指体温逐渐上升达39℃或以上，数天后又逐渐下降至正常水平，持续数天后又逐渐升高，如此反复多次,不规则热指发热体温曲线无一定规律性",
      "datems": "1453713901105",
      "createdAt": "2016-01-25T11:10:34.000Z",
      "updatedAt": "2016-01-25T11:10:34.000Z"
    },
    {
      "id": 23,
      "examitem_id": "3278f630-bd11-11e5-8cfe-770f2937a8b8",
      "parent_id": "df8a5720-bd10-11e5-8cfe-770f2937a8b8",
      "parent_name": "药物代谢动力学",
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

2.3 笔记相关


2.3.1 获取笔记专业列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=note_major
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=note_major

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

2.3.2 获取笔记科目列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=note_subject
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=note_subject

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

2.3.3 获取笔记列表

接口地址：/studentManage/api/note/getAll

方法：get

参数：

keyword：关键字
请求实例：http://localhost:4000/studentManage/api/note/getAll

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

2.3.4 获取笔记列表，含点赞量，收藏量，分页，模糊查询

接口地址：/studentManage/api/note/list

方法：get

参数：

keyword：关键字；
subject_id：科目id；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/note/list?subject_id=9039a280-a71b-11e5-b779-99d7f151235d

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

2.3.5 获取笔记详情，及评价列表

接口地址：/studentManage/api/note/getOne

方法：get

参数：

note_id：笔记id
请求实例：http://localhost:4000/studentManage/api/note/getOne?note_id=ca5fbf90-e13f-11e5-8e43-8bea282120fc

{
  "code": "200",
  "msg": "获取信息成功！",
  "note": {
    "id": 9,
    "level": 1,
    "note_id": "ca5fbf90-e13f-11e5-8e43-8bea282120fc",
    "major_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "subject_id": "e9ece7e0-e13d-11e5-8e43-8bea282120fc",
    "subject_name": "病理学",
    "title": "第一章 细胞、组织的适应和损伤",
    "content": "<p>第一节 适 应&nbsp;</p><p>&nbsp; 细胞和其构成的组织、器官能耐受内外环境各种有害因子的刺激作用而得以存活的过程称为适应。在形态上表现为萎缩、肥大、增生和化生。&nbsp;</p><p>&nbsp; 一、萎缩（atrophy）：是指已发育正常的实质细胞、组织、器官的体积缩小。 &nbsp; 1、生理性萎缩：人体许多组织、器官随着年龄增长自然地发生生理性萎缩。 &nbsp; 2、病理性萎缩：&nbsp;</p><p>&nbsp; （1）营养不良性萎缩：可分为局部营养不良性萎缩和全身性营养不良萎缩，后者如：饥饿和恶性肿瘤的恶病质。&nbsp;</p><p>&nbsp; （2）压迫性萎缩：如：肾盂积水引起的肾萎缩。&nbsp;</p><p>&nbsp; （3）废用性萎缩：即长期工作负荷减少所引起的萎缩。 &nbsp; （4）神经性萎缩：如：神经损伤所致的肌肉萎缩。&nbsp;</p><p>&nbsp; （5）内分泌性萎缩：如：垂体肿瘤所引起的肾上腺萎缩。 &nbsp; 二、肥大（hypertrophy）：细胞、组织和器官体积的增大。 &nbsp;&nbsp;</p><p>1、代偿性肥大：细胞肥大多具有功能代偿的意义。 &nbsp;</p><p>&nbsp; 2、内分泌性肥大：由激素引发的肥大称为内分泌性肥大。 &nbsp; 三、增生（hyperplasia）：实质细胞的增多，可导致组织器官的增大。&nbsp;</p><p>&nbsp; 1、生理性增生：生理条件下发生的增生。 &nbsp; 2、病理性增生：在病理条件下发生的增生。 &nbsp; 四、化生（metaplasia）：一种分化成熟的细胞转化为另一种分化成熟细胞的过程。 &nbsp; 1、上皮性：胃腺上皮→肠上皮化生&nbsp;</p><p>&nbsp; 柱状上皮（气管、宫颈、胆囊）→鳞状上皮化生 &nbsp; 2、间叶性：纤维结缔组织→骨、软骨 &nbsp; 骨骼肌→骨&nbsp;</p><p>第二节 细胞、组织的损伤 &nbsp; 一、原因和发生机制&nbsp;</p><p>&nbsp; 二、形态学变化&nbsp;</p><p>&nbsp; （一）变性（degeneration）：是指细胞或细胞间质受损伤后因代谢发生障碍所致的某些可逆性形态学变化。表现为细胞浆内或间质中出现异常物质或正常物质异常增多。 &nbsp; 1、细胞水肿（cellular swelling）：细胞内水分的增多。 &nbsp; 肉眼：器官体积肿大，颜色苍白。&nbsp;</p><p>&nbsp; 镜下：依病变轻重，分别呈颗粒变性，疏松样变，气球样变。 &nbsp; 2、脂肪变性（fatty degeneration）：细胞内甘油三脂的蓄积。</p><p>（1）好发部位：肝细胞、心肌纤维、肾小管上皮。 &nbsp; （2）病理变化：肝脂肪变性（严重时为脂肪肝） &nbsp; 心肌脂肪变性→虎斑心&nbsp;</p><p>&nbsp; 3、玻璃样变（hyaline change）：又称透明变性。&nbsp;</p><p>&nbsp;&nbsp;</p><p>（1）细胞内玻璃样变：浆细胞中的Russell小体、酒精性肝病时肝细胞内Mallory小体、</p><p>肾小管上皮细胞中玻璃样小滴。&nbsp;</p><p>&nbsp; （2）纤维结缔组织玻璃样变：胶原纤维增宽融合，呈均质红染。 &nbsp; （3）细动脉玻璃样变：管壁增厚，有红染蛋白性物质沉积，管腔狭窄。 &nbsp; 4、淀粉样变：组织间质中有淀粉样物质沉积。 &nbsp; 5、粘液样变性：组织间质中类粘液物质增多。&nbsp;</p><p>&nbsp; 6、病理性色素沉着：指有色物质（色素）在细胞内外的异常蓄积，其中包括含铁血黄素、脂褐素、黑色素及胆红素等。&nbsp;</p><p>&nbsp; 7、病理性钙化：指骨和牙齿以外的组织中有固体钙盐的沉积，包括转移性钙化和营养不良性钙化。&nbsp;</p><p>&nbsp; （二）坏死（necrosis）：活体内范围不等的局部组织细胞死亡。 &nbsp; 1、基本病变：细胞核：核固缩、核碎裂、核溶解。 &nbsp; 细胞浆：红染、进而解体。 &nbsp; 细胞间质：崩解 &nbsp; 2、类型：&nbsp;</p><p>&nbsp; （1）凝固性坏死：坏死组织发生凝固，常保持轮廓残影。 &nbsp; 好发部位：心肌、肝、脾、肾。&nbsp;</p><p>&nbsp; 病理变化：肉眼：组织干燥，灰白色。&nbsp;</p><p>&nbsp; 镜下：细胞结构消失，组织轮廓保存（早期）。&nbsp;</p><p>&nbsp; 特殊类型：干酪样坏死（发生在结核病灶，坏死组织呈灰黄色，细腻。镜下坏死彻底，不见组织轮廓。） &nbsp; （2）液化性坏死：坏死组织因酶性分解而变为液态。 &nbsp; 好发部位：脑、脊髓等。&nbsp;</p><p>&nbsp; 病理变化：坏死组织分解液化。&nbsp;</p><p>&nbsp; 特殊类型：脂肪坏死（分为创伤性、酶解性，分别好发于乳腺、胰腺）。 &nbsp; （3）坏疽（gangrene）：大块组织坏死后继发腐败菌感染，所形成的特殊形态改变。 &nbsp; 干性坏疽：好发于四肢末端，坏死组织干燥，边界清楚。&nbsp;</p><p>&nbsp; 湿性坏疽：好发于肠管、胆囊、子宫、肺，坏死组织湿润、肿胀，边界不清。 &nbsp; 气性坏疽：常继发于深达肌肉的开放性创伤，由产气荚膜杆菌引起，坏死组织内含气泡呈蜂窝状。&nbsp;</p><p>&nbsp; （4）纤维素性坏死（fibrinoid necrosis）：坏死组织呈细丝、颗粒状，似红染的纤维素。 &nbsp; 好发部位：结缔组织和血管壁。&nbsp;</p><p>&nbsp; 疾病举例：急进性高血压、风湿病、系统性红斑狼疮。 &nbsp; 3、结局&nbsp;</p><p>&nbsp; （1）局部炎症反应：由细胞坏死诱发。&nbsp;</p><p>&nbsp; （2）溶解吸收：坏死组织溶解后常由淋巴管、血管吸收或被巨噬细胞吞噬清除。 &nbsp; （3）分离排除形成缺损：表现为糜烂、溃疡、空洞、瘘管、窦道。&nbsp;</p><p>&nbsp; （4）机化：肉芽组织取代坏死组织的过程。&nbsp;</p><p>&nbsp; （5）包裹、钙化：前者指纤维组织包绕在坏死组织周围，后者指坏死组织中钙盐的沉积。</p><p>（三）凋亡（apoptosis）：活体内单个细胞或小团细胞在基因调空下的程序性死亡。死亡细胞的质膜不破裂，不引发死亡细胞的自溶，不引起急性炎症反应。<br></p>",
    "datems": "1456882589369",
    "createdAt": "2016-03-03T12:59:39.000Z",
    "updatedAt": "2016-03-07T11:09:32.000Z",
    "s_count": 0,
    "d_count": 1,
    "p_count": 1
  }
}

2.3.6 收藏笔记

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 笔记id
user_id: 用户id
type = note
operation = s
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

2.3.7 点赞笔记

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 笔记id
user_id: 用户id
type = note
operation = d
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

2.3.8 评价笔记

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id: 笔记id
parent_type:note
user_id:评论人id
content:评论内容
{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "5bcb3050-e469-11e5-9620-594c23421db2",
    "parent_type": "note",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "输血这一篇笔记好极了",
    "comment_id": "2dbd03c0-7d4b-11e6-ad58-a5b719e717c1",
    "datems": "1474167252476",
    "createdAt": "2016-09-18T02:54:12.477Z",
    "updatedAt": "2016-09-18T02:54:12.477Z",
    "id": 5
  }
}

2.4 资源相关


2.4.1 获取资源专业列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=resource_major
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_major

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

3.13 获取资源科目列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=resource_subject
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_subject

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

2.4.2 获取资源科目列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=resource_subject
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=resource_subject

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

2.4.3 获取资源列表

接口地址：/studentManage/api/resource/getAll

方法：get

参数：

keyword：关键字
请求实例：http://localhost:4000/studentManage/api/resource/getAll

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

2.4.4 获取资源列表，含收藏量，评论量，分页

接口地址：/studentManage/api/resource/list

方法：get

参数：

keyword：关键字；
subject_id：科目id；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/resource/list?subject_id=9039a280-a71b-11e5-b779-99d7f151235d

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


2.4.5 获取资源详情

接口地址：/studentManage/api/resource/getOne

方法：get

参数：

resource_id：资源ID
请求实例：http://localhost:4000/studentManage/api/resource/getOne?resource_id=adf71a40-bd1a-11e5-9482-4d7e67b0bbbc

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


2.4.6 收藏资源

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 资源id
user_id: 用户id
type = resource
operation=s
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


2.4.7 点赞资源

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 资源id
user_id: 用户id
type = resource
operation = d
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


2.4.8 评论资源

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id:资源id
parent_type:resource
user_id:评论人id
content:评论内容
{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "63899030-c447-11e5-b7b8-9b9bf580f0d3",
    "parent_type": "resource",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "资源不错，感谢分享",
    "comment_id": "728421a0-7d4b-11e6-ad58-a5b719e717c1",
    "datems": "1474167367866",
    "createdAt": "2016-09-18T02:56:07.868Z",
    "updatedAt": "2016-09-18T02:56:07.868Z",
    "id": 6
  }
}

2.5 新闻相关


2.5.1 获取新闻标签列表

接口地址：/studentManage/api/type/findListByType

方法：get

参数：

type=subscription
请求实例：http://localhost:4000/studentManage/api/type/findListByType?type=subscription

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

2.5.2 获取新闻列表

接口地址：/studentManage/api/news/list

方法：get

参数：

type_id：新闻类型id；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/news/list?type_id=5811dda0-b2ec-11e5-a306-33448f6b146a

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

2.5.3 获取新闻详情，及评价列表

接口地址：/studentManage/api/news/getOne

方法：get

参数：

news_id：新闻id
请求实例：http://localhost:4000/studentManage/api/news/getOne?news_id=35087d60-a85a-11e5-aa1d-11c0314c8644

{
  "code": "200",
  "msg": "获取信息成功！",
  "commentlist": null,
  "note": {
    "id": 9,
    "level": 1,
    "note_id": "ca5fbf90-e13f-11e5-8e43-8bea282120fc",
    "major_id": "a75077f0-bcfb-11e5-8cfe-770f2937a8b8",
    "major_name": "基础医学",
    "subject_id": "e9ece7e0-e13d-11e5-8e43-8bea282120fc",
    "subject_name": "病理学",
    "title": "第一章 细胞、组织的适应和损伤",
    "content": "<p>第一节 适 应&nbsp;</p><p>&nbsp; 细胞和其构成的组织、器官能耐受内外环境各种有害因子的刺激作用而得以存活的过程称为适应。在形态上表现为萎缩、肥大、增生和化生。&nbsp;</p><p>&nbsp; 一、萎缩（atrophy）：是指已发育正常的实质细胞、组织、器官的体积缩小。 &nbsp; 1、生理性萎缩：人体许多组织、器官随着年龄增长自然地发生生理性萎缩。 &nbsp; 2、病理性萎缩：&nbsp;</p><p>&nbsp; （1）营养不良性萎缩：可分为局部营养不良性萎缩和全身性营养不良萎缩，后者如：饥饿和恶性肿瘤的恶病质。&nbsp;</p><p>&nbsp; （2）压迫性萎缩：如：肾盂积水引起的肾萎缩。&nbsp;</p><p>&nbsp; （3）废用性萎缩：即长期工作负荷减少所引起的萎缩。 &nbsp; （4）神经性萎缩：如：神经损伤所致的肌肉萎缩。&nbsp;</p><p>&nbsp; （5）内分泌性萎缩：如：垂体肿瘤所引起的肾上腺萎缩。 &nbsp; 二、肥大（hypertrophy）：细胞、组织和器官体积的增大。 &nbsp;&nbsp;</p><p>1、代偿性肥大：细胞肥大多具有功能代偿的意义。 &nbsp;</p><p>&nbsp; 2、内分泌性肥大：由激素引发的肥大称为内分泌性肥大。 &nbsp; 三、增生（hyperplasia）：实质细胞的增多，可导致组织器官的增大。&nbsp;</p><p>&nbsp; 1、生理性增生：生理条件下发生的增生。 &nbsp; 2、病理性增生：在病理条件下发生的增生。 &nbsp; 四、化生（metaplasia）：一种分化成熟的细胞转化为另一种分化成熟细胞的过程。 &nbsp; 1、上皮性：胃腺上皮→肠上皮化生&nbsp;</p><p>&nbsp; 柱状上皮（气管、宫颈、胆囊）→鳞状上皮化生 &nbsp; 2、间叶性：纤维结缔组织→骨、软骨 &nbsp; 骨骼肌→骨&nbsp;</p><p>第二节 细胞、组织的损伤 &nbsp; 一、原因和发生机制&nbsp;</p><p>&nbsp; 二、形态学变化&nbsp;</p><p>&nbsp; （一）变性（degeneration）：是指细胞或细胞间质受损伤后因代谢发生障碍所致的某些可逆性形态学变化。表现为细胞浆内或间质中出现异常物质或正常物质异常增多。 &nbsp; 1、细胞水肿（cellular swelling）：细胞内水分的增多。 &nbsp; 肉眼：器官体积肿大，颜色苍白。&nbsp;</p><p>&nbsp; 镜下：依病变轻重，分别呈颗粒变性，疏松样变，气球样变。 &nbsp; 2、脂肪变性（fatty degeneration）：细胞内甘油三脂的蓄积。</p><p>（1）好发部位：肝细胞、心肌纤维、肾小管上皮。 &nbsp; （2）病理变化：肝脂肪变性（严重时为脂肪肝） &nbsp; 心肌脂肪变性→虎斑心&nbsp;</p><p>&nbsp; 3、玻璃样变（hyaline change）：又称透明变性。&nbsp;</p><p>&nbsp;&nbsp;</p><p>（1）细胞内玻璃样变：浆细胞中的Russell小体、酒精性肝病时肝细胞内Mallory小体、</p><p>肾小管上皮细胞中玻璃样小滴。&nbsp;</p><p>&nbsp; （2）纤维结缔组织玻璃样变：胶原纤维增宽融合，呈均质红染。 &nbsp; （3）细动脉玻璃样变：管壁增厚，有红染蛋白性物质沉积，管腔狭窄。 &nbsp; 4、淀粉样变：组织间质中有淀粉样物质沉积。 &nbsp; 5、粘液样变性：组织间质中类粘液物质增多。&nbsp;</p><p>&nbsp; 6、病理性色素沉着：指有色物质（色素）在细胞内外的异常蓄积，其中包括含铁血黄素、脂褐素、黑色素及胆红素等。&nbsp;</p><p>&nbsp; 7、病理性钙化：指骨和牙齿以外的组织中有固体钙盐的沉积，包括转移性钙化和营养不良性钙化。&nbsp;</p><p>&nbsp; （二）坏死（necrosis）：活体内范围不等的局部组织细胞死亡。 &nbsp; 1、基本病变：细胞核：核固缩、核碎裂、核溶解。 &nbsp; 细胞浆：红染、进而解体。 &nbsp; 细胞间质：崩解 &nbsp; 2、类型：&nbsp;</p><p>&nbsp; （1）凝固性坏死：坏死组织发生凝固，常保持轮廓残影。 &nbsp; 好发部位：心肌、肝、脾、肾。&nbsp;</p><p>&nbsp; 病理变化：肉眼：组织干燥，灰白色。&nbsp;</p><p>&nbsp; 镜下：细胞结构消失，组织轮廓保存（早期）。&nbsp;</p><p>&nbsp; 特殊类型：干酪样坏死（发生在结核病灶，坏死组织呈灰黄色，细腻。镜下坏死彻底，不见组织轮廓。） &nbsp; （2）液化性坏死：坏死组织因酶性分解而变为液态。 &nbsp; 好发部位：脑、脊髓等。&nbsp;</p><p>&nbsp; 病理变化：坏死组织分解液化。&nbsp;</p><p>&nbsp; 特殊类型：脂肪坏死（分为创伤性、酶解性，分别好发于乳腺、胰腺）。 &nbsp; （3）坏疽（gangrene）：大块组织坏死后继发腐败菌感染，所形成的特殊形态改变。 &nbsp; 干性坏疽：好发于四肢末端，坏死组织干燥，边界清楚。&nbsp;</p><p>&nbsp; 湿性坏疽：好发于肠管、胆囊、子宫、肺，坏死组织湿润、肿胀，边界不清。 &nbsp; 气性坏疽：常继发于深达肌肉的开放性创伤，由产气荚膜杆菌引起，坏死组织内含气泡呈蜂窝状。&nbsp;</p><p>&nbsp; （4）纤维素性坏死（fibrinoid necrosis）：坏死组织呈细丝、颗粒状，似红染的纤维素。 &nbsp; 好发部位：结缔组织和血管壁。&nbsp;</p><p>&nbsp; 疾病举例：急进性高血压、风湿病、系统性红斑狼疮。 &nbsp; 3、结局&nbsp;</p><p>&nbsp; （1）局部炎症反应：由细胞坏死诱发。&nbsp;</p><p>&nbsp; （2）溶解吸收：坏死组织溶解后常由淋巴管、血管吸收或被巨噬细胞吞噬清除。 &nbsp; （3）分离排除形成缺损：表现为糜烂、溃疡、空洞、瘘管、窦道。&nbsp;</p><p>&nbsp; （4）机化：肉芽组织取代坏死组织的过程。&nbsp;</p><p>&nbsp; （5）包裹、钙化：前者指纤维组织包绕在坏死组织周围，后者指坏死组织中钙盐的沉积。</p><p>（三）凋亡（apoptosis）：活体内单个细胞或小团细胞在基因调空下的程序性死亡。死亡细胞的质膜不破裂，不引发死亡细胞的自溶，不引起急性炎症反应。<br></p>",
    "datems": "1456882589369",
    "createdAt": "2016-03-03T12:59:39.000Z",
    "updatedAt": "2016-03-07T11:09:32.000Z",
    "s_count": 0,
    "d_count": 1,
    "p_count": 1
  }
}

2.5.4 添加订阅

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id：新闻标签id
user_id：用户
type=subscription
operation=g
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

2.4.6 收藏新闻

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 新闻id
user_id: 用户id
type = news
operation=s
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


2.4.5 点赞新闻

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 新闻id
user_id: 用户id
type = news
operation = d
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


2.5.7 评价新闻

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id:新闻id
parent_type:news
user_id:评论人id
content:评论内容
{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "c9d53d70-3d42-11e6-ab7b-4b13ffcc5cad",
    "parent_type": "news",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "新闻不错，感谢分享",
    "comment_id": "b96768c0-7d4b-11e6-ad58-a5b719e717c1",
    "datems": "1474167486796",
    "createdAt": "2016-09-18T02:58:06.800Z",
    "updatedAt": "2016-09-18T02:58:06.800Z",
    "id": 8
  }
}

2.6 社区相关


2.6.1 获取社区列表

接口地址：/studentManage/api/community/list

方法：get

参数：

keyword：关键字
请求实例：http://localhost:4000/studentManage/api/community/list

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

2.6.2 获取社区详情，及帖子列表

接口地址：/studentManage/api/community/getOne

方法：get

参数：

community_id：社区id
user_id：用户id(可选)
请求实例：http://localhost:4000/studentManage/api/community/getOne?community_id=95e8d500-bcfd-11e5-8cfe-770f2937a8b8&user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5

{
  "code": "200",
  "msg": "获取信息成功！",
  "ifFocused": "yes",
  "community": {
    "id": 13,
    "community_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
    "name": "晒身边",
    "title": "晒晒更健康",
    "icon": "http://120.25.124.68:3010/image/u=890810284,2099347886&fm=21.jpg",
    "createdAt": "2016-01-17T09:35:03.000Z",
    "updatedAt": "2016-09-13T08:55:53.000Z",
    "s_count": 2,
    "t_count": 1
  },
  "postlist": [
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 22,
      "post_id": "00c5fa30-eaab-11e5-85f8-05ebc4dc7db8",
      "parent_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "晒身边",
      "title": "小烦恼没什么大不了",
      "content": "小烦恼没什么大不了小烦恼没什么大不了",
      "images": "public/file/3bd870116ff9708f5141aa8a374aeabf.jpg",
      "level": 0,
      "datems": "1458045290883",
      "createdAt": "2016-03-15T12:39:47.000Z",
      "updatedAt": "2016-03-15T12:39:47.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}

2.6.3 获取帖子列表

接口地址：/studentManage/api/post/list

方法：get

参数：

community_id：社区id；
keyword：关键字；
page：页码（默认为1）；
limit：每页条数（默认为10）
请求实例：http://localhost:4000/studentManage/api/post/list?community_id=d8d4d140-b2ec-11e5-a306-33448f6b146a

{
  "code": "200",
  "msg": "获取列表成功！",
  "count": 9,
  "list": [
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "user_name": "wuwanyu",
      "user_account": "18233561907",
      "user_icon": null,
      "id": 34,
      "post_id": "e1e1a9e0-78e7-11e6-8382-710908096f7b",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:53:20.000Z",
      "updatedAt": "2016-09-12T12:53:20.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 4,
      "post_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "我的苦逼考研日记",
      "content": "我的苦逼考研日记内容",
      "images": null,
      "level": 1,
      "datems": "1450521352744",
      "createdAt": "2015-12-19T10:36:45.000Z",
      "updatedAt": "2016-03-13T10:50:12.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "user_name": "wuwanyu",
      "user_account": "18233561907",
      "user_icon": null,
      "id": 35,
      "post_id": "fc9ffa20-78e7-11e6-81d4-67075da56a85",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:54:05.000Z",
      "updatedAt": "2016-09-12T12:54:05.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 5,
      "post_id": "223efcd0-bd1e-11e5-8867-73161ac92107",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "关于基础医学的一些疑问",
      "content": "今天学了基础医学的一些课程，发现自己好多不懂得...",
      "images": null,
      "level": 2,
      "datems": "1453037282590",
      "createdAt": "2016-01-17T13:34:49.000Z",
      "updatedAt": "2016-01-17T13:37:17.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "user_name": "wuwanyu",
      "user_account": "18233561907",
      "user_icon": null,
      "id": 36,
      "post_id": "517ed070-78e8-11e6-a493-3904f149739f",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:56:27.000Z",
      "updatedAt": "2016-09-12T12:56:27.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 11,
      "post_id": "ea1619a0-e541-11e5-85a9-b5063fca5f8b",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 1,
      "datems": "1457450512284",
      "createdAt": "2016-03-08T15:24:56.000Z",
      "updatedAt": "2016-03-13T10:50:15.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
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
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 13,
      "post_id": "bfd90020-e542-11e5-ae05-cb9952b81b77",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 0,
      "datems": "1457450835695",
      "createdAt": "2016-03-08T15:30:55.000Z",
      "updatedAt": "2016-03-08T15:30:55.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "HerryPoter",
      "user_account": "HerryPoter@163.com",
      "user_icon": "http://picm.bbzhi.com/yingshibizhi/halibote/halibote_391073_m.jpg",
      "id": 22,
      "post_id": "00c5fa30-eaab-11e5-85f8-05ebc4dc7db8",
      "parent_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "晒身边",
      "title": "小烦恼没什么大不了",
      "content": "小烦恼没什么大不了小烦恼没什么大不了",
      "images": "public/file/3bd870116ff9708f5141aa8a374aeabf.jpg",
      "level": 0,
      "datems": "1458045290883",
      "createdAt": "2016-03-15T12:39:47.000Z",
      "updatedAt": "2016-03-15T12:39:47.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ]
}

2.6.4 获取帖子详情，及评论列表

接口地址：/studentManage/api/post/getOne

方法：get

参数：

post_id：帖子id
请求实例：http://localhost:4000/studentManage/api/post/getOne?post_id=4732fa80-a63c-11e5-bda2-a16c423e1024

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

2.6.5 发帖

接口地址：/studentManage/api/post/add

方法：post

参数：(form-data)

parent_id：所属社区id
parent_name：所属社区
title：帖子标题
content：帖子内容
images: 上传图片
user_id:用户id
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

2.6.5 点赞帖子

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id: 帖子id
user_id: 用户id
type = post
operation = d
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


2.6.6 关注社区

接口地址：/studentManage/api/obj_operation/add

方法：post

参数：

obj_id = 社区id
user_id = 用户id
type = coummunity
operation = g
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

2.6.7 获取精选帖列表

接口地址：/studentManage/api/post/goodlist

方法：get

参数：

{
  "code": "200",
  "msg": "获取列表成功！",
  "list": [
    {
      "id": 1,
      "post_id": "post01",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "新人报道，望多多指教",
      "content": "0",
      "images": null,
      "level": 2,
      "user_id": "user01",
      "user_name": "wuwanyu",
      "user_icon": null,
      "datems": "3454422",
      "createdAt": null,
      "updatedAt": "2016-03-13T11:16:20.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 2,
      "post_id": "post02",
      "parent_id": "95e8d500-bcfd-11e5-8cfe-770f2937a8b8",
      "parent_name": "晒身边",
      "title": "小烦恼没什么大不了",
      "content": "0",
      "images": null,
      "level": 2,
      "user_id": "user02",
      "user_name": "chenguang",
      "user_icon": null,
      "datems": "3454422",
      "createdAt": null,
      "updatedAt": "2016-03-13T11:16:23.000Z",
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
      "images": null,
      "level": 2,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "user_icon": null,
      "datems": "1453037282590",
      "createdAt": "2016-01-17T13:34:49.000Z",
      "updatedAt": "2016-01-17T13:37:17.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 10,
      "post_id": "e4007ba0-e541-11e5-85a9-b5063fca5f8b",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 2,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "user_icon": null,
      "datems": "1457450512284",
      "createdAt": "2016-03-08T15:24:46.000Z",
      "updatedAt": "2016-03-08T15:24:46.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    },
    {
      "id": 12,
      "post_id": "ba001d00-e542-11e5-ae05-cb9952b81b77",
      "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "测试来了",
      "content": "我是过来测试哒",
      "images": null,
      "level": 2,
      "user_id": "2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5",
      "user_name": "wuwanyu",
      "user_icon": null,
      "datems": "1457450835695",
      "createdAt": "2016-03-08T15:30:45.000Z",
      "updatedAt": "2016-03-08T15:30:45.000Z",
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ],
  "count": 5
}

2.6.8 根据社区id，获取置顶贴列表

接口地址：/studentManage/api/post/toplist

方法：get

参数：

community_id：社区id
返回值：

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
      "s_count": null,
      "d_count": null,
      "p_count": null
    }
  ],
  "count": 2
}

2.6.10 评论帖子

接口地址：/studentManage/api/comment/add

方法：post

参数：

parent_id：帖子id
parent_type = "post"
user_id：发帖人
content：帖子内容
返回值：

{
  "code": "200",
  "msg": "创建成功！",
  "comment": {
    "parent_id": "d8d4d140-b2ec-11e5-a306-33448f6b146a",
    "parent_type": "post",
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "content": "哈哈，，苦逼的楼主",
    "comment_id": "1f2f9c30-7d48-11e6-ad58-a5b719e717c1",
    "datems": "1474165939571",
    "createdAt": "2016-09-18T02:32:19.579Z",
    "updatedAt": "2016-09-18T02:32:19.579Z",
    "id": 2
  }
}

2.7 用户相关


2.7.1 获取我收藏的课程

接口地址：/studentManage/api/obj_operation/myCollection

方法：get

参数：

user_id: 用户id；
type= course
请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=course

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

2.7.2 获取我收藏的试卷

接口地址：/studentManage/api/obj_operation/myCollection

方法：get

参数：

user_id: 用户id；
type=exam
请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=exam

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

2.7.3 获取我收藏的笔记

接口地址：/studentManage/api/obj_operation/myCollection

方法：get

参数：

user_id: 用户id；
type=note
请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=note

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

2.7.4 获取我收藏的新闻

接口地址：/studentManage/api/obj_operation/myCollection

方法：get

参数：

user_id: 用户id；
type=news
请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=news

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

2.7.5 获取我的错题

接口地址：/studentManage/api/obj_operation/myCollection

方法：get

参数：

user_id: 用户id；
type=wrong
请求实例：http://localhost:4000/studentManage/api/obj_operation/myCollection?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=wrong

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

2.7.6 获取我关注的社区

接口地址：/studentManage/api/obj_operation/myFocus

方法：get

参数：

user_id: 用户id；
type=coummunity
请求实例：http://localhost:4000/studentManage/api/obj_operation/myFocus?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=coummunity

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

2.7.7 获取我关注的新闻标签

接口地址：/studentManage/api/obj_operation/myFocus

方法：get

参数：

user_id: 用户id；
type=subscription
请求实例：http://localhost:4000/studentManage/api/obj_operation/myFocus?user_id=2fc48bd0-a62c-11e5-9a32-a31e4e4cd6a5&type=subscription

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

2.7.8 用户登录

接口地址：/studentManage/api/user/login

方法：post

参数：

account: 账号（例如：wuwanyu_321@163.com）；
psw: 密码（例如： 123）
请求实例：http://localhost:4000/studentManage/api/user/login

登录成功 { "code": "200", "msg": "登录成功！", "user": { "user_id": "6a3eb1f0-ad2f-11e5-9ec1-cbdc2e34acc2", "name": "wuwanyu", "psw": "123", "account": "wuwanyu_321@163.com", "school": "西北大学", "major": "软件工程", "points": "10", "datems": null, "type": "student", "icon": "/files/image/Tulips.jpg", "desc": null, "createdAt": "2015-12-28T06:52:57.000Z", "updatedAt": "2015-12-28T06:52:57.000Z", "id": 4 } }
登录失败：密码输入错误 { "code": "203", "msg": "密码输入错误！" }
登录失败：账号不存在 { "code": "202", "msg": "账号不存在！" }

2.7.9 用户注册

接口地址：/studentManage/api/user/reg

方法：post

参数：(form-data)

account: 账号，例如：HerryPoter@163.com
- name: 用户名，例如：HerryPoter
psw:密码，例如： 111111
school: 学校，例如：哈佛大学（非必须）
major: 专业，例如：魔法专业（非必须）
icon: 用户头像，图片文件
请求实例：http://localhost:4000/studentManage/api/user/reg

注册成功 { "code": "200", "msg": "注册成功！", "item": { "account": "HerryPoter@163.com", "psw": "111111", "name": "HerryPoter", "school": "哈佛大学", "major": "魔法专业", "icon": "http://120.25.124.68:4000/upload/image/Koala.jpg", "user_id": "c7318520-dbd0-11e5-85bf-7b6030e90180", "points": "10", "datems": "1456412200184", "type": "student", "createdAt": "2016-02-25T15:02:24.629Z", "updatedAt": "2016-02-25T15:02:24.629Z", "id": 10 } }
注册失败：账号已经存在 { "code": "400", "msg": "该账号已经注册！" }

2.7.10 查看某人主页

接口地址：/studentManage/api/user/getOneHomePage

方法：get

参数：

user_id : 用户ID

请求实例：http://localhost:4000/studentManage/api/user/getOneHomePage?user_id=39ccddf0-dfaa-11e5-834e-a3924c9e9477

{
  "code": "200",
  "msg": "获取列表成功！",
  "info": {
    "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
    "name": "wuwanyu",
    "psw": "123",
    "account": "18233561907",
    "school": "东北大学",
    "major": "通信工程",
    "points": 12,
    "datems": "1450514441486",
    "type": "student",
    "icon": null,
    "desc": null,
    "createdAt": "2015-12-19T08:42:31.000Z",
    "updatedAt": "2016-09-12T12:40:55.000Z",
    "id": 3
  },
  "postList": [
    {
      "id": 34,
      "post_id": "e1e1a9e0-78e7-11e6-8382-710908096f7b",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:53:20.000Z",
      "updatedAt": "2016-09-12T12:53:20.000Z"
    },
    {
      "id": 35,
      "post_id": "fc9ffa20-78e7-11e6-81d4-67075da56a85",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:54:05.000Z",
      "updatedAt": "2016-09-12T12:54:05.000Z"
    },
    {
      "id": 36,
      "post_id": "517ed070-78e8-11e6-a493-3904f149739f",
      "parent_id": "43210960-b2ed-11e5-a306-33448f6b146a",
      "parent_name": "医学生",
      "title": "如何评价鹏远宿舍乱收费现象",
      "content": "作为东北大学毕业生，不得不说，鹏远宿舍的做法非常过分",
      "images": "",
      "level": 0,
      "user_id": "39ccddf0-dfaa-11e5-834e-a3924c9e9477",
      "datems": "1458045290883",
      "createdAt": "2016-09-12T12:56:27.000Z",
      "updatedAt": "2016-09-12T12:56:27.000Z"
    }
  ]
}
=======

