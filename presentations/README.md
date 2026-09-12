# 使用说明

本目录包含用于生成 PPTX 的脚本与幻灯片内容（占位图/文本）。

文件说明：
- generate_pptx.py：使用 python-pptx 读取 slides_content.json 并生成 PPTX 文件。
- slides_content.json：包含 17 页幻灯片的文本内容（JSON 格式）。

生成步骤：
1. 在本地环境准备 Python（3.8+ 推荐）。
2. 安装依赖：
   pip install python-pptx
3. 运行脚本：
   python presentations/generate_pptx.py
4. 生成文件位于 presentations_output/ 基建山河_解码中国地形_地形篇.pptx

说明与后续替换：
- 目前幻灯片中使用的是文本与占位布局；如需嵌入更精美的地图、剖面图与科考插画，请把图片上传到仓库并在 slides_content.json 中为相应幻灯片添加字段 "image": "path/to/image.png"，然后调整脚本以按位置插入图片。
- 如果你希望我直接将已生成的 PPTX 上传到仓库，请允许我运行生成脚本并上传二进制文件（当前环境无法直接在服务器端生成二进制并返回给你），因此我提供了此脚本以便你在本地或 CI 环境中快速生成成品。

如需我把脚本调整为支持插入图片位置、字体或模板细节，请告诉我具体需求，我会修改脚本并再次提交。
