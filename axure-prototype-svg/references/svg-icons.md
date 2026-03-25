# 常用 SVG 图标库

本文档提供了一组基础、通用的 SVG 图标代码，专为 `axure-prototype-svg` 技能生成高保真原型时调用。
所有图标均遵循**极简、可缩放、纯路径 (Path/Line/Rect/Circle/Polyline/Polygon)** 的原则，确保导入 Axure 后能完美“Convert to Shapes”（转换为形状）。

**使用说明：**

- 默认尺寸：`24x24`
- 默认颜色：`#4E5969` (次文字色) 或 `currentColor`
- 使用时，请直接复制 `<svg>` 标签内部的路径，或者直接使用包含定位属性的完整 `<svg>`，并根据具体页面的视觉规范替换 `width`、`height` 和 `stroke` / `fill` 属性。
- **注意**：请勿使用复杂的 `clip-path`、`mask` 或外部 `<use>` 引用，以保证兼容性。

***

## 1. 导航与方向 (Navigation & Direction)

### 1.1 向下箭头 (Chevron Down)

常用于：下拉菜单、手风琴展开

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polyline points="6,9 12,15 18,9" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 1.2 向上箭头 (Chevron Up)

常用于：收起菜单、折叠面板

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polyline points="18,15 12,9 6,15" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 1.3 向右箭头 (Chevron Right)

常用于：列表进入下一级、面包屑分隔符

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polyline points="9,18 15,12 9,6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 1.4 向左箭头 (Chevron Left)

常用于：返回上一页

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polyline points="15,18 9,12 15,6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

***

## 2. 基础操作 (Basic Actions)

### 2.1 关闭 / 取消 (Close / X)

常用于：关闭弹窗、抽屉、清空输入框

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <line x1="18" y1="6" x2="6" y2="18" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="6" y1="6" x2="18" y2="18" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.2 搜索 / 放大镜 (Search)

常用于：搜索框图标

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="11" cy="11" r="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="15.5" y1="15.5" x2="20" y2="20" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.3 添加 / 新建 (Plus / Add)

常用于：新增按钮、添加行

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <line x1="12" y1="5" x2="12" y2="19" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="5" y1="12" x2="19" y2="12" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.4 编辑 / 铅笔 (Edit)

常用于：修改、编辑表单

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M12 20H21" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M16.5 3.5C16.8978 3.10217 17.4374 2.87868 18 2.87868C18.5626 2.87868 19.1022 3.10217 19.5 3.5C19.8978 3.89782 20.1213 4.43739 20.1213 5C20.1213 5.56261 19.8978 6.10217 19.5 6.5L7 19L3 20L4 16L16.5 3.5Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.5 删除 / 垃圾桶 (Delete / Trash)

常用于：删除行、移除项

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M3 6H21" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M19 6V20C19 20.5304 18.7768 21.0383 18.3812 21.4336C17.9855 21.8289 17.4776 22 16.9474 22H7.05263C6.52236 22 6.0145 21.8289 5.61882 21.4336C5.22315 21.0383 5 20.5304 5 20V6" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M8 6V4C8 3.46957 8.21071 2.96086 8.58579 2.58579C8.96086 2.21071 9.46957 2 10 2H14C14.5304 2 15.0391 2.21071 15.4142 2.58579C15.7893 2.96086 16 3.46957 16 4V6" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.6 复制 (Copy)
常用于：复制单号、复制链接
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="9" y="9" width="13" height="13" rx="2" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M5 15H4C3.46957 15 2.96086 14.7893 2.58579 14.4142C2.21071 14.0391 2 13.5304 2 13V4C2 3.46957 2.21071 2.96086 2.58579 2.58579C2.96086 2.21071 3.46957 2 4 2H13C13.5304 2 14.0391 2.21071 14.4142 2.58579C14.7893 2.96086 15 3.46957 15 4V5" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.7 眼睛 / 查看 (Eye)
常用于：预览、密码显示/隐藏控制
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M1 12C1 12 5 4 12 4C19 4 23 12 23 12C23 12 19 20 12 20C5 20 1 12 1 12Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <circle cx="12" cy="12" r="3" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 2.8 星星 / 收藏 (Star)
常用于：收藏、评分、重点标记
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polygon points="12,2 15.09,8.26 22,9.27 17,14.14 18.18,21.02 12,17.77 5.82,21.02 7,14.14 2,9.27 8.91,8.26" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

***

## 3. 状态与提示 (Status & Feedback)

### 3.1 成功 / 勾选 (Success / Check)

常用于：任务完成、多选框选中状态

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polyline points="20,6 9,17 4,12" stroke="#00B42A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 3.2 警告 / 提示 (Warning / Info Circle)

