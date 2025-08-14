<script setup lang="ts">
defineOptions({
  name: "Welcome"
});

// 复选框选项数据
const checkboxOptions = [
  { label: "选项一", checked: true },
  { label: "选项二", checked: false },
  { label: "选项三", checked: true },
  { label: "选项四", checked: false },
  { label: "选项五", checked: false },
  { label: "选项六", checked: false },
  { label: "选项七", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false },
  { label: "选项八", checked: false }
];
// 内容卡片数据
const contentCards = [
  {
    title: "内容卡片 1",
    content: [
      "这是第一个内容卡片，包含了一些示例文本。此区域可以滚动，而标题栏和左侧复选框列表保持固定不动。",
      "通过纯CSS实现了这种布局效果，不依赖任何第三方样式库。使用了flex布局和overflow属性来控制滚动行为。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  },
  {
    title: "内容卡片 2",
    content: [
      "这是第二个内容卡片，展示了更多的文本内容。当内容超出可视区域时，右侧区域会出现滚动条，方便用户浏览所有内容。",
      "固定元素（标题栏和侧边栏）使用了CSS的overflow: hidden属性，而内容区域则设置了overflow-y: auto，使其可以垂直滚动。"
    ]
  }
  // 可以添加更多内容卡片...
];

// 处理复选框变化事件
const handleCheckboxChange = item => {
  console.log("复选框变化:", item.label, "状态:", item.checked);
  // 这里可以添加筛选逻辑
};
</script>

<template>
  <!-- 页面容器（使用 pure-vue-admin 布局容器） -->
  <div class="fixed-layout-page">
    <!-- 主要内容区域 -->
    <div class="main-container">
      <!-- 左侧复选框列表 -->
      <aside class="checkbox-sidebar">
        <h2 class="sidebar-title">选项筛选</h2>
        <div class="checkbox-group">
          <div
            v-for="(item, index) in checkboxOptions"
            :key="index"
            class="checkbox-item"
          >
            <input
              :id="'option' + index"
              v-model="item.checked"
              type="checkbox"
              @change="handleCheckboxChange(item)"
            />
            <label :for="'option' + index">{{ item.label }}</label>
          </div>
        </div>
      </aside>

      <!-- 右侧内容显示区 -->
      <main class="content-area">
        <h2 class="content-title">主要内容展示</h2>

        <!-- 动态生成内容卡片 -->
        <div
          v-for="(card, index) in contentCards"
          :key="index"
          class="content-card"
        >
          <h3>{{ card.title }}</h3>
          <p v-for="(paragraph, pIndex) in card.content" :key="pIndex">
            {{ paragraph }}
          </p>
        </div>
      </main>
    </div>
  </div>
</template>

<style scoped>
/* 基础样式 */
.fixed-layout-page {
  height: 100vh;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

/* 标题栏样式 */
.custom-header {
  background-color: #2c3e50;
  color: white;
  padding: 1rem 2rem;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  z-index: 10;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1600px;
  margin: 0 auto;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

/* 主要内容区域容器 */
.main-container {
  display: flex;
  flex: 1;
  overflow: hidden;
}

/* 左侧复选框列表 */
.checkbox-sidebar {
  width: 250px;
  background-color: #f8f9fa;
  border-right: 1px solid #dee2e6;
  padding: 1.5rem;
  overflow-y: auto;
}

.sidebar-title {
  font-size: 1.2rem;
  margin-bottom: 1rem;
  color: #343a40;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid #dee2e6;
}

.checkbox-group {
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

.checkbox-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  cursor: pointer;
  padding: 0.4rem;
  border-radius: 4px;
  transition: background-color 0.2s;
}

.checkbox-item:hover {
  background-color: #e9ecef;
}

.checkbox-item input {
  width: 16px;
  height: 16px;
}

.checkbox-item label {
  flex: 1;
  cursor: pointer;
  color: #495057;
}

/* 右侧内容显示区 */
.content-area {
  flex: 1;
  padding: 2rem;
  overflow-y: auto;
  background-color: #ffffff;
}

.content-title {
  font-size: 1.4rem;
  margin-bottom: 1.5rem;
  color: #212529;
}

.content-card {
  background-color: #f8f9fa;
  border-radius: 6px;
  padding: 1.5rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

.content-card h3 {
  margin-bottom: 1rem;
  color: #343a40;
}

.content-card p {
  color: #6c757d;
  line-height: 1.6;
  margin-bottom: 1rem;
}

/* 自定义滚动条 */
.content-area::-webkit-scrollbar {
  width: 8px;
}

.content-area::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 4px;
}

.content-area::-webkit-scrollbar-thumb {
  background: #bbb;
  border-radius: 4px;
}

.content-area::-webkit-scrollbar-thumb:hover {
  background: #999;
}

/* 响应式调整 */
@media (max-width: 768px) {
  .main-container {
    flex-direction: column;
  }

  .checkbox-sidebar {
    width: 100%;
    border-right: none;
    border-bottom: 1px solid #dee2e6;
    max-height: 200px;
    overflow-y: auto;
  }
}
</style>
