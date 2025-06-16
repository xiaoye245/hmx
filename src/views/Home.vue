<!-- 代码已包含 CSS：使用 TailwindCSS , 安装 TailwindCSS 后方可看到布局样式效果 -->
<template>
<div class="min-h-screen bg-gray-50">
<!-- 顶部导航 -->
<header class="bg-white/80 backdrop-blur-lg shadow-lg fixed w-full z-50 border-b border-amber-200/50">
<div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between flex-wrap">
<div class="flex items-center space-x-4">
<div class="relative">
<div class="absolute inset-0 rounded-full bg-gradient-to-tr from-amber-200 via-amber-100 to-white blur-lg opacity-60"></div>
<img src="https://ai-public.mastergo.com/ai/img_res/c38a0e64aea8dab6d4d5122267a69f97.jpg"
class="h-12 w-12 rounded-full relative z-10 shadow-md transform hover:scale-105 transition-transform duration-300" alt="Logo"/>
<div class="absolute -bottom-1 -right-1 w-4 h-4 bg-amber-500 rounded-full border-2 border-white shadow-sm"></div>
</div>
<div>
<h1 class="text-2xl font-bold bg-gradient-to-r from-amber-900 to-amber-700 bg-clip-text text-transparent drop-shadow">黄梅戏数据可视化平台</h1>
<p class="text-xs text-amber-600 mt-1">传承艺术瑰宝 · 弘扬戏曲文化</p>
</div>
</div>
<div class="flex items-center space-x-6">
<a-tabs v-model:activeKey="activeKey" class="overflow-x-auto transition-all duration-300 bg-white/60 rounded-full shadow px-2">
<a-tab-pane key="1" tab="观众年龄分布" />
<a-tab-pane key="2" tab="观众性别比例" />
<a-tab-pane key="3" tab="观众地域分布" />
<a-tab-pane key="4" tab="剧目主题变迁" />
<a-tab-pane key="5" tab="演员剧目关系" />
</a-tabs>
<div class="flex items-center space-x-4">
</div>
</div>
</div>
</header>
<!-- 主要内容区域 -->
<main class="pt-[88px] pb-12 w-full max-w-4xl mx-auto px-2 sm:px-4 md:px-6">
<!-- 装饰图片 -->
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6 mb-8">
<!-- 年龄分布相关图片 -->
<template v-if="activeKey === '1'">
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/4d48f5cc1d398e4c1a34c3f2dddeca06.jpg"
alt="观众年龄分布" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">全龄观众</h3>
<p class="text-sm text-gray-100 drop-shadow">跨越年龄的艺术魅力</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/76c1bf128dadc12e0c1f125802e755c9.jpg"
alt="年轻观众" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">青年传承</h3>
<p class="text-sm text-gray-100 drop-shadow">新生代的文化认同</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/f4b1db87a7e5d4f6daef1e008856097c.jpg"
alt="中年观众" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">中坚力量</h3>
<p class="text-sm text-gray-100 drop-shadow">戏曲文化的守护者</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/0d4b2712be1bcc7ecf0817207e89aa10.jpg"
alt="老年观众" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">戏曲挚爱</h3>
<p class="text-sm text-gray-100 drop-shadow">经典艺术的忠实拥趸</p>
</div>
</div>
</div>
</template>
<!-- 性别比例相关图片 -->
<template v-if="activeKey === '2'">
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/943805c8e99165ba07cbd666458b93a7.jpg"
alt="女性表演者" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">优雅风韵</h3>
<p class="text-sm text-gray-100 drop-shadow">女性艺术的独特魅力</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/f117850884918dcfb1562d3f00e74edd.jpg"
alt="男性表演者" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">阳刚之美</h3>
<p class="text-sm text-gray-100 drop-shadow">男性角色的独特诠释</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/23ab0a0254e2a651ac1656b8badd5121.jpg"
alt="观众群像" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">知音雅集</h3>
<p class="text-sm text-gray-100 drop-shadow">多元观众的共鸣</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/41b482671b3b7689e41a5230fc6905f7.jpg"
alt="群舞表演" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">群舞呈现</h3>
<p class="text-sm text-gray-100 drop-shadow">性别比例的舞台展现</p>
</div>
</div>
</div>
</template>
<!-- 地域分布相关图片 -->
<template v-if="activeKey === '3'">
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/63a3f9fbee565a0452f599cf05e1d80b.jpg"
alt="安徽地区" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">徽风皖韵</h3>
<p class="text-sm text-gray-100 drop-shadow">戏曲发源地的魅力</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/8397a07febb589a02ab0cf9bc9b2c784.jpg"
alt="上海地区" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">海派新韵</h3>
<p class="text-sm text-gray-100 drop-shadow">现代舞台的创新演绎</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/d94347ca36eefb9b786ad1fed1e64651.jpg"
alt="江西地区" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">赣鄱风情</h3>
<p class="text-sm text-gray-100 drop-shadow">地方特色的完美融合</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/eb75372e909c696770ca5c7d44a6c4e3.jpg"
alt="全国分布" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">全国传播</h3>
<p class="text-sm text-gray-100 drop-shadow">文化影响力的扩展</p>
</div>
</div>
</div>
</template>
<!-- 主题变迁相关图片 -->
<template v-if="activeKey === '4'">
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/dd7180b84139a4ec902abc8d31419259.jpg"
alt="传统题材" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">经典传承</h3>
<p class="text-sm text-gray-100 drop-shadow">传统剧目的永恒魅力</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/3feda3e51d7631739618adfd740fb50b.jpg"
alt="现代题材" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">创新突破</h3>
<p class="text-sm text-gray-100 drop-shadow">现代元素的融入</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/97ddecad6b9c4a624df0a90ed8e78b24.jpg"
alt="革命题材" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">革命精神</h3>
<p class="text-sm text-gray-100 drop-shadow">时代主题的艺术呈现</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/8bc10e9aa88edc350c5bb4f60506af6c.jpg"
alt="题材变迁" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">主题演变</h3>
<p class="text-sm text-gray-100 drop-shadow">艺术发展的历程</p>
</div>
</div>
</div>
</template>
<!-- 演员剧目关系相关图片 -->
<template v-if="activeKey === '5'">
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/ae48b33a8be24a23ac378eb51136b112.jpg"
alt="演员风采" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">名家风采</h3>
<p class="text-sm text-gray-100 drop-shadow">艺术大师的风采</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/8bd49aeacbbe40c42a14d5740c3f1718.jpg"
alt="排练现场" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">默契配合</h3>
<p class="text-sm text-gray-100 drop-shadow">演员间的精妙互动</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/75809841631966bc6ffe327201a21814.jpg"
alt="剧目集锦" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">经典剧目</h3>
<p class="text-sm text-gray-100 drop-shadow">艺术精髓的传承</p>
</div>
</div>
</div>
<div class="relative overflow-hidden rounded-3xl shadow-xl aspect-[4/3] group transition-all duration-300 hover:scale-105 hover:shadow-2xl hover:-translate-y-2 hover:ring-4 hover:ring-amber-200/60 hover:bg-amber-50/40 active:scale-95 bg-gradient-to-br from-amber-50 via-white to-amber-100">
<img src="https://ai-public.mastergo.com/ai/img_res/ecefb4b1aebbabf5d7b6398e1ddf1abd.jpg"
alt="演出剪影" class="w-full h-full object-cover transition-all duration-300 ease-in-out cursor-pointer hover:scale-105 hover:shadow-xl hover:brightness-110 group-hover:scale-105 group-hover:brightness-110 hover:rotate-1 animate-fadein"/>
<div class="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-end">
<div class="backdrop-blur-md bg-white/30 rounded-b-3xl p-4 w-full">
<h3 class="text-lg font-bold text-white drop-shadow">经典剪影</h3>
<p class="text-sm text-gray-100 drop-shadow">舞台精彩瞬间集锦</p>
</div>
</div>
</div>
</template>
</div>
<div class="bg-gradient-to-br from-amber-50 via-white to-amber-100 rounded-3xl shadow-lg p-8 border border-gray-100 relative overflow-hidden">
<img src="https://ai-public.mastergo.com/ai/img_res/24f70ee6c9ac5248ad4a0756ef33b8b7.jpg"
alt="卷轴背景" class="absolute inset-0 w-full h-full object-cover opacity-30"/>
<div class="absolute -left-1 sm:-left-3 top-1/2 transform -translate-y-1/2 hidden sm:block">
<img src="https://ai-public.mastergo.com/ai/img_res/ed4b1e201c24b5ae1760d205e84a79e6.jpg"
alt="装饰元素" class="h-[100px] sm:h-[200px] w-2 sm:w-6"/>
</div>
<div class="absolute -right-1 sm:-right-3 top-1/2 transform -translate-y-1/2 hidden sm:block">
<img src="https://ai-public.mastergo.com/ai/img_res/760ce83ffe5b9cf062864c40a02eee24.jpg"
alt="装饰元素" class="h-[100px] sm:h-[200px] w-2 sm:w-6"/>
</div>
<div class="relative z-10">
<!-- 年龄分布 -->
<div v-show="activeKey === '1'" class="w-full">
<h2 class="text-xl font-semibold mb-6 text-gray-800 border-l-4 border-amber-500 pl-4">观众年龄分布</h2>
<div ref="ageChart" class="w-full h-[400px] md:h-[500px] lg:h-[600px]"></div>
</div>
<!-- 性别比例 -->
<div v-show="activeKey === '2'" class="w-full">
<h2 class="text-lg font-medium mb-4">观众性别比例</h2>
<div ref="genderChart" class="w-full h-[400px] md:h-[500px] lg:h-[600px]"></div>
</div>
<!-- 地域分布 -->
<div v-show="activeKey === '3'" class="w-full">
<h2 class="text-lg font-medium mb-4">观众地域分布</h2>
<div ref="regionChart" class="w-full h-[400px] md:h-[500px] lg:h-[600px]"></div>
</div>
<!-- 主题变迁 -->
<div v-show="activeKey === '4'" class="w-full">
<h2 class="text-lg font-medium mb-4">剧目主题变迁</h2>
<div ref="themeChart" class="w-full h-[400px] md:h-[500px] lg:h-[600px]"></div>
</div>
<!-- 演员剧目关系 -->
<div v-show="activeKey === '5'" class="w-full">
<div class="flex items-center justify-between mb-4">
<h2 class="text-lg font-medium">演员剧目关系图</h2>
<div class="flex space-x-2">
<a-button class="!rounded-button" @click="showAllRelations">显示所有关系</a-button>
<a-select v-model:value="selectedActor" class="w-48 !rounded-button" placeholder="选择演员" @change="filterByActor">
<a-select-option v-for="actor in actors" :key="actor" :value="actor">{{ actor }}</a-select-option>
</a-select>
</div>
</div>
<div ref="relationChart" class="w-full h-[400px] md:h-[500px] lg:h-[600px]"></div>
</div>
</div>
</div>
</main>
</div>
</template>
<script lang="ts" setup>
import { ref, onMounted, nextTick, watch } from 'vue';
import * as echarts from 'echarts';
import { DatePicker, Button, Tabs, Select } from 'ant-design-vue';
import { SearchOutlined } from '@ant-design/icons-vue';
const activeKey = ref('1');
const ageChart = ref<HTMLElement | null>(null);
const genderChart = ref<HTMLElement | null>(null);
const regionChart = ref<HTMLElement | null>(null);
const themeChart = ref<HTMLElement | null>(null);
const relationChart = ref<HTMLElement | null>(null);
const selectedActor = ref<string>('');
const relationChartInstance = ref<echarts.ECharts | null>(null);
const actors = ['马兰', '韩再芬', '李明', '王小虎', '张月'];
const plays = ['天仙配', '女驸马', '牛郎织女', '梁山伯与祝英台', '孟丽君'];
const actorPlayRelations = [
{ source: '马兰', target: '天仙配' },
{ source: '马兰', target: '牛郎织女' },
{ source: '韩再芬', target: '女驸马' },
{ source: '韩再芬', target: '孟丽君' },
{ source: '李明', target: '天仙配' },
{ source: '李明', target: '梁山伯与祝英台' },
{ source: '王小虎', target: '牛郎织女' },
{ source: '王小虎', target: '孟丽君' },
{ source: '张月', target: '梁山伯与祝英台' },
{ source: '张月', target: '女驸马' }
];
const filterByActor = (actor: string) => {
if (!relationChartInstance.value) return;
const filteredRelations = actor ? actorPlayRelations.filter(relation => relation.source === actor) : actorPlayRelations;
const nodes: any[] = [];
const links: any[] = [];
filteredRelations.forEach(relation => {
if (!nodes.find(node => node.name === relation.source)) {
nodes.push({
name: relation.source,
category: 0,
symbolSize: 50,
itemStyle: { color: '#ff7875' }
});
}
if (!nodes.find(node => node.name === relation.target)) {
nodes.push({
name: relation.target,
category: 1,
symbolSize: 40,
itemStyle: { color: '#ffd666' }
});
}
links.push({
source: relation.source,
target: relation.target
});
});
relationChartInstance.value.setOption({
series: [{
data: nodes,
edges: links
}]
});
};
const showAllRelations = () => {
selectedActor.value = '';
filterByActor('');
};
const chartInited = ref({
  age: false,
  gender: false,
  region: false,
  theme: false,
  relation: false
});
let ageChartInstance: echarts.ECharts | null = null;
let genderChartInstance: echarts.ECharts | null = null;
let regionChartInstance: echarts.ECharts | null = null;
let themeChartInstance: echarts.ECharts | null = null;

onMounted(async () => {
  await nextTick();
  // 只初始化第一个tab
  if (activeKey.value === '1' && ageChart.value) {
    ageChartInstance = echarts.init(ageChart.value!);
    ageChartInstance.setOption({
      animation: false,
      tooltip: {
        trigger: 'axis',
        axisPointer: {
          type: 'shadow'
        }
      },
      legend: {
        data: ['18-25岁', '26-35岁', '36-45岁', '46-55岁', '56岁以上']
      },
      grid: {
        left: '10%',
        right: '10%',
        bottom: '3%',
        containLabel: true
      },
      xAxis: {
        type: 'category',
        data: ['2018', '2019', '2020', '2021', '2022']
      },
      yAxis: {
        type: 'value'
      },
      series: [
        { name: '18-25岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [320, 332, 301, 334, 390] },
        { name: '26-35岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [220, 182, 191, 234, 290] },
        { name: '36-45岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [150, 232, 201, 154, 190] },
        { name: '46-55岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [98, 77, 101, 99, 40] },
        { name: '56岁以上', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [43, 77, 101, 75, 40] }
      ]
    });
    chartInited.value.age = true;
  }
  window.addEventListener('resize', () => {
    if (ageChartInstance) ageChartInstance.resize();
    if (genderChartInstance) genderChartInstance.resize();
    if (regionChartInstance) regionChartInstance.resize();
    if (themeChartInstance) themeChartInstance.resize();
    if (relationChartInstance.value) relationChartInstance.value.resize();
  });
});

watch(activeKey, async (newKey) => {
  await nextTick();
  setTimeout(() => {
    if (newKey === '1') {
      if (!chartInited.value.age && ageChart.value) {
        ageChartInstance = echarts.init(ageChart.value!);
        ageChartInstance.setOption({
          animation: false,
          tooltip: {
            trigger: 'axis',
            axisPointer: { type: 'shadow' }
          },
          legend: { data: ['18-25岁', '26-35岁', '36-45岁', '46-55岁', '56岁以上'] },
          grid: { left: '10%', right: '10%', bottom: '3%', containLabel: true },
          xAxis: { type: 'category', data: ['2018', '2019', '2020', '2021', '2022'] },
          yAxis: { type: 'value' },
          series: [
            { name: '18-25岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [320, 332, 301, 334, 390] },
            { name: '26-35岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [220, 182, 191, 234, 290] },
            { name: '36-45岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [150, 232, 201, 154, 190] },
            { name: '46-55岁', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [98, 77, 101, 99, 40] },
            { name: '56岁以上', type: 'bar', stack: 'total', emphasis: { focus: 'series' }, data: [43, 77, 101, 75, 40] }
          ]
        });
        chartInited.value.age = true;
      } else if (ageChartInstance) {
        ageChartInstance.resize();
      }
    }
    if (newKey === '2') {
      if (!chartInited.value.gender && genderChart.value) {
        genderChartInstance = echarts.init(genderChart.value!);
        genderChartInstance.setOption({
          animation: false,
          tooltip: { trigger: 'item' },
          legend: { top: '5%', left: 'center' },
          series: [
            {
              name: '性别比例', type: 'pie', radius: ['40%', '70%'], avoidLabelOverlap: false,
              itemStyle: { borderRadius: 10, borderColor: '#fff', borderWidth: 2 },
              label: { show: false, position: 'center' },
              emphasis: { label: { show: true, fontSize: '40', fontWeight: 'bold' } },
              labelLine: { show: false },
              data: [ { value: 1048, name: '女性' }, { value: 735, name: '男性' } ]
            }
          ]
        });
        chartInited.value.gender = true;
      } else if (genderChartInstance) {
        genderChartInstance.resize();
      }
    }
    if (newKey === '3') {
      if (!chartInited.value.region && regionChart.value) {
        regionChartInstance = echarts.init(regionChart.value!);
        regionChartInstance.setOption({
          animation: false,
          tooltip: { trigger: 'axis', axisPointer: { type: 'shadow' } },
          grid: { left: '10%', right: '10%', bottom: '3%', containLabel: true },
          xAxis: { type: 'value', boundaryGap: [0, 0.01] },
          yAxis: { type: 'category', data: ['安徽', '江西', '湖北', '浙江', '上海', '其他'] },
          series: [ { type: 'bar', data: [18203, 12489, 9034, 5970, 3970, 2610] } ]
        });
        chartInited.value.region = true;
      } else if (regionChartInstance) {
        regionChartInstance.resize();
      }
    }
    if (newKey === '4') {
      if (!chartInited.value.theme && themeChart.value) {
        themeChartInstance = echarts.init(themeChart.value!);
        themeChartInstance.setOption({
          animation: false,
          tooltip: {
            trigger: 'axis',
            axisPointer: {
              type: 'cross',
              label: { backgroundColor: '#6a7985' }
            }
          },
          legend: { data: ['传统题材', '现代题材', '革命题材', '爱情题材'] },
          grid: { left: '10%', right: '10%', bottom: '3%', containLabel: true },
          xAxis: { type: 'category', boundaryGap: false, data: ['2018', '2019', '2020', '2021', '2022'] },
          yAxis: { type: 'value' },
          series: [
            { name: '传统题材', type: 'line', stack: 'Total', areaStyle: {}, emphasis: { focus: 'series' }, data: [120, 132, 101, 134, 90] },
            { name: '现代题材', type: 'line', stack: 'Total', areaStyle: {}, emphasis: { focus: 'series' }, data: [220, 182, 191, 234, 290] },
            { name: '革命题材', type: 'line', stack: 'Total', areaStyle: {}, emphasis: { focus: 'series' }, data: [150, 232, 201, 154, 190] },
            { name: '爱情题材', type: 'line', stack: 'Total', areaStyle: {}, emphasis: { focus: 'series' }, data: [320, 332, 301, 334, 390] }
          ]
        });
        chartInited.value.theme = true;
      } else if (themeChartInstance) {
        themeChartInstance.resize();
      }
    }
    if (newKey === '5') {
      if (!chartInited.value.relation && relationChart.value) {
        relationChartInstance.value = echarts.init(relationChart.value!);
        relationChartInstance.value.setOption({
          animation: false,
          tooltip: {},
          legend: { data: ['演员', '剧目'] },
          series: [{
            type: 'graph', layout: 'force', animation: false,
            label: { show: true, position: 'right', formatter: '{b}' },
            draggable: true,
            categories: [ { name: '演员' }, { name: '剧目' } ],
            force: { repulsion: 200, gravity: 0.1, edgeLength: [100, 200] },
            lineStyle: { color: '#bfbfbf', width: 2, curveness: 0.3 },
            emphasis: { focus: 'adjacency', lineStyle: { width: 4 } }
          }]
        });
        filterByActor('');
        chartInited.value.relation = true;
      } else if (relationChartInstance.value) {
        relationChartInstance.value.resize();
      }
    }
  }, 0);
});
</script>
<style scoped>
.bg-white {
background-image: linear-gradient(to right, rgba(255,255,255,0.95), rgba(255,255,255,0.95));
}
:deep(.ant-tabs-tab) {
@apply text-gray-600 text-sm transition-colors duration-300;
}
:deep(.ant-tabs-tab:hover) {
@apply text-amber-600;
}
:deep(.ant-tabs-tab.ant-tabs-tab-active .ant-tabs-tab-btn) {
@apply text-amber-600 font-medium;
}
:deep(.ant-tabs-ink-bar) {
@apply bg-amber-600;
}
:deep(.ant-picker-input > input) {
@apply text-sm;
}
:deep(.ant-select-selector) {
@apply shadow-sm hover:shadow-md transition-shadow duration-300;
}
:deep(.ant-btn:not(.ant-btn-primary)) {
@apply border-gray-300 hover:border-amber-500 hover:text-amber-500 transition-colors duration-300;
}
</style> 