常用于：表单错误提示、气泡说明

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="12" r="10" stroke="#FF7D00" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="12" y1="8" x2="12" y2="12" stroke="#FF7D00" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="12" y1="16" x2="12.01" y2="16" stroke="#FF7D00" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

```

### 3.3 错误 / 阻止 (Error / X Circle)

常用于：操作失败、禁止状态

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="12" r="10" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="15" y1="9" x2="9" y2="15" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="9" y1="9" x2="15" y2="15" stroke="#F53F3F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

***

## 4. 业务场景 (Business Scenarios)

### 4.1 日历 / 日期 (Calendar)

常用于：日期选择器

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="3" y="4" width="18" height="18" rx="2" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="16" y1="2" x2="16" y2="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="2" x2="8" y2="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="10" x2="21" y2="10" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 4.2 时钟 / 历史 (Clock)
常用于：操作日志、处理时长、定时任务
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="12" r="10" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="12,6 12,12 16,14" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 4.3 提醒 / 闹钟 (Alarm Clock)
常用于：时间提醒、定时通知、倒计时
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="13" r="8" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="12,9 12,13 15,15" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="5" y1="3" x2="7" y2="5" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="19" y1="3" x2="17" y2="5" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 4.4 地址 / 定位 (Location / Map Pin)
常用于：收货地址、地图定位、门店位置
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21 10C21 17 12 23 12 23C12 23 3 17 3 10C3 7.61305 3.94821 5.32387 5.63604 3.63604C7.32387 1.94821 9.61305 1 12 1C14.3869 1 16.6761 1.94821 18.364 3.63604C20.0518 5.32387 21 7.61305 21 10Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <circle cx="12" cy="10" r="3" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 4.5 更多 / 省略号 (More / Ellipsis Horizontal)

常用于：表格操作列、更多菜单

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="5" cy="12" r="1.5" fill="#4E5969"/>
  <circle cx="12" cy="12" r="1.5" fill="#4E5969"/>
  <circle cx="19" cy="12" r="1.5" fill="#4E5969"/>
</svg>
```

### 4.6 视频播放 (Play Video)

常用于：视频资源卡片、开始播放按钮

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="12" r="10" stroke="#1677FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polygon points="10,8 16,12 10,16" stroke="#1677FF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" fill="#1677FF"/>
</svg>
```

### 4.7 刷新 / 重置 (Refresh)

常用于：刷新列表、重新获取数据

```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21 12C21 16.9706 16.9706 21 12 21C7.02944 21 3 16.9706 3 12C3 7.02944 7.02944 3 12 3C15.5458 3 18.6117 5.0453 20 8" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="21,3 21,8 16,8" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

---

## 5. 文件与数据 (File & Data)

### 5.1 文档 / 报告 (Document)
常用于：文件列表、报告详情
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M14 2H6C4.89543 2 4 2.89543 4 4V20C4 21.1046 4.89543 22 6 22H18C19.1046 22 20 21.1046 20 20V8L14 2Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M14 2V8H20" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="13" x2="16" y2="13" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="17" x2="16" y2="17" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 5.2 图片 / 照片 (Image)
常用于：图片占位、上传头像、相册
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="3" y="3" width="18" height="18" rx="2" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <circle cx="8.5" cy="8.5" r="1.5" fill="#4E5969"/>
  <polyline points="21,15 16,10 5,21" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 5.3 附件 / 回形针 (Attachment / Paperclip)
常用于：上传附件、文件链接
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21.44 11.05L12.25 20.24C11.1242 21.3658 9.59728 21.9983 8.005 21.9983C6.41272 21.9983 4.88582 21.3658 3.76 20.24C2.63418 19.1142 2.00171 17.5873 2.00171 15.995C2.00171 14.4027 2.63418 12.8758 3.76 11.75L12.95 2.56C13.7006 1.80943 14.7186 1.38776 15.78 1.38776C16.8414 1.38776 17.8594 1.80943 18.61 2.56C19.3606 3.31057 19.7822 4.32856 19.7822 5.39C19.7822 6.45144 19.3606 7.46943 18.61 8.22L9.42 17.41C9.04471 17.7853 8.53571 17.9961 8.005 17.9961C7.47429 17.9961 6.96529 17.7853 6.59 17.41C6.21471 17.0347 6.00391 16.5257 6.00391 15.995C6.00391 15.4643 6.21471 14.9553 6.59 14.58L15.07 6.1" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 5.4 下载 / 导出 (Download)
常用于：导出报表、下载文件
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21 15V19C21 19.5304 20.7893 20.0391 20.4142 20.4142C20.0391 20.7893 19.5304 21 19 21H5C4.46957 21 3.96086 20.7893 3.58579 20.4142C3.21071 20.0391 3 19.5304 3 19V15" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="7,10 12,15 17,10" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="12" y1="15" x2="12" y2="3" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 5.5 上传 / 导入 (Upload)
常用于：上传文件
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21 15V19C21 19.5304 20.7893 20.0391 20.4142 20.4142C20.0391 20.7893 19.5304 21 19 21H5C4.46957 21 3.96086 20.7893 3.58579 20.4142C3.21071 20.0391 3 19.5304 3 19V15" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="17,8 12,3 7,8" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="12" y1="3" x2="12" y2="15" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

