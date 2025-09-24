<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>东莞市锦鹰自动化设备有限公司 - 压铸自动化解决方案专家</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.8/dist/chart.umd.min.js"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  
  <!-- Tailwind 配置 -->
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#0F3460',      // 深蓝主色
            secondary: '#1A73E8',    // 亮蓝辅助色
            accent: '#E6B325',       // 金色强调色
            dark: '#2C3E50',         // 深色
            light: '#F5F7FA',        // 浅色背景
            neutral: '#95A5A6'       // 中性色
          },
          fontFamily: {
            inter: ['Inter', 'sans-serif'],
          },
        },
      }
    }
  </script>
  
  <style type="text/tailwindcss">
    @layer utilities {
      .content-auto {
        content-visibility: auto;
      }
      .text-shadow {
        text-shadow: 0 2px 4px rgba(0,0,0,0.1);
      }
      .text-shadow-lg {
        text-shadow: 0 4px 8px rgba(0,0,0,0.2);
      }
      .transition-transform {
        transition-property: transform;
        transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
        transition-duration: 300ms;
      }
      .hover-lift {
        @apply hover:-translate-y-1 transition-all duration-300;
      }
      .section-padding {
        @apply py-16 md:py-24;
      }
    }
  </style>
</head>

<body class="font-inter text-dark bg-white">
  <!-- 导航栏 -->
  <header id="navbar" class="fixed w-full top-0 z-50 transition-all duration-300 bg-transparent">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4">
        <!-- 公司Logo -->
        <a href="#" class="flex items-center space-x-2">
          <div class="w-10 h-10 bg-primary rounded-md flex items-center justify-center">
            <span class="text-white font-bold text-xl">锦鹰</span>
          </div>
          <span class="text-primary font-bold text-lg md:text-xl hidden sm:block">锦鹰自动化</span>
        </a>
        
        <!-- 桌面导航 -->
        <nav class="hidden md:flex space-x-8">
          <a href="#home" class="text-white hover:text-accent transition-colors">首页</a>
          <a href="#about" class="text-white hover:text-accent transition-colors">关于我们</a>
          <a href="#products" class="text-white hover:text-accent transition-colors">产品中心</a>
          <a href="#cases" class="text-white hover:text-accent transition-colors">应用案例</a>
          <a href="#contact" class="text-white hover:text-accent transition-colors">联系我们</a>
        </nav>
        
        <!-- 联系电话 -->
        <div class="hidden md:flex items-center space-x-1 text-white">
          <i class="fa fa-phone"></i>
          <span>13829267422</span>
        </div>
        
        <!-- 移动端菜单按钮 -->
        <button id="menuBtn" class="md:hidden text-white text-2xl">
          <i class="fa fa-bars"></i>
        </button>
      </div>
    </div>
    
    <!-- 移动端导航菜单 -->
    <div id="mobileMenu" class="md:hidden bg-white shadow-lg absolute w-full left-0 top-full transform -translate-y-full opacity-0 transition-all duration-300 pointer-events-none">
      <div class="container mx-auto px-4 py-4 flex flex-col space-y-4">
        <a href="#home" class="text-primary hover:text-accent py-2 border-b border-gray-100">首页</a>
        <a href="#about" class="text-primary hover:text-accent py-2 border-b border-gray-100">关于我们</a>
        <a href="#products" class="text-primary hover:text-accent py-2 border-b border-gray-100">产品中心</a>
        <a href="#cases" class="text-primary hover:text-accent py-2 border-b border-gray-100">应用案例</a>
        <a href="#contact" class="text-primary hover:text-accent py-2">联系我们</a>
        <div class="flex items-center space-x-2 text-primary pt-2">
          <i class="fa fa-phone"></i>
          <span>13829267422</span>
        </div>
      </div>
    </div>
  </header>

  <!-- 英雄区域 -->
  <section id="home" class="relative h-screen flex items-center justify-center overflow-hidden">
    <!-- 背景图：在此处添加公司主视觉图片 -->
    <div class="absolute inset-0 z-0">
      <img src="hero-bg.jpg" alt="压铸自动化生产线" class="w-full h-full object-cover">
      <div class="absolute inset-0 bg-primary/60"></div>
    </div>
    
    <div class="container mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
      <h1 class="text-[clamp(2rem,5vw,4rem)] font-bold text-white leading-tight text-shadow-lg mb-6">
        东莞市锦鹰自动化设备有限公司
      </h1>
      <p class="text-[clamp(1rem,2vw,1.25rem)] text-white/90 max-w-3xl mx-auto mb-10 text-shadow">
        专注于压铸行业自动化解决方案，提供高品质自动化机器设备，
        助力企业提升生产效率与产品质量
      </p>
      <div class="flex flex-col sm:flex-row justify-center gap-4">
        <a href="#products" class="bg-accent hover:bg-accent/90 text-white font-medium py-3 px-8 rounded-md transition-all hover-lift">
          查看产品
        </a>
        <a href="#contact" class="bg-transparent border-2 border-white hover:border-accent text-white hover:text-accent font-medium py-3 px-8 rounded-md transition-all hover-lift">
          联系我们
        </a>
      </div>
    </div>
    
    <!-- 向下滚动指示 -->
    <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 text-white animate-bounce">
      <i class="fa fa-angle-down text-3xl"></i>
    </div>
  </section>

  <!-- 关于我们 -->
  <section id="about" class="section-padding bg-light">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold text-primary mb-4">关于锦鹰自动化</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-neutral max-w-3xl mx-auto">专注压铸自动化领域多年，致力于为客户提供高效、稳定、智能的自动化解决方案</p>
      </div>
      
      <div class="grid md:grid-cols-2 gap-12 items-center">
        <!-- 公司图片：在此处添加公司厂房或团队图片 -->
        <div class="relative group">
          <img src="company-factory.jpg" alt="锦鹰自动化厂房" class="w-full h-auto rounded-lg shadow-xl">
          <div class="absolute inset-0 bg-primary/30 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex items-center justify-center">
            <span class="text-white text-xl font-medium">现代化生产基地</span>
          </div>
        </div>
        
        <div>
          <h3 class="text-2xl font-semibold text-primary mb-4">公司简介</h3>
          <p class="text-gray-700 mb-4">
            东莞市锦鹰自动化设备有限公司成立于2010年，是一家专业从事压铸行业自动化设备研发、生产、销售及服务的高新技术企业。
          </p>
          <p class="text-gray-700 mb-6">
            公司拥有一支由机械设计、电气控制、软件开发等专业人才组成的技术团队，凭借多年行业经验和技术积累，为客户提供量身定制的自动化解决方案，帮助客户实现生产自动化、智能化升级，降低生产成本，提高生产效率和产品质量。
          </p>
          
          <div class="grid sm:grid-cols-2 gap-6 mb-8">
            <div class="flex items-start space-x-3">
              <div class="bg-primary/10 p-3 rounded-full text-primary">
                <i class="fa fa-lightbulb-o text-xl"></i>
              </div>
              <div>
                <h4 class="font-semibold text-primary mb-1">技术创新</h4>
                <p class="text-gray-600 text-sm">持续研发投入，保持技术领先</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="bg-primary/10 p-3 rounded-full text-primary">
                <i class="fa fa-certificate text-xl"></i>
              </div>
              <div>
                <h4 class="font-semibold text-primary mb-1">品质保证</h4>
                <p class="text-gray-600 text-sm">严格质量控制，确保设备稳定</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="bg-primary/10 p-3 rounded-full text-primary">
                <i class="fa fa-users text-xl"></i>
              </div>
              <div>
                <h4 class="font-semibold text-primary mb-1">专业团队</h4>
                <p class="text-gray-600 text-sm">资深工程师，丰富行业经验</p>
              </div>
            </div>
            <div class="flex items-start space-x-3">
              <div class="bg-primary/10 p-3 rounded-full text-primary">
                <i class="fa fa-headphones text-xl"></i>
              </div>
              <div>
                <h4 class="font-semibold text-primary mb-1">完善服务</h4>
                <p class="text-gray-600 text-sm">售前咨询，售后技术支持</p>
              </div>
            </div>
          </div>
          
          <a href="#contact" class="inline-flex items-center text-primary font-medium hover:text-accent transition-colors">
            了解更多 <i class="fa fa-long-arrow-right ml-2"></i>
          </a>
        </div>
      </div>
      
      <!-- 公司数据 -->
      <div class="grid grid-cols-2 md:grid-cols-4 gap-6 mt-20">
        <div class="bg-white p-6 rounded-lg shadow-md text-center hover-lift">
          <div class="text-4xl font-bold text-primary mb-2">10+</div>
          <div class="text-gray-600">行业经验</div>
        </div>
        <div class="bg-white p-6 rounded-lg shadow-md text-center hover-lift">
          <div class="text-4xl font-bold text-primary mb-2">50+</div>
          <div class="text-gray-600">专业技术人员</div>
        </div>
        <div class="bg-white p-6 rounded-lg shadow-md text-center hover-lift">
          <div class="text-4xl font-bold text-primary mb-2">300+</div>
          <div class="text-gray-600">成功案例</div>
        </div>
        <div class="bg-white p-6 rounded-lg shadow-md text-center hover-lift">
          <div class="text-4xl font-bold text-primary mb-2">98%</div>
          <div class="text-gray-600">客户满意度</div>
        </div>
      </div>
    </div>
  </section>

  <!-- 产品中心 -->
  <section id="products" class="section-padding">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold text-primary mb-4">自动化机器设备</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-neutral max-w-3xl mx-auto">我们提供全系列压铸自动化设备，满足不同生产需求，提升生产效率</p>
      </div>
      
      <!-- 产品分类 -->
      <div class="flex flex-wrap justify-center gap-4 mb-12">
        <button class="product-filter active bg-primary text-white px-6 py-2 rounded-full text-sm font-medium">全部产品</button>
        <button class="product-filter bg-gray-100 hover:bg-primary/10 px-6 py-2 rounded-full text-sm font-medium transition-colors">压铸机器人</button>
        <button class="product-filter bg-gray-100 hover:bg-primary/10 px-6 py-2 rounded-full text-sm font-medium transition-colors">自动化生产线</button>
        <button class="product-filter bg-gray-100 hover:bg-primary/10 px-6 py-2 rounded-full text-sm font-medium transition-colors">检测设备</button>
        <button class="product-filter bg-gray-100 hover:bg-primary/10 px-6 py-2 rounded-full text-sm font-medium transition-colors">辅助设备</button>
      </div>
      
      <!-- 产品列表 -->
      <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- 产品1：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
        <div class="relative h-60 overflow-hidden">
            <!-- 核心修改：移除固定尺寸，添加自适应规则 -->
            <img src="19955cba72a6c969e30f6b5b2ce695f4.jpg" 
                alt="JY-650配比机" 
                class="w-full h-full object-cover"> <!-- 自适应容器关键样式 -->
            <div class="absolute top-4 right-4 bg-accent text-white text-xs font-bold px-3 py-1 rounded-full">
            热销产品
            </div>
        </div>
        <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-650 配比机</h3>
            <p class="text-gray-600 mb-4 text-sm">高精度伺服控制，快速响应，适用于各类压铸产品的自动取件、喷雾等工序</p>
            <div class="flex justify-between items-center">
            <span class="text-primary font-bold">¥ 24000 起</span>
            <a href="jy-650-details.html?id=1" class="text-secondary hover:text-accent transition-colors" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
            </a>
            </div>
        </div>
        </div>
        <!-- 产品2：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
          <div class="relative h-60 overflow-hidden">
            <img src="product-2.jpg" alt="全自动压铸生产线" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-1200 全自动压铸生产线</h3>
            <p class="text-gray-600 mb-4 text-sm">集成送料、压铸、取件、冷却、检测等工序，实现全自动化生产</p>
            <div class="flex justify-between items-center">
              <span class="text-primary font-bold">¥ 180,000 起</span>
              <a href="#" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 产品3：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
          <div class="relative h-60 overflow-hidden">
            <img src="product-3.jpg" alt="铸件尺寸检测设备" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-800 铸件尺寸检测设备</h3>
            <p class="text-gray-600 mb-4 text-sm">采用机器视觉技术，自动检测铸件尺寸精度，提高质检效率和准确性</p>
            <div class="flex justify-between items-center">
              <span class="text-primary font-bold">¥ 56,000 起</span>
              <a href="#" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 产品4：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
          <div class="relative h-60 overflow-hidden">
            <img src="product-4.jpg" alt="自动喷雾润滑系统" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-300 自动喷雾润滑系统</h3>
            <p class="text-gray-600 mb-4 text-sm">精准控制喷雾量和范围，提高模具寿命，减少脱模剂消耗</p>
            <div class="flex justify-between items-center">
              <span class="text-primary font-bold">¥ 22,000 起</span>
              <a href="#" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 产品5：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
          <div class="relative h-60 overflow-hidden">
            <img src="product-5.jpg" alt="机器人上下料系统" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
            <div class="absolute top-4 right-4 bg-accent text-white text-xs font-bold px-3 py-1 rounded-full">
              新品
            </div>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-500 机器人上下料系统</h3>
            <p class="text-gray-600 mb-4 text-sm">柔性自动化上下料解决方案，可与多种设备对接，提高生产效率</p>
            <div class="flex justify-between items-center">
              <span class="text-primary font-bold">¥ 45,000 起</span>
              <a href="#" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
        
        <!-- 产品6：在此处添加产品图片 -->
        <div class="bg-white rounded-lg shadow-md overflow-hidden group hover-lift">
          <div class="relative h-60 overflow-hidden">
            <img src="product-6.jpg" alt="自动化控制系统" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-primary mb-2">JY-700 自动化控制系统</h3>
            <p class="text-gray-600 mb-4 text-sm">智能化中央控制系统，实现多设备协同工作，可远程监控和管理</p>
            <div class="flex justify-between items-center">
              <span class="text-primary font-bold">¥ 32,000 起</span>
              <a href="#" class="text-secondary hover:text-accent transition-colors">
                查看详情 <i class="fa fa-arrow-right ml-1"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
      
      <div class="text-center mt-12">
        <a href="#" class="inline-block bg-primary hover:bg-primary/90 text-white font-medium py-3 px-8 rounded-md transition-all hover-lift">
          查看全部产品 <i class="fa fa-arrow-right ml-2"></i>
        </a>
      </div>
    </div>
  </section>

  <!-- 技术优势 -->
  <section class="section-padding bg-primary text-white">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold mb-4">我们的技术优势</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-white/80 max-w-3xl mx-auto">依托强大的研发实力和技术积累，为客户提供领先的自动化解决方案</p>
      </div>
      
      <div class="grid md:grid-cols-3 gap-8">
        <div class="bg-white/10 backdrop-blur-sm p-8 rounded-lg hover-lift">
          <div class="w-16 h-16 bg-accent/20 rounded-full flex items-center justify-center mb-6">
            <i class="fa fa-cogs text-2xl text-accent"></i>
          </div>
          <h3 class="text-xl font-semibold mb-4">定制化解决方案</h3>
          <p class="text-white/70">根据客户生产需求和场地条件，量身定制自动化解决方案，确保设备与生产流程完美匹配</p>
        </div>
        
        <div class="bg-white/10 backdrop-blur-sm p-8 rounded-lg hover-lift">
          <div class="w-16 h-16 bg-accent/20 rounded-full flex items-center justify-center mb-6">
            <i class="fa fa-microchip text-2xl text-accent"></i>
          </div>
          <h3 class="text-xl font-semibold mb-4">智能化控制系统</h3>
          <p class="text-white/70">采用先进的PLC控制系统和人机界面，操作简单直观，可实现远程监控和数据分析</p>
        </div>
        
        <div class="bg-white/10 backdrop-blur-sm p-8 rounded-lg hover-lift">
          <div class="w-16 h-16 bg-accent/20 rounded-full flex items-center justify-center mb-6">
            <i class="fa fa-tachometer text-2xl text-accent"></i>
          </div>
          <h3 class="text-xl font-semibold mb-4">高效稳定运行</h3>
          <p class="text-white/70">设备运行稳定可靠，故障率低，生产效率高，大幅降低人工成本和产品不良率</p>
        </div>
      </div>
      
      <!-- 数据对比图表 -->
      <div class="mt-20 bg-white/5 backdrop-blur-sm p-6 rounded-lg">
        <h3 class="text-xl font-semibold mb-6 text-center">自动化前后生产效率对比</h3>
        <div class="h-80">
          <canvas id="efficiencyChart"></canvas>
        </div>
      </div>
    </div>
  </section>

  <!-- 应用案例 -->
  <section id="cases" class="section-padding bg-light">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold text-primary mb-4">成功应用案例</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-neutral max-w-3xl mx-auto">我们的设备已成功应用于多家知名企业，帮助客户实现自动化生产升级</p>
      </div>
      
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- 案例1：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-1.jpg" alt="汽车零部件压铸自动化生产线" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">汽车零部件压铸自动化生产线</h3>
            <p class="text-white/80 text-sm">某知名汽车零部件制造商</p>
          </div>
        </div>
        
        <!-- 案例2：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-2.jpg" alt="摩托车配件自动化生产系统" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">摩托车配件自动化生产系统</h3>
            <p class="text-white/80 text-sm">某大型摩托车企业</p>
          </div>
        </div>
        
        <!-- 案例3：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-3.jpg" alt="家电压铸件自动化生产线" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">家电压铸件自动化生产线</h3>
            <p class="text-white/80 text-sm">某知名家电企业</p>
          </div>
        </div>
        
        <!-- 案例4：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-4.jpg" alt="通讯设备零件自动化生产" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">通讯设备零件自动化生产</h3>
            <p class="text-white/80 text-sm">某通讯设备制造商</p>
          </div>
        </div>
        
        <!-- 案例5：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-5.jpg" alt="医疗器械零件自动化生产线" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">医疗器械零件自动化生产线</h3>
            <p class="text-white/80 text-sm">某医疗器械企业</p>
          </div>
        </div>
        
        <!-- 案例6：在此处添加案例图片 -->
        <div class="group relative overflow-hidden rounded-lg shadow-md hover-lift h-64">
          <img src="case-6.jpg" alt="LED灯具配件自动化生产" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-110">
          <div class="absolute inset-0 bg-gradient-to-t from-primary/80 to-transparent opacity-80"></div>
          <div class="absolute bottom-0 left-0 p-6">
            <h3 class="text-white font-semibold text-lg mb-1">LED灯具配件自动化生产</h3>
            <p class="text-white/80 text-sm">某照明企业</p>
          </div>
        </div>
      </div>
      
      <div class="text-center mt-12">
        <a href="#" class="inline-block bg-white border border-primary text-primary hover:bg-primary hover:text-white font-medium py-3 px-8 rounded-md transition-all hover-lift">
          查看更多案例 <i class="fa fa-arrow-right ml-2"></i>
        </a>
      </div>
    </div>
  </section>

  <!-- 客户评价 -->
  <section class="section-padding">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold text-primary mb-4">客户评价</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-neutral max-w-3xl mx-auto">听听我们的客户怎么说</p>
      </div>
      
      <div class="testimonial-slider relative">
        <div class="overflow-hidden">
          <div class="testimonial-track flex transition-transform duration-500">
            <!-- 评价1：在此处添加客户logo -->
            <div class="testimonial-item w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-4">
              <div class="bg-white p-8 rounded-lg shadow-md h-full">
                <div class="flex items-center mb-6">
                  <img src="client-1.jpg" alt="客户logo" class="w-16 h-16 object-contain mr-4">
                  <div>
                    <h4 class="font-semibold text-primary">广州某汽车零部件有限公司</h4>
                    <div class="flex text-accent mt-1">
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                    </div>
                  </div>
                </div>
                <p class="text-gray-600 italic">
                  "锦鹰自动化的压铸生产线帮助我们实现了生产自动化，不仅提高了生产效率30%以上，还大大降低了产品不良率，非常满意他们的设备和服务。"
                </p>
              </div>
            </div>
            
            <!-- 评价2：在此处添加客户logo -->
            <div class="testimonial-item w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-4">
              <div class="bg-white p-8 rounded-lg shadow-md h-full">
                <div class="flex items-center mb-6">
                  <img src="client-2.jpg" alt="客户logo" class="w-16 h-16 object-contain mr-4">
                  <div>
                    <h4 class="font-semibold text-primary">深圳某电子科技有限公司</h4>
                    <div class="flex text-accent mt-1">
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star-half-o"></i>
                    </div>
                  </div>
                </div>
                <p class="text-gray-600 italic">
                  "从设备安装调试到员工培训，锦鹰自动化的团队都表现出专业的素养。他们的自动化检测设备为我们节省了大量人力，检测精度也非常高。"
                </p>
              </div>
            </div>
            
            <!-- 评价3：在此处添加客户logo -->
            <div class="testimonial-item w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-4">
              <div class="bg-white p-8 rounded-lg shadow-md h-full">
                <div class="flex items-center mb-6">
                  <img src="client-3.jpg" alt="客户logo" class="w-16 h-16 object-contain mr-4">
                  <div>
                    <h4 class="font-semibold text-primary">佛山某家电制造有限公司</h4>
                    <div class="flex text-accent mt-1">
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                      <i class="fa fa-star"></i>
                    </div>
                  </div>
                </div>
                <p class="text-gray-600 italic">
                  "与锦鹰自动化合作多年，他们的设备稳定性好，售后服务响应及时，是我们值得信赖的合作伙伴。最近上线的全自动生产线更是让我们的产能提升了50%。"
                </p>
              </div>
            </div>
          </div>
        </div>
        
        <!-- 滑动控制按钮 -->
        <button class="testimonial-prev absolute top-1/2 left-0 transform -translate-y-1/2 bg-white w-10 h-10 rounded-full shadow-md flex items-center justify-center text-primary hover:text-accent transition-colors z-10 md:-left-5">
          <i class="fa fa-angle-left text-xl"></i>
        </button>
        <button class="testimonial-next absolute top-1/2 right-0 transform -translate-y-1/2 bg-white w-10 h-10 rounded-full shadow-md flex items-center justify-center text-primary hover:text-accent transition-colors z-10 md:-right-5">
          <i class="fa fa-angle-right text-xl"></i>
        </button>
        
        <!-- 指示器 -->
        <div class="flex justify-center mt-8 space-x-2">
          <button class="testimonial-dot w-3 h-3 rounded-full bg-primary"></button>
          <button class="testimonial-dot w-3 h-3 rounded-full bg-gray-300"></button>
          <button class="testimonial-dot w-3 h-3 rounded-full bg-gray-300"></button>
        </div>
      </div>
    </div>
  </section>

  <!-- 联系我们 -->
  <section id="contact" class="section-padding bg-light">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-bold text-primary mb-4">联系我们</h2>
        <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
        <p class="text-neutral max-w-3xl mx-auto">无论您有任何疑问或需求，都欢迎随时联系我们，我们将竭诚为您服务</p>
      </div>
      
      <div class="grid md:grid-cols-2 gap-12">
        <div>
          <form class="bg-white p-8 rounded-lg shadow-md">
            <h3 class="text-xl font-semibold text-primary mb-6">发送询价</h3>
            <div class="mb-4">
              <label for="name" class="block text-gray-700 mb-2 text-sm">姓名</label>
              <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary" placeholder="请输入您的姓名">
            </div>
            <div class="mb-4">
              <label for="phone" class="block text-gray-700 mb-2 text-sm">电话</label>
              <input type="tel" id="phone" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary" placeholder="请输入您的电话">
            </div>
            <div class="mb-4">
              <label for="company" class="block text-gray-700 mb-2 text-sm">公司名称</label>
              <input type="text" id="company" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary" placeholder="请输入您的公司名称">
            </div>
            <div class="mb-6">
              <label for="message" class="block text-gray-700 mb-2 text-sm">留言</label>
              <textarea id="message" rows="4" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-primary/50 focus:border-primary" placeholder="请输入您的需求或疑问"></textarea>
            </div>
            <button type="submit" class="w-full bg-primary hover:bg-primary/90 text-white font-medium py-3 px-6 rounded-md transition-all hover-lift">
              提交询价
            </button>
          </form>
        </div>
        
        <div>
          <div class="bg-white p-8 rounded-lg shadow-md h-full">
            <h3 class="text-xl font-semibold text-primary mb-6">联系方式</h3>
            
            <div class="space-y-6">
              <div class="flex items-start">
                <div class="bg-primary/10 p-3 rounded-full text-primary mr-4">
                  <i class="fa fa-map-marker"></i>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-1">公司地址</h4>
                  <p class="text-gray-600">广东省东莞市清溪镇三星村三星路2号</p>
                </div>
              </div>
              
              <div class="flex items-start">
                <div class="bg-primary/10 p-3 rounded-full text-primary mr-4">
                  <i class="fa fa-phone"></i>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-1">联系电话</h4>
                  <p class="text-gray-600">13829267422</p>
                </div>
              </div>
              
              <div class="flex items-start">
                <div class="bg-primary/10 p-3 rounded-full text-primary mr-4">
                  <i class="fa fa-envelope"></i>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-1">电子邮箱</h4>
                  <p class="text-gray-600">ozyrro@163.com</p>
                </div>
              </div>
              
              <div class="flex items-start">
                <div class="bg-primary/10 p-3 rounded-full text-primary mr-4">
                  <i class="fa fa-clock-o"></i>
                </div>
                <div>
                  <h4 class="font-semibold text-primary mb-1">工作时间</h4>
                  <p class="text-gray-600">周一至周五: 8:00 - 18:00</p>
                  <p class="text-gray-600">周六: 9:00 - 15:00 (节假日除外)</p>
                </div>
              </div>
            </div>
            
            <!-- 微信二维码：在此处添加微信二维码图片 -->
            <div class="mt-8">
              <h4 class="font-semibold text-primary mb-3">微信咨询</h4>
              <div class="bg-gray-100 p-4 inline-block rounded-md">
                <img src="cad5562bd2142c40b44fe2b289e3b994.jpg" alt="微信二维码" class="w-32 h-32 object-contain">
              </div>
            </div>
            
            <!-- 地图：可替换为实际地图 -->
            <div class="mt-8">
              <h4 class="font-semibold text-primary mb-3">公司位置</h4>
              <div class="w-full h-64 bg-gray-200 rounded-md overflow-hidden">
                <img src="map-location.jpg" alt="公司位置地图" class="w-full h-full object-cover">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 页脚 -->
  <footer class="bg-primary text-white pt-16 pb-8">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8 mb-12">
        <div>
          <div class="flex items-center space-x-2 mb-6">
            <div class="w-10 h-10 bg-white rounded-md flex items-center justify-center">
              <span class="text-primary font-bold text-xl">锦鹰</span>
            </div>
            <span class="font-bold text-lg">锦鹰自动化</span>
          </div>
          <p class="text-white/70 mb-6">
            专注于压铸行业自动化解决方案，提供高品质自动化机器设备，助力企业提升生产效率与产品质量。
          </p>
          <div class="flex space-x-4">
            <a href="#" class="bg-white/10 hover:bg-accent w-10 h-10 rounded-full flex items-center justify-center transition-colors">
              <i class="fa fa-weixin"></i>
            </a>
            <a href="#" class="bg-white/10 hover:bg-accent w-10 h-10 rounded-full flex items-center justify-center transition-colors">
              <i class="fa fa-weibo"></i>
            </a>
            <a href="#" class="bg-white/10 hover:bg-accent w-10 h-10 rounded-full flex items-center justify-center transition-colors">
              <i class="fa fa-linkedin"></i>
            </a>
            <a href="#" class="bg-white/10 hover:bg-accent w-10 h-10 rounded-full flex items-center justify-center transition-colors">
              <i class="fa fa-youtube-play"></i>
            </a>
          </div>
        </div>
        
        <div>
          <h4 class="text-lg font-semibold mb-6">快速链接</h4>
          <ul class="space-y-3">
            <li><a href="#home" class="text-white/70 hover:text-accent transition-colors">首页</a></li>
            <li><a href="#about" class="text-white/70 hover:text-accent transition-colors">关于我们</a></li>
            <li><a href="#products" class="text-white/70 hover:text-accent transition-colors">产品中心</a></li>
            <li><a href="#cases" class="text-white/70 hover:text-accent transition-colors">应用案例</a></li>
            <li><a href="#contact" class="text-white/70 hover:text-accent transition-colors">联系我们</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-semibold mb-6">产品系列</h4>
          <ul class="space-y-3">
            <li><a href="#" class="text-white/70 hover:text-accent transition-colors">压铸机器人</a></li>
            <li><a href="#" class="text-white/70 hover:text-accent transition-colors">自动化生产线</a></li>
            <li><a href="#" class="text-white/70 hover:text-accent transition-colors">检测设备</a></li>
            <li><a href="#" class="text-white/70 hover:text-accent transition-colors">辅助设备</a></li>
            <li><a href="#" class="text-white/70 hover:text-accent transition-colors">自动化控制系统</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-semibold mb-6">联系我们</h4>
          <ul class="space-y-3">
            <li class="flex items-start">
              <i class="fa fa-map-marker mt-1 mr-3 text-accent"></i>
              <span class="text-white/70">广东省东莞市清溪镇三星村三星路2号</span>
            </li>
            <li class="flex items-center">
              <i class="fa fa-phone mr-3 text-accent"></i>
              <span class="text-white/70">13829267422</span>
            </li>
            <li class="flex items-center">
              <i class="fa fa-envelope mr-3 text-accent"></i>
              <span class="text-white/70">ozyrro@163.com</span>
            </li>
          </ul>
        </div>
      </div>
      
      <div class="border-t border-white/10 pt-8">
        <div class="flex flex-col md:flex-row justify-between items-center">
          <p class="text-white/50 text-sm mb-4 md:mb-0">
            &copy; 2023 东莞市锦鹰自动化设备有限公司 版权所有 | 粤ICP备XXXXXXXX号
          </p>
          <div class="flex space-x-6">
            <a href="#" class="text-white/50 hover:text-white text-sm transition-colors">隐私政策</a>
            <a href="#" class="text-white/50 hover:text-white text-sm transition-colors">服务条款</a>
            <a href="#" class="text-white/50 hover:text-white text-sm transition-colors">网站地图</a>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- 返回顶部按钮 -->
  <button id="backToTop" class="fixed bottom-8 right-8 bg-primary hover:bg-accent text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center transition-all opacity-0 pointer-events-none z-50">
    <i class="fa fa-angle-up text-xl"></i>
  </button>

  <!-- JavaScript -->
  <script>
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    const backToTop = document.getElementById('backToTop');
    
    window.addEventListener('scroll', function() {
      if (window.scrollY > 50) {
        navbar.classList.add('bg-primary', 'shadow-md');
        navbar.classList.remove('bg-transparent');
        
        backToTop.classList.remove('opacity-0', 'pointer-events-none');
        backToTop.classList.add('opacity-100', 'pointer-events-auto');
      } else {
        navbar.classList.remove('bg-primary', 'shadow-md');
        navbar.classList.add('bg-transparent');
        
        backToTop.classList.add('opacity-0', 'pointer-events-none');
        backToTop.classList.remove('opacity-100', 'pointer-events-auto');
      }
    });
    
    // 移动端菜单
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    let menuOpen = false;
    
    menuBtn.addEventListener('click', function() {
      if (menuOpen) {
        mobileMenu.classList.add('-translate-y-full', 'opacity-0', 'pointer-events-none');
        mobileMenu.classList.remove('translate-y-0', 'opacity-100', 'pointer-events-auto');
        menuBtn.innerHTML = '<i class="fa fa-bars"></i>';
      } else {
        mobileMenu.classList.remove('-translate-y-full', 'opacity-0', 'pointer-events-none');
        mobileMenu.classList.add('translate-y-0', 'opacity-100', 'pointer-events-auto');
        menuBtn.innerHTML = '<i class="fa fa-times"></i>';
      }
      menuOpen = !menuOpen;
    });
    
    // 平滑滚动
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        // 关闭移动菜单（如果打开）
        if (menuOpen) {
          mobileMenu.classList.add('-translate-y-full', 'opacity-0', 'pointer-events-none');
          mobileMenu.classList.remove('translate-y-0', 'opacity-100', 'pointer-events-auto');
          menuBtn.innerHTML = '<i class="fa fa-bars"></i>';
          menuOpen = false;
        }
        
        const targetId = this.getAttribute('href');
        const targetElement = document.querySelector(targetId);
        
        if (targetElement) {
          window.scrollTo({
            top: targetElement.offsetTop - 80,
            behavior: 'smooth'
          });
        }
      });
    });
    
    // 返回顶部
    backToTop.addEventListener('click', function() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    });
    
    // 效率对比图表
    const ctx = document.getElementById('efficiencyChart').getContext('2d');
    const efficiencyChart = new Chart(ctx, {
      type: 'bar',
      data: {
        labels: ['生产效率', '产品合格率', '人力成本', '能耗成本', '生产周期'],
        datasets: [
          {
            label: '自动化前',
            data: [60, 85, 100, 90, 80],
            backgroundColor: 'rgba(255, 255, 255, 0.5)',
            borderColor: 'rgba(255, 255, 255, 0.8)',
            borderWidth: 1
          },
          {
            label: '自动化后',
            data: [95, 98, 30, 60, 40],
            backgroundColor: 'rgba(230, 179, 37, 0.8)',
            borderColor: 'rgba(230, 179, 37, 1)',
            borderWidth: 1
          }
        ]
      },
      options: {
        responsive: true,
        maintainAspectRatio: false,
        scales: {
          y: {
            beginAtZero: true,
            max: 100,
            ticks: {
              color: 'rgba(255, 255, 255, 0.7)'
            },
            grid: {
              color: 'rgba(255, 255, 255, 0.1)'
            }
          },
          x: {
            ticks: {
              color: 'rgba(255, 255, 255, 0.7)'
            },
            grid: {
              color: 'rgba(255, 255, 255, 0.1)'
            }
          }
        },
        plugins: {
          legend: {
            labels: {
              color: 'rgba(255, 255, 255, 0.9)'
            }
          }
        }
      }
    });
    
    // 客户评价轮播
    const track = document.querySelector('.testimonial-track');
    const prevBtn = document.querySelector('.testimonial-prev');
    const nextBtn = document.querySelector('.testimonial-next');
    const dots = document.querySelectorAll('.testimonial-dot');
    let currentSlide = 0;
    const slideCount = document.querySelectorAll('.testimonial-item').length;
    
    function updateSlidePosition() {
      let slideWidth = 100;
      if (window.innerWidth >= 768 && window.innerWidth < 1024) {
        slideWidth = 50; // 平板显示2个
      } else if (window.innerWidth >= 1024) {
        slideWidth = 33.333; // 桌面显示3个
      }
      
      track.style.transform = `translateX(-${currentSlide * slideWidth}%)`;
      
      // 更新指示器
      dots.forEach((dot, index) => {
        if (index === currentSlide) {
          dot.classList.add('bg-primary');
          dot.classList.remove('bg-gray-300');
        } else {
          dot.classList.remove('bg-primary');
          dot.classList.add('bg-gray-300');
        }
      });
    }
    
    prevBtn.addEventListener('click', () => {
      currentSlide = Math.max(0, currentSlide - 1);
      updateSlidePosition();
    });
    
    nextBtn.addEventListener('click', () => {
      let maxSlide = slideCount - 1;
      if (window.innerWidth >= 768 && window.innerWidth < 1024) {
        maxSlide = slideCount - 2;
      } else if (window.innerWidth >= 1024) {
        maxSlide = slideCount - 3;
      }
      
      currentSlide = Math.min(maxSlide, currentSlide + 1);
      updateSlidePosition();
    });
    
    dots.forEach((dot, index) => {
      dot.addEventListener('click', () => {
        currentSlide = index;
        updateSlidePosition();
      });
    });
    
    // 窗口大小变化时重新计算
    window.addEventListener('resize', updateSlidePosition);
    
    // 产品筛选
    const filterButtons = document.querySelectorAll('.product-filter');
    
    filterButtons.forEach(button => {
      button.addEventListener('click', () => {
        // 移除所有按钮的active状态
        filterButtons.forEach(btn => {
          btn.classList.remove('active', 'bg-primary', 'text-white');
          btn.classList.add('bg-gray-100', 'hover:bg-primary/10');
        });
        
        // 添加当前按钮的active状态
        button.classList.add('active', 'bg-primary', 'text-white');
        button.classList.remove('bg-gray-100', 'hover:bg-primary/10');
        
        // 这里可以添加实际的筛选逻辑
      });
    });
  </script>
</body>
</html>
