# 三种大小

- order: 1

三种大小的输入框，大的用在表单中，中的为默认。

---

````jsx
var Datepicker = antd.Datepicker;

React.render(
  <div>
    <Datepicker size="lg" />
    <Datepicker />
    <Datepicker size="sm" />
  </div>
, document.getElementById('components-datepicker-demo-size'));
````