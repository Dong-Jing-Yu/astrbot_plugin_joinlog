<div align="center">

# astrbot_plugin_grouplog

</div>



```json
event.message_obj.raw_message (AIOCQHTTP)

进群申请(发送验证信息)(未进)
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'request', 'request_type': 'group', 'group_id': 目标群, 'user_id': 目标用户, 'comment': 'xxx', 'flag': '标志', 'sub_type': 'add'}> 

进群(审核)(未进)
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'request', 'request_type': 'group', 'group_id': 目标群, 'user_id': 目标用户, 'comment': '问题：xxx\n答案：xxx', 'flag':'标志', 'sub_type': 'add'}>

邀请进群(进入)
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'notice', 'group_id': 目标群, 'user_id': 目标用户, 'notice_type': 'group_increase', 'operator_id': 操作人, 'sub_type': 'invite'}>

同意进群(进入)
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'notice', 'group_id': 目标群, 'user_id': 目标用户, 'notice_type': 'group_increase', 'operator_id': 操作人, 'sub_type': 'approve'}>

自行退群
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'notice', 'group_id': 目标群, 'user_id': 目标用户, 'notice_type': 'group_decrease', 'sub_type': 'leave', 'operator_id': 0}>

被踢出
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'notice', 'group_id': 目标群, 'user_id': 目标用户, 'notice_type': 'group_decrease', 'sub_type': 'kick', 'operator_id': 操作人}>

管理员撤回消息
<Event, {'time': 时间戳, 'self_id': 自己的id, 'post_type': 'notice', 'group_id': 目标群, 'user_id': 目标用户, 'notice_type': 'group_recall', 'operator_id': 操作人, 'message_id': id}
```