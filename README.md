# About-SceneKit
关于iOS游戏库，SceneKit的使用

>SKView的中心坐标在屏幕中间，一个二位坐标系。

##关于SKView的ignoresSiblingOrder属性：(可以理解为多个图层，根据z轴的大小分层)
>>当 ignoresSiblingOrder 为 false 时，SpriteKit 会按照节点在其父节点的 children 数组中的顺序呈现节点——也就是说，数组顺序决定了哪个绘制“在“另一个。这也意味着 SpriteKit 必须一次渲染每个节点，因此 OpenGL 绘制调用开销会降低效率。
>>当 ignoresSiblingOrder 为真时，SpriteKit 完全依赖于 zPosition 属性来确定绘制的顺序。这意味着它有时可以将同一 z 处的所有内容组合成一次绘制，这使得渲染速度更快。但这也意味着如果你想控制哪些节点绘制在其他节点之前，你需要适本地设置它们的 zPosition。
