# 进阶

## 文字指令

### 细节描述

1. 内容描述：你想要图的样子
2. 风格描述：环境、背景氛围、参考的艺术风格等
3. 构图描述：构图、镜头、焦距、景深、光线等

#### 内容描述

画面的主体（人/动物/建筑/风景）

#### 风格描述

环境是室内或者室外的自然场景；风格是真实照片或者插画

#### 构图描述

俯瞰图birds-eye view或者脸部特写headshot；合适的相机镜头和焦距；合适的景深来控制画面的主题位置；

### 参数描述

参数描述：图片质量、图片尺寸比例、使用的模型、seed等

* 自定义尺寸比例，`--ar 3:2`宽比高
* 模型v4或者v5，`--v 4`当前最高v5版本
* 图片文字权重，`--iw 2`范围

### 细节描述的方法

**人或者物:**&#x20;

person, animal, character, location, object, etc. 人、动物、人物、地点、物体等。

**图片载体形式:**&#x20;

photo, painting, illustration, sculpture, doodle, tapestry, etc. 照片、绘画、插图、雕塑、涂鸦、挂毯等。

**环境:**&#x20;

indoors, outdoors, on the moon, in Narnia, underwater, the Emerald City, etc. 室内、室外、月球上、纳尼亚、水下、翡翠城等。

**光:**&#x20;

soft, ambient, overcast, neon, studio lights, etc 柔和、环境、阴天、霓虹灯、工作室灯等

**颜色:**&#x20;

vibrant, muted, bright, monochromatic, colorful, black and white, pastel, etc. 充满活力、柔和、明亮、单色、彩色、黑白、柔和等。

**情绪:**&#x20;

Sedate, calm, raucous, energetic, etc. 稳重、平静、喧闹、精力充沛等。

**构图:**&#x20;

Portrait, headshot, closeup, birds-eye view, etc. 人像、爆头、特写、鸟瞰图等。

### 高频参数说明

**图片比例**（横纵比， 默认1:1）

\--aspect，--ar

**混沌值**（值越高，产生的图片想象力越丰富）

\--chaos \<number 0–100>&#x20;

**删除不要的元素**

\--no&#x20;

**图片质量**（值越高质量越好，默认1）

\--quality <0.25, 0.5, 1, 2, 5> or --q <0.25, 0.5, 1, 2, 5>&#x20;

**版本**

\--version <1, 2, 3, 4, or 5> or --v <1, 2, 3, 4, or 5> 使用不同版本的 Midjourney 算法。当前算法 (V4) 是默认设置。

**新图片与参考图的相似程度**（数值范围为0\~2(--v 5情况下)，默认值为0.25，数值越大，参考原图的比重越高。）

\--iw&#x20;

**其他**

\--hd 使用早期的替代模型来生成更大、更不一致的图像。该算法可能适用于抽象和风景图像。

\--niji 另一种模型专注于动漫风格的图像。

\--style <4a, 4b or 4c> 在 Midjourney模型版本4的版本之间切换

#### 几个例子

a small boy with black eyes and dark hair , smiling , cartoon , super detailed , 8k ,HD --q 2 --uplight --v 4

Head and shoulders portrait of the couple, 8k resolution concept art, dynamic lighting hyperdetailed intricately detailed Splash art trending on ArtStation triadic colors Unreal Engine 5 volumetric lighting

A girl 10 years old standing with her mother, looking at the blue skies, it's spring, the flowers are colorful, the green space is green, they are happy, in the sky there are birds, a modren plane and the sunlight

Computer mouse made of tree roots, gorgeous, delicate, detailed, cinematic texture

## 非文字指令

### 垫图

用文字指令生成的图随机性很大，如果想生成特定风格或者个人专属的图片，可以用垫图来实现。

垫图就是给一些样板图，让midjourney来参考，或者基于这些图片去进行改造

**操作：**

1. 在对话框中点击+号按钮上传png/jpg图片
2. 鼠标右键拷贝链接（可以一次性垫多张图，图片链接间打上空格即可）
3. 添加相关文字指令

### Blend混图

和垫图原理差不多。上传多张图进行进行一个混合，生成一张全新的图。

用混图，只支持上传图片，不支持添加文字指令

**操作：**

1. 命令`/blend`

### Remix微调
