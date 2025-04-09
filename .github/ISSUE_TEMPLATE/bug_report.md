name: 🐛 Bug 报告
description: 报告项目中遇到的 Bug
labels: [bug]
body:
  - type: markdown
    attributes:
      value: |
        感谢你的反馈！请尽可能填写完整以下信息。

  - type: input
    id: title
    attributes:
      label: Bug 标题
      description: 简洁描述你遇到的问题
      placeholder: 例如：登录页面提交按钮无响应
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: 描述
      description: 请详细描述你遇到的问题
      placeholder: 包括操作步骤、实际结果、期望结果等
    validations:
      required: true

  - type: input
    id: url
    attributes:
      label: 出错的请求地址（可选）
      placeholder: 例如：https://yourdomain.com/user/login

  - type: textarea
    id: logs
    attributes:
      label: 异常堆栈或日志（可选）
      placeholder: 贴上后端返回的错误信息或控制台日志

  - type: input
    id: env
    attributes:
      label: 环境信息（可选）
      placeholder: 系统、浏览器、版本等
