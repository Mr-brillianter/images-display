# [图片提示词查看器](https://mr-brillianter.github.io/images-display/)

## 项目简介

这是一个用于查看和标记图片的Web应用程序。用户可以加载包含图片和提示词的目录，对图片进行查看、标记（Good、Perfect、Abandon），并将标记结果导出为CSV文件。

## 主要功能

- 加载并显示图片和对应的提示词
- 支持图片标记（Good、Perfect、Abandon）
- 标记结果自动保存到本地存储
- 支持按标记类型筛选图片
- 支持导出标记结果为标准CSV文件
- 优化显示1024x1216尺寸的图片

## 目录结构要求

应用程序需要读取特定格式的目录结构：

```
autoruns/
├── 0/
│   ├── prompt.txt  (包含提示词文本)
│   └── image.png   (对应的图片文件)
├── 1/
│   ├── prompt.txt
│   └── image.png
├── 2/
│   ├── prompt.txt
│   └── image.png
...
└── 38/
    ├── prompt.txt
    └── image.png
```

## 使用方法

1. 打开`image_viewer.html`文件
2. 点击"选择autoruns目录"按钮
3. 选择包含上述结构的目录
4. 浏览图片并添加标记
5. 使用顶部的过滤按钮筛选图片
6. 点击"导出标记表格"按钮导出CSV文件

## 技术说明

- 使用原生JavaScript开发
- 使用File System Access API读取本地文件
- 使用LocalStorage保存标记数据
- 支持标准CSV格式导出

## English Description

### Project Overview

This is a web application for viewing and tagging images. Users can load directories containing images and their corresponding prompts, view and tag images (Good, Perfect, Abandon), and export tagging results to CSV files.

### Main Features

- Load and display images along with their prompts
- Support image tagging (Good, Perfect, Abandon)
- Automatically save tagging results to local storage
- Filter images by tag type
- Export tagging results to standard CSV format
- Optimized display for 1024x1216 images

### Directory Structure Requirements

The application requires a specific directory structure:

```
autoruns/
├── 0/
│   ├── prompt.txt  (contains prompt text)
│   └── image.png   (corresponding image file)
├── 1/
│   ├── prompt.txt
│   └── image.png
├── 2/
│   ├── prompt.txt
│   └── image.png
...
└── 38/
    ├── prompt.txt
    └── image.png
```

### Usage

1. Open `image_viewer.html` file
2. Click the "Select autoruns directory" button
3. Choose a directory with the above structure
4. Browse images and add tags
5. Use the filter buttons at the top to filter images
6. Click the "Export Tag Table" button to export CSV file

### Technical Details

- Developed using native JavaScript
- Uses File System Access API to read local files
- Uses LocalStorage to save tagging data
- Supports standard CSV format export