---

## 6. 用户与组织 (User & Organization)

### 6.1 用户 / 个人 (User)
常用于：个人中心、账号管理、医生/患者占位
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="12" cy="7" r="4" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M4 21C4 17.134 7.58172 14 12 14C16.4183 14 20 17.134 20 21" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 6.2 团队 / 多人 (Users)
常用于：租户管理、机构管理、团队列表
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <circle cx="9" cy="7" r="4" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M1 21C1 17.134 4.58172 14 9 14C13.4183 14 17 17.134 17 21" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M16 3.13C17.53 3.53 18.66 4.9 18.66 6.5C18.66 8.1 17.53 9.47 16 9.87" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M23 21C23 18.06 21.03 15.53 18.33 14.47" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 6.3 退出登录 (Log Out)
常用于：顶部栏退出操作
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M9 21H5C4.46957 21 3.96086 20.7893 3.58579 20.4142C3.21071 20.0391 3 19.5304 3 19V5C3 4.46957 3.21071 3.96086 3.58579 3.58579C3.96086 3.21071 4.46957 3 5 3H9" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <polyline points="16,17 21,12 16,7" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="21" y1="12" x2="9" y2="12" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

---

## 7. 系统与设置 (System & Settings)

### 7.1 设置 / 齿轮 (Settings)
常用于：系统设置、配置中心
```svg
<svg width="24" height="24" viewBox="0 0 1024 1024" fill="#4E5969" xmlns="http://www.w3.org/2000/svg">
  <path d="M663.04 108.544l118.784 69.632c-5.632 34.304-13.824 111.616 16.896 165.888 31.744 55.808 105.472 88.064 137.216 99.328 3.072 19.968 6.144 48.64 6.144 69.12 0 18.944-3.072 46.592-6.144 69.12-32.256 11.776-104.96 43.52-137.216 99.84-31.232 54.784-23.04 132.096-16.896 165.888l-118.784 69.632c-28.16-23.04-89.088-67.584-150.528-67.584-61.952 0-123.904 45.056-151.04 67.584L242.176 847.872c5.632-34.304 13.824-111.616-16.896-165.888-31.744-55.808-105.472-88.064-137.216-99.328-3.072-19.968-6.144-48.64-6.144-69.12 0-18.944 3.072-46.592 6.144-69.12 32.256-11.776 104.96-43.52 137.216-99.84 31.232-54.784 22.528-131.584 16.896-165.888l118.784-69.632c28.16 23.04 89.088 67.584 150.528 67.584 61.952 0 123.904-45.056 151.552-68.096m-2.048-87.04c-14.848 0-30.208 5.632-40.96 15.872-15.872 14.848-69.632 57.344-108.032 57.344-38.4 0-92.16-42.496-108.032-57.344-10.752-10.24-26.112-15.872-40.96-15.872-7.68 0-15.872 1.536-23.04 4.608L184.832 117.248l-3.072 2.048c-17.92 13.312-27.136 38.912-22.528 61.44 5.12 20.992 14.336 89.6-5.12 123.392C135.168 337.92 71.68 363.52 51.2 370.176c-20.48 6.656-38.4 26.624-41.984 48.128-0.512 2.56-9.216 55.808-9.216 94.72s8.704 92.672 9.216 94.72c3.584 21.504 21.504 41.984 41.984 48.128 20.48 6.656 83.968 32.768 102.912 66.048 18.944 33.792 9.728 101.888 5.12 123.392-5.12 22.016 4.608 47.616 22.528 61.44L336.896 998.4l3.072 1.536c7.168 3.072 14.848 4.608 23.04 4.608 14.848 0 30.208-5.632 40.96-15.872 15.872-14.848 69.632-57.344 108.032-57.344 38.4 0 92.16 42.496 108.032 57.344 10.752 9.728 26.112 15.36 40.96 15.36 7.68 0 15.872-1.536 23.04-4.608l155.136-90.624 3.072-2.048c17.92-13.312 27.136-39.424 22.528-61.44-5.12-20.992-14.336-89.6 5.12-123.392 18.944-33.792 82.432-59.904 102.912-66.048 20.48-6.656 38.4-26.624 41.984-48.128 0.512-2.56 9.216-55.808 9.216-94.72s-8.704-92.672-9.216-94.72c-3.584-21.504-21.504-41.984-41.984-48.128-20.48-6.656-83.968-32.768-102.912-66.048-18.944-33.792-9.728-101.888-5.12-123.392 5.12-22.016-4.608-47.616-22.528-61.44L687.104 27.648l-3.072-1.536c-7.168-3.072-15.36-4.608-23.04-4.608zM512 369.664c78.848 0 143.36 64.512 143.36 143.36s-64.512 143.36-143.36 143.36-143.36-64.512-143.36-143.36 64.512-143.36 143.36-143.36m0-81.92c-124.416 0-225.28 100.864-225.28 225.28s100.864 225.28 225.28 225.28 225.28-100.864 225.28-225.28-100.864-225.28-225.28-225.28z"/>
</svg>
```

### 7.2 锁定 / 安全 (Lock)
常用于：权限限制、锁定状态、密码修改
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="3" y="11" width="18" height="11" rx="2" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M7 11V7C7 5.67392 7.52678 4.40215 8.46447 3.46447C9.40215 2.52678 10.6739 2 12 2C13.3261 2 14.5979 2.52678 15.5355 3.46447C16.4732 4.40215 17 5.67392 17 7V11" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 7.3 首页 / 房子 (Home)
常用于：面包屑首页、底部导航栏
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M9 22V12H15V22" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 7.4 链接 / 绑定 (Link)
常用于：设备绑定、复制链接
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M10 13A5 5 0 0 0 17 13L20.5 9.5A5 5 0 0 0 13.5 2.5L11 5" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M14 11A5 5 0 0 0 7 11L3.5 14.5A5 5 0 0 0 10.5 21.5L13 19" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

---

## 8. 通讯与客服 (Communication & Support)

### 8.1 电话 / 拨打 (Phone)
常用于：联系患者、呼叫坐席
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M22 16.92V21C22 21.55 21.55 22 21 22C10.5 22 2 13.5 2 3C2 2.45 2.45 2 3 2H7.08C7.55 2 7.95 2.34 8.05 2.8L9.22 5.54C9.32 5.76 9.28 6.01 9.11 6.18L7.37 7.92C9.14 11.03 12.97 14.86 16.08 16.63L17.82 14.89C17.99 14.72 18.24 14.68 18.46 14.78L21.2 15.95C21.66 16.05 22 16.45 22 16.92Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 8.2 消息 / 聊天 (Message)
常用于：站内信、在线客服、意见反馈
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M21 15C21 15.5304 20.7893 16.0391 20.4142 16.4142C20.0391 16.7893 19.5304 17 19 17H7L3 21V5C3 4.46957 3.21071 3.96086 3.58579 3.58579C3.96086 3.21071 4.46957 3 5 3H19C19.5304 3 20.0391 3.21071 20.4142 3.58579C20.7893 3.96086 21 4.46957 21 5V15Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 8.3 摄像头 / 录像 (Camera)
常用于：发起视频见证、录音录像状态
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M23 7L16 12L23 17V7Z" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <rect x="1" y="5" width="15" height="14" rx="2" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 8.4 麦克风 / 语音 (Microphone)
常用于：语音输入、静音/解除静音控制
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="9" y="2" width="6" height="12" rx="3" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M19 10V12C19 15.866 15.866 19 12 19C8.13401 19 5 15.866 5 12V10" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="12" y1="19" x2="12" y2="22" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="22" x2="16" y2="22" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

---

## 9. 界面布局 (Layout & UI)

### 9.1 菜单 / 汉堡图标 (Menu)
常用于：移动端展开侧边栏
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <line x1="3" y1="12" x2="21" y2="12" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="6" x2="21" y2="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="18" x2="21" y2="18" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 9.2 列表视图 (List View)
常用于：切换到列表展示模式
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <line x1="8" y1="6" x2="21" y2="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="12" x2="21" y2="12" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="8" y1="18" x2="21" y2="18" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="6" x2="3.01" y2="6" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="12" x2="3.01" y2="12" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <line x1="3" y1="18" x2="3.01" y2="18" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 9.3 网格视图 / 卡片视图 (Grid View)
常用于：切换到卡片展示模式
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect x="3" y="3" width="7" height="7" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <rect x="14" y="3" width="7" height="7" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <rect x="14" y="14" width="7" height="7" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  <rect x="3" y="14" width="7" height="7" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 9.4 过滤 / 漏斗 (Filter)
常用于：列表的高级筛选入口
```svg
<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
  <polygon points="22,3 2,3 10,12.46 10,19 14,21 14,12.46 22,3" stroke="#4E5969" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```
