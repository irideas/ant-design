# 自定义关闭按钮

- order: 4

自定义关闭按钮的样式和文字。

---

````jsx
var notification = require('antd/lib/notification');

var key = 'someKeyStringString';

var close = function() {
  notification.close(key);
};

var btn = <button onClick={close} className="ant-btn ant-btn-primary ant-btn-sm">自定义关闭按钮</button>;

var openNotification = function() {
  notification.open({
    message: "这是标题",
    description: "这是提示框的文案这是提示框示框的文案这是提示是提示框的文案这是提示框的文案",
    btn: btn,
    key: key
  });
};

React.render(
  <div>
    <button className="ant-btn ant-btn-primary" onClick={openNotification}>打开通知提醒框</button>
  </div>,
document.getElementById('components-notification-demo-with-btn'));
````