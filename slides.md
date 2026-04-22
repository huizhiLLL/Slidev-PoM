---
theme: default
title: AI 大范围发展下生产力与生产关系的再审视
info: |
  基于《马克思主义基本原理》第三章的分析
fonts:
  sans: Noto Serif SC
  serif: Noto Serif SC
  mono: Fira Code
layout: center
class: text-center
transition: fade
---

<style>
:root {
  --slidev-theme-primary: #2c3e50;
  --text-color: #333333;
  --heading-color: #1a252f;
  --bg-color: #fafafa;
  --accent-red: #8b0000;
  --accent-blue: #2f5d7c;
  --border-light: #e0e6ed;
}

body {
  font-family: 'Noto Serif SC', 'Source Han Serif SC', 'SimSun', serif;
  color: var(--text-color);
  background-color: var(--bg-color);
}

h1, h2, h3, h4 {
  color: var(--heading-color);
  font-weight: 600;
  letter-spacing: 0.05em;
  margin-bottom: 0.9rem;
}

h1 {
  font-size: 3rem;
  line-height: 1.2;
  max-width: 90%;
  margin-left: auto;
  margin-right: auto;
  font-weight: 700;
}

h1.cover-title {
  max-width: none !important;
  font-size: 1em !important;
  line-height: 1.15 !important;
}

h1.cover-title .title-line {
  display: block;
  white-space: nowrap;
}

h1.cover-title .title-line:first-child {
  font-size: 3.6rem !important;
}

h1.cover-title .title-line:last-child {
  font-size: 3rem !important;
}

h2 {
  font-size: 2.15rem;
  border-bottom: 1px solid var(--border-light);
  padding-bottom: 0.45rem;
  display: inline-block;
}

h3 {
  font-size: 1.18rem;
}

p, li {
  font-size: 1.15rem;
  line-height: 1.7;
}

ul {
  line-height: 1.7;
  padding-left: 1.2rem;
}

li {
  margin-bottom: 0.35rem;
}

.layout-grid {
  display: grid;
  gap: 1.1rem;
  margin-top: 1rem;
  text-align: left;
}

.grid-2 { grid-template-columns: 1fr 1fr; }
.grid-3 { grid-template-columns: 1fr 1fr 1fr; }

.img-placeholder {
  background: #f1f4f8;
  border: 1px dashed #b0bec5;
  border-radius: 6px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #6c7a80;
  font-size: 0.88rem;
  min-height: 120px;
  text-align: center;
  padding: 0.8rem;
}

.img-placeholder.small {
  min-height: 72px;
}

.img-placeholder.medium {
  min-height: 180px;
}

.img-placeholder.large {
  min-height: 240px;
}

.box {
  background: #ffffff;
  border: 1px solid var(--border-light);
  border-radius: 8px;
  padding: 0.95rem 1.1rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.03);
}

.accent-quote {
  border-left: 4px solid var(--slidev-theme-primary);
  padding-left: 1rem;
  color: #34495e;
  margin-top: 1rem;
  text-align: left;
  font-size: 1.1rem;
  line-height: 1.65;
}

.flow-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 0.6rem;
  margin-top: 1rem;
}

.flow-box {
  flex: 1;
  text-align: center;
  padding: 0.75rem 0.6rem;
  background: #ffffff;
  border: 1px solid var(--border-light);
  border-radius: 8px;
  font-weight: 600;
  font-size: 1rem;
}

.flow-arrow {
  font-size: 1.3rem;
  color: #7f8c8d;
}

.highlight {
  color: var(--accent-red);
  font-weight: 600;
}

.blue {
  color: var(--accent-blue);
  font-weight: 600;
}

.small-note {
  font-size: 0.88rem;
  color: #66727d;
  line-height: 1.5;
}

.tag-row {
  display: flex;
  justify-content: center;
  gap: 0.75rem;
  flex-wrap: wrap;
  margin-top: 1.2rem;
}

.tag {
  border: 1px solid var(--border-light);
  background: white;
  padding: 0.35rem 0.8rem;
  border-radius: 999px;
  font-size: 1.05rem;
}

.section-label {
  color: #7a8691;
  font-size: 0.95rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  margin-bottom: 0.8rem;
}

/* 内容密集页专用：进一步压缩间距 */
.dense h3 { margin-bottom: 0.5rem; }
.dense li { margin-bottom: 0.2rem; }
.dense p, .dense li { font-size: 1rem; line-height: 1.6; }
.dense .box { padding: 0.75rem 0.9rem; }
.dense .accent-quote { margin-top: 0.7rem; font-size: 1rem; }

.intro-hero-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
  margin-top: 1rem;
}

.intro-hero-card {
  background: #ffffff;
  border: 1px solid var(--border-light);
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 18px rgba(0, 0, 0, 0.05);
}

.intro-hero-visual {
  min-height: 290px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 1.2rem;
  font-size: 1.02rem;
  line-height: 1.7;
}

.intro-hero-visual.left {
  background: linear-gradient(135deg, #eef4fb 0%, #f8fbff 100%);
  color: #35506b;
}

.intro-hero-visual.right {
  background: linear-gradient(135deg, #fff3f2 0%, #fffaf8 100%);
  color: #7a4540;
}

.intro-hero-label {
  padding: 0.8rem 1rem;
  font-size: 1rem;
  font-weight: 600;
  text-align: center;
  background: #ffffff;
}

</style>

<div v-motion-slide-visible-bottom>
  <h1 class="cover-title">
    <span class="title-line">AI 大范围发展下</span>
    <span class="title-line">生产力与生产关系的再审视</span>
  </h1>
  <p class="text-2xl text-gray-600 ml-80">—— 基于《马克思主义基本原理》第三章的分析</p>
</div>

<div class="text-gray-900 text-xl mt-12" v-motion-fade-visible>
  小组成员：陈诺 黄宇镐 李冀斌 胡泽亮<br>
  汇报日期：2026.4.27
</div>

---
transition: fade
---

<h1>一. 导入——AI 时代的十字路口</h1>

<div class="intro-hero-grid" style="margin-top: 1rem;">
  <div class="intro-hero-card">
    <div class="intro-hero-visual left">
      <img src="\assets\3.png">
    </div>
    <div class="intro-hero-label blue">生产力正在快速跃升</div>
  </div>

  <div class="intro-hero-card">
    <div class="intro-hero-visual right">
      <img src="\assets\1.png"
    </div>
    <div class="intro-hero-label highlight">垄断风险与就业压力同步上升</div>
  </div>
</div>

---
transition: fade
---

<h1>一. 导入——AI 时代的十字路口</h1>

<div class="layout-grid grid-2 dense" style="margin-top: 1rem;">
  <div>
    <h3 class="text-center blue">生产力正在快速跃升</h3>
    <ul class="mt-2">
      <li>高保真图像、视频、音乐与医疗辅助等领域持续突破，不断拓展技术边界</li>
      <li>新的先进生产力形态正在迅速成形</li>
    </ul>
  </div>

  <div>
    <h3 class="text-center highlight">垄断风险与就业压力同步上升</h3>
    <ul class="mt-2">
      <li>AI 正在重组知识劳动任务结构，对部分岗位和入门机会形成压力</li>
      <li>对 AI 使用方式与定价机制的决定权，正日益集中于少数平台与资本主体</li>
    </ul>
  </div>
</div>

<div class="accent-quote dense">
  AI 时代呈现出鲜明张力：生产力快速跃升，并不意味着共享型分配关系已经同步形成。
</div>

<div class="layout-grid grid-2 dense" style="margin-top: 0.7rem;">
  <div class="box">
    <h3 class="text-center">分析对象超出技术表层</h3>
    <p>若只着眼于模型能力与算力竞赛，只能把握技术表面。真正决定社会后果的，是技术被嵌入了何种社会关系之中。</p>
  </div>

  <div class="box">
    <h3 class="text-center">马克思主义理论框架</h3>
    <p>《马克思主义基本原理》第三章提供了理解 AI 的理论视角。<span class="highlight">核心在于：生产力与生产关系的矛盾运动。</span></p>
  </div>
</div>

---
transition: slide-up
---

# 二. 理论框架的当代适用<br>——生产力三要素的深刻变革

<br>
<div class="layout-grid grid-3 dense" style="margin-top: 1.4rem;">
  <div class="box" v-click>
    <h3>劳动者</h3>
    <ul class="mt-2">
      <li>劳动者结构正在扩展，不再局限于传统知识劳动者。</li>
      <li>提示词设计、数据标注、模型评测、AI 运维与合规等岗位正在上升。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3>劳动资料</h3>
    <ul class="mt-2">
      <li>算力基础设施、算法模型和数据平台成为关键劳动资料。</li>
      <li>这套新的劳动资料，正在决定生产过程的进入门槛和控制能力。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3>劳动对象</h3>
    <ul class="mt-2">
      <li>数据正在成为关键生产要素，也是重要劳动对象之一。</li>
      <li>数字经济时代的"原料"，越来越表现为可计算的数据资源。</li>
    </ul>
  </div>
</div>
<br>

<div class="accent-quote dense" v-click>
  AI 并非"新问题可以抛开旧理论"，恰恰相反——它是经典理论框架在数字时代的新检验场。
</div>

---
transition: fade
---

# 核心命题：生产资料控制权的归属

<br>
<div class="flow-container" v-click>
  <div class="flow-box">算力</div>
  <div class="flow-arrow">+</div>
  <div class="flow-box">模型</div>
  <div class="flow-arrow">+</div>
  <div class="flow-box">平台入口</div>
  <div class="flow-arrow">+</div>
  <div class="flow-box">数据资源</div>
</div>

<div class="layout-grid grid-2 mt-8">
  <div class="box" v-click>
    <h3 class="text-center">问题已超出"技术强弱"本身</h3>
    <ul>
      <li>数据成为关键原料、算力成为核心工具后，控制权归属成为核心问题。</li>
      <li>控制权体现于算力、模型、平台入口与数据资源的占有方式。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">这正是生产关系问题</h3>
    <ul>
      <li>分析对象不只是 AI 这一生产力形态本身。</li>
      <li class="highlight">更包括其嵌入的所有制结构、治理规则与收益分配方式。</li>
    </ul>
  </div>
</div>

---
transition: slide-left
---

# 三. AI 的"一体两面"——<br><br>面向一：<span class="highlight">通往自由王国之路</span>

<div class="layout-grid grid-2">
  <div v-click>
    <p>
      马克思认为，只有当生产力高度发达、物质财富充裕涌流时，共产主义才具备实现的物质前提。
    </p>
    <ul class="mt-3">
      <li>AI 是近年来最具代表性的先进生产力形态之一</li>
      <li>它显著压缩了部分重复性认知任务所需时间</li>
      <li>"必要劳动时间减少、自由时间增加"在现实层面具有了更高的可能性</li>
    </ul>
    <br>
    <strong class="text-2xl">现实可能性并不等于现实结果</strong>
  </div>

  <div v-click>
    <div class="img-placeholder medium">
<img src="\assets\4.png">
    </div>
  </div>
</div>

---
transition: slide-left
---

# 生产社会化的体现与知识劳动的流程重组

<div class="flow-container" v-click>
  <div class="flow-box">
    全球化算力<br>
    <span class="small-note">训练与推理依赖跨地域基础设施</span>
  </div>
  <div class="flow-arrow">+</div>
  <div class="flow-box">
    互联网规模数据<br>
    <span class="small-note">公共语料与海量交互不断沉淀</span>
  </div>
  <div class="flow-arrow">+</div>
  <div class="flow-box">
    开源代码生态<br>
    <span class="small-note">框架、工具链与社区协作共同演化</span>
  </div>
</div>

<div class="layout-grid grid-2 mt-6">
  <div class="box" v-click>
    <h3 class="text-center">被压缩的环节</h3>
    <ul>
      <li>文案初稿、绘图生成、资料检索、基础审核等重复性认知任务。</li>
      <li>AI 正在缩短这些环节所需时间，并重组知识劳动流程。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">仍然依赖人的环节</h3>
    <ul>
      <li>责任判断、纠错、协同、价值判断与最终决策。</li>
      <li>人类活劳动并未趋近于零，而是在重新定位。</li>
    </ul>
  </div>
</div>

<div class="accent-quote" v-click>
  AI 生产过程具有鲜明的社会化特征，<span class="highlight">收益归属与分配问题</span>因而愈加尖锐。马克思关于"自由时间"的论述，为理解这一变化提供了重要理论方向。
</div>

---
transition: slide-up
---

# 面向二：<span class="blue">资本的现代性枷锁</span>

<div class="box mt-4" v-click>
  <p>
    马克思指出，生产关系对生产力具有强大的反作用。在特定条件下，它也可能像桎梏一样束缚先进生产力的发展。
  </p>
</div>

<div class="accent-quote mt-4" v-click>
  在现行资本主义生产关系，即私有制逻辑主导下，
  <span class="highlight">AI 可能被导向垄断化、集中化的发展路径。</span>
</div>

<div class="layout-grid grid-2 mt-4">
  <div v-click>
    <div class="img-placeholder medium">
      <img src="\assets\CIS_shares.jpg">
    </div>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">资本逻辑的现代性制约</h3>
    <ul>
      <li>资源向头部集中，算力、模型、数据与入口形成新壁垒。</li>
      <li>技术被优先纳入降本增效、利润最大化的应用逻辑。</li>
      <li>部分岗位和入门机会随之收缩，差距可能持续扩大。</li>
    </ul>
  </div>
</div>

---
transition: slide-up
---

# 资本有机构成（C:V）与结构性失衡
<br>
<div class="layout-grid grid-2">
  <div class="box" v-click>
    <h3 class="text-center">公式回顾</h3>
    <ul>
      <li><strong>C：</strong> 不变资本，传统上是机器、厂房、设备；在 AI 时代更集中体现为算力与训练投入。</li>
      <li><strong>V：</strong> 可变资本，即购买劳动力所支付的工资。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">AI 时代的深刻变化</h3>
    <ul>
      <li>训练算力和资本密集度显著上升，头部企业优势更容易被放大。</li>
      <li>部分企业强化降本增效逻辑，提高了技术性失业和岗位收缩风险。</li>
      <li>若收入分配与就业吸纳机制滞后，结构性失衡将进一步加剧。</li>
    </ul>
  </div>
</div>

<div class="accent-quote" v-click>
  问题不在于商品必然过剩，而在于生产能力增长与社会分配机制之间，
  可能出现新的失衡与有效需求不足风险。
</div>

---
transition: fade
---

# 数据资产化与收益分配不对称

<br>
<div class="layout-grid grid-2 items-center">
  <div v-click>
    <ul>
      <li><strong>用户持续贡献数据：</strong> 发帖、点赞、浏览、评论、交互等行为均沉淀为平台的重要数据资源。</li>
      <li><strong>平台将其转化为资产：</strong> 数据被用于积累模型能力、优化推荐系统和提升商业价值。</li>
      <li><strong>普通用户难以分享收益：</strong> 上述贡献通常不形成对应的工资性收益。</li>
    </ul>
    <div class="accent-quote mt-4">
      数据收益分配与平台权力约束，已成为数字经济时代的重要议题。
    </div>
  </div>

  <div class="box text-center" v-click>
    <div class="mb-3"><strong>用户行为、内容与交互</strong></div>
    <div class="text-2xl text-gray-400 mb-3">↓</div>
    <div class="mb-3"><strong>平台沉淀为数据资产</strong></div>
    <div class="text-2xl text-gray-400 mb-3">↓</div>
    <div class="mb-3"><strong>转化为模型能力与商业价值</strong></div>
    <div class="text-2xl text-gray-400 mb-3">↓</div>
    <div><strong class="highlight">收益分配并未同步回到数据贡献者</strong></div>
  </div>
</div>

---
transition: slide-left
---

# 四. 出路何在——法律与政策层面的制度干预

<div class="accent-quote mt-4" v-click>
  马克思主义基本原理指出，上层建筑并非被动反映经济基础，而是具有能动的反作用——这为调整技术发展方向提供了制度空间。
</div>

<div class="layout-grid grid-2 mt-5">
  <div class="box" v-click>
    <h3>欧盟《人工智能法案》</h3>
    <ul>
      <li>全球首个综合性 AI 法律框架，核心思路是风险分级监管。</li>
      <li>将部分 social scoring 等实践列为不可接受风险，并要求强化透明度与版权合规。</li>
      <li><strong>马原视角：</strong> 政治上层建筑通过法律强制力，限制资本借 AI 进行无序扩张和过度监控。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3>中国《生成式人工智能服务管理暂行办法》</h3>
    <ul>
      <li>强调价值导向、防止歧视性内容生成，并建立备案、登记与内容安全治理机制。</li>
      <li>结合后续标识制度等配套规则，体现国家对 AI 发展方向的主动引导。</li>
      <li><strong>马原视角：</strong> 上层建筑对经济基础发展方向进行定向调控的典型表现。</li>
    </ul>
  </div>
</div>

---
transition: slide-right
---

# 意识形态层面：观念上层建筑的思想博弈

<div class="box mt-6" v-click>
  <p>
    当前全球科技界的重要争论之一，是 AI 的产权与开放方式安排。
    现实并非"开源还是闭源"的二元选择，而是一个连续谱。
  </p>
</div>

<div class="layout-grid grid-2 mt-8">
  <div class="box" v-click>
    <h3 class="text-center">闭源派 / 受控开放</h3>
    <ul>
      <li>强调核心竞争力、商业回报和安全可控。</li>
      <li>背后对应私有财产神圣不可侵犯、市场主导的价值逻辑。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">开源派 / 知识共享</h3>
    <ul>
      <li>强调降低技术门槛，使更多主体能够在前人成果之上持续创新。</li>
      <li>开源不等于公有制，但在公共性与社会化生产方面具有一定呼应意义。</li>
    </ul>
  </div>
</div>

<div class="accent-quote" v-click>
  这场争论的实质，不只是技术路线之争，
  而是数字时代围绕 AI 产权与技术目的的意识形态博弈。
</div>

---
transition: slide-up
---

# 社会治理层面：对新型生产关系的探索

<br>
<div class="layout-grid grid-2">
  <div class="box" v-click>
    <h3 class="text-center">制度探索的现实背景</h3>
    <ul>
      <li>当雇佣劳动制等旧有生产关系在 AI 冲击下受到深刻挑战时，社会必须寻找新的制度安排。</li>
      <li>核心在于使 AI 创造的社会财富不只表现为资本收益的增长。</li>
    </ul>
  </div>

  <div class="box" v-click>
    <h3 class="text-center">全民基本收入（UBI）讨论</h3>
    <ul>
      <li>UBI 设想提出：国家是否应向全体公民提供无条件的基本生活保障金？</li>
      <li>它并非唯一方案，但表明社会正在探索雇佣劳动关系之外的新型分配机制。</li>
      <li>其意义在于体现上层建筑面对生产力巨变时的能动调整。</li>
    </ul>
  </div>
</div>

<div class="accent-quote" v-click>
  法律划定发展边界，意识形态争夺解释权，社会政策探索新方案——
  这是马克思主义关于经济基础与上层建筑相互作用原理的现实案例。
</div>

---
transition: fade
---

# 结语：回到马克思的智慧

<div class="layout-grid grid-2 items-center dense">
  <div v-click>
    <div class="img-placeholder large">
      <img src="\assets\hennie-stander-StV6G2GURA8-unsplash.jpg">
    </div>
  </div>

  <div v-click>
    <div class="box mb-3">
      <p>分析路径：<strong>生产力飞跃 → 生产关系桎梏 → 上层建筑反作用</strong></p>
    </div>
    <ul>
      <li>决定性因素并非技术参数本身，也不在于代码规模。</li>
      <li>AI 是通往共享的阶梯，还是加固资本权力的围栏，关键在于——谁控制它、如何分配收益、通过何种制度加以约束。</li>
      <li>只有通过生产关系变革与上层建筑的积极调节，先进生产力才可能真正成为全体社会成员通向"自由王国"的桥梁。</li>
    </ul>
    <div class="accent-quote">
      机器本身并非问题的根源，关键在于它被纳入何种社会关系和资本逻辑之中使用。
    </div>
  </div>
</div>

---
transition: fade
---

<div class="relative h-full w-full">
  <div class="absolute inset-0 flex items-center justify-center text-center">
    <h1 style="font-size: 3.8rem; max-width: none; margin: 0;">
      谢谢聆听
    </h1>
  </div>

  <div
    class="absolute text-right text-gray-500"
    style="right: 2.5rem; bottom: 2rem; font-size: 0.95rem; line-height: 1.8;"
  >
    <div style="font-weight: 600; color: #4b5563;">小组分工</div>
    <div>陈诺：汇报</div>
    <div>黄宇镐：汇报稿撰写</div>
    <div>李冀斌：资料搜集</div>
    <div>胡泽亮：幻灯片制作</div>
  </div>
</div>
