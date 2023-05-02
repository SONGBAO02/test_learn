<template>
  <div id="aCoursesList" class="bg-fa of">
    <!-- 轮播图bannner  -->
    <div class="page">
      <div class="banner">
        <div class="banner-left" style="height: 360px;">
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">国家精品</a>
            </span>
            <span class="subject"></span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" class="subject1" target="_blank" rel="noopener noreferrer">计算机</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="大数据与人工智能" target="_blank" rel="noopener noreferrer">大数据与人工智能</a>
              <span>/</span>
              <a href="#" class="subject1" title="软件工程" target="_blank" rel="noopener noreferrer">软件工程</a>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">外语</a>
            </span>
            <span class="subject">
              <span class="subject">
                <a href="#" class="subject1" title="听力/口语" target="_blank" rel="noopener noreferrer">听力/口语</a>
                <span>/</span>
                <a href="#" class="subject1" title="写作/翻译" target="_blank" rel="noopener noreferrer">写作/翻译</a>
              </span>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">理学工学农学</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="数学" target="_blank" rel="noopener noreferrer">数学</a>
              <span>/</span>
              <a href="#" class="subject1" title="物理" target="_blank" rel="noopener noreferrer">物理</a>
              <span>/</span>
              <a href="#" class="subject1" title="化学" target="_blank" rel="noopener noreferrer">化学</a>
              <span>/</span>
              <a href="#" class="subject1" title="天文学" target="_blank" rel="noopener noreferrer">天文学</a>
              <span>/</span>
              <a href="#" class="subject1" title="地理学" target="_blank" rel="noopener noreferrer">地理学</a>
              <span>/</span>
              <a href="#" class="subject1" title="生物科学" target="_blank" rel="noopener noreferrer">生物科学</a>
              <span>/</span>
              <a href="#" class="subject1" title="机械" target="_blank" rel="noopener noreferrer">机械</a>
              <span>/</span>
              <a href="#" class="subject1" title="电气信息" target="_blank" rel="noopener noreferrer">电气信息</a>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">考研</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="数学" target="_blank" rel="noopener noreferrer">数学</a>
              <span>/</span>
              <a href="#" class="subject1" title="英语" target="_blank" rel="noopener noreferrer">英语</a>
              <span>/</span>
              <a href="#" class="subject1" title="政治" target="_blank" rel="noopener noreferrer">政治</a>
              <span>/</span>
              <a href="#" class="subject1" title="408计算机" target="_blank" rel="noopener noreferrer">408计算机</a>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">期末突击</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="数学" target="_blank" rel="noopener noreferrer">数学</a>
              <span>/</span>
              <a href="#" class="subject1" title="物理" target="_blank" rel="noopener noreferrer">物理</a>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">四六级</a>
            </span>
            <span class="subject"></span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">大学应试英语</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="四六级" target="_blank" rel="noopener noreferrer">四六级</a>
              <span>/</span>
              <a href="#" class="subject1" title="考研英语" target="_blank" rel="noopener noreferrer">考研英语</a>
            </span>
          </div>
          <div class="banner-left-course">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">专升本</a>
            </span>
            <span class="subject">
              <a href="#" class="subject1" title="广东" target="_blank" rel="noopener noreferrer">广东</a>
              <span>/</span>
              <a href="#" class="subject1" title="广西" target="_blank" rel="noopener noreferrer">广西</a>
              <span>/</span>
              <a href="#" class="subject1" title="云南" target="_blank" rel="noopener noreferrer">云南</a>
              <span>/</span>
              <a href="#" class="subject1" title="广西" target="_blank" rel="noopener noreferrer">浙江</a>
              <span>/</span>
              <a href="#" class="subject1" title="广西" target="_blank" rel="noopener noreferrer">黑龙江</a>
              <span>/</span>
            </span>
          </div>
          <div class="banner-left-course more">
            <span class="banner-left-course-tpye">
              <a href="#" target="_blank" rel="noopener noreferrer">更多</a>
            </span>
            <span class="subject"> <img src="~/assets/img/more.png" alt=""></span>
          </div>
        </div>

        <!-- <幻灯片开始> -->
        <div v-swiper:mySwiper="swiperOption" class="banner-middle">
          <div class="swiper-wrapper">
            <div v-for="banner in bannerList" :key="banner.id" class="swiper-slide" style="background: #040b1b">
              <a target="_blank" :href="banner.linkUrl">
                <img :src="banner.imageUrl" :alt="banner.title" />
              </a>
            </div>
          </div>
          <div class="swiper-pagination swiper-pagination-white"></div>
          <div class="swiper-button-prev swiper-button-white" slot="button-prev"></div>
          <div class="swiper-button-next swiper-button-white" slot="button-next"></div>
        </div>
        <!-- <幻灯片结束> -->

        <div class="banner-right">
          <div class="user pad">
            <a href="#"><img class="circleImg1" src="~/assets/img/user1.png" alt=""></a>
          </div>
          <div class=" user1">
            蜡笔小金
          </div>
          <div class="Collect-courses">
            <a href="#">
              <div class="courses">大学物理-力学与热学</div>
            </a>
            <a href="#">
              <div class="courses">计算机组成原理</div>
            </a>
            <a href="#">
              <div class="courses">计算机数据结构</div>
            </a>
          </div>

          <div class="MyCourses">
            <div class="MyCourses1" role="button" tabindex="0">我的课程</div>
          </div>
        </div>
      </div>
    </div>

    <!-- 热门课程 -->
    <div class="wrapper">
      <section class="container">
        <header class="comm-title">
          <h2 class="tac">
            <span class="c-333">热门课程</span>
          </h2>
        </header>
        <article class="comm-course-list">
          <ul class="of" id="bna">
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295592705.jpg" class="img-responsive" alt="听力口语">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="听力口语" class="course-title fsize18 c-333">听力口语</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">9634人学习</i>
                    |
                    <i class="c-999 f-fA">9634评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295581911.jpg" class="img-responsive" alt="Java精品课程">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="Java精品课程" class="course-title fsize18 c-333">Java精品课程</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">501人学习</i>
                    |
                    <i class="c-999 f-fA">501评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295604295.jpg" class="img-responsive" alt="C4D零基础">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="C4D零基础" class="course-title fsize18 c-333">C4D零基础</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">300人学习</i>
                    |
                    <i class="c-999 f-fA">300评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442302831779.jpg" class="img-responsive" alt="数学给宝宝带来的兴趣">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="数学给宝宝带来的兴趣" class="course-title fsize18 c-333">数学给宝宝带来的兴趣</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">256人学习</i>
                    |
                    <i class="c-999 f-fA">256评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295455437.jpg" class="img-responsive" alt="零基础入门学习Python课程学习">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="零基础入门学习Python课程学习" class="course-title fsize18 c-333">零基础入门学习Python课程学习</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">137人学习</i>
                    |
                    <i class="c-999 f-fA">137评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295570359.jpg" class="img-responsive" alt="MySql从入门到精通">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="MySql从入门到精通" class="course-title fsize18 c-333">MySql从入门到精通</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">125人学习</i>
                    |
                    <i class="c-999 f-fA">125评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442302852837.jpg" class="img-responsive" alt="搜索引擎优化技术">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="搜索引擎优化技术" class="course-title fsize18 c-333">搜索引擎优化技术</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">123人学习</i>
                    |
                    <i class="c-999 f-fA">123评论</i>
                  </span>
                </section>
              </div>
            </li>
            <li>
              <div class="cc-l-wrap">
                <section class="course-img">
                  <img src="~/assets/photo/course/1442295379715.jpg" class="img-responsive" alt="20世纪西方音乐">
                  <div class="cc-mask">
                    <a href="/course/1" title="开始学习" class="comm-btn c-btn-1">开始学习</a>
                  </div>
                </section>
                <h3 class="hLh30 txtOf mt10">
                  <a href="/course/1" title="20世纪西方音乐" class="course-title fsize18 c-333">20世纪西方音乐</a>
                </h3>
                <section class="mt10 hLh20 of">
                  <span class="fr jgTag bg-green">
                    <i class="c-fff fsize12 f-fA">免费</i>
                  </span>
                  <span class="fl jgAttr c-ccc f-fA">
                    <i class="c-999 f-fA">34人学习</i>
                    |
                    <i class="c-999 f-fA">34评论</i>
                  </span>
                </section>
              </div>
            </li>
          </ul>
        </article>
      </section>
    </div>

    <!-- 名师优选 -->
    <div class="wrapper">
      <section class="container">
        <header class="comm-title">
          <h2 class="tac">
            <span class="c-333">名师优选</span>
          </h2>
        </header>
        <article class="i-teacher-list">
          <ul class="of">
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="姚晨" target="_blank">
                    <img src="~/assets/photo/teacher/1442297885942.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="姚晨" target="_blank" class="fsize18 c-666">姚晨</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">北京师范大学法学院副教授、清华大学法学博士。自2004年至今已有9年的司法考试培训经验。长期从事司法考试辅导，深知命题规律，了解解题技巧。内容把握准确，授课重点明确，层次分明，调理清晰，将法条法理与案例有机融合，强调综合，深入浅出。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">北京师范大学法学院副教授</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="谢娜" target="_blank">
                    <img src="~/assets/photo/teacher/1442297919077.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="谢娜" target="_blank" class="fsize18 c-666">谢娜</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">十年课程研发和培训咨询经验，曾任国企人力资源经理、大型外企培训经理，负责企业大学和培训体系搭建；曾任专业培训机构高级顾问、研发部总监，为包括广东移动、东莞移动、深圳移动、南方电网、工商银行、农业银行、民生银行、邮储银行、TCL集团、清华大学继续教育学院、中天路桥、广西扬翔股份等超过200家企业提供过培训与咨询服务，并担任近50个大型项目的总负责人。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">资深课程设计专家，专注10年AACTP美国培训协会认证导师</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="刘德华" target="_blank">
                    <img src="~/assets/photo/teacher/1442297927029.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="刘德华" target="_blank" class="fsize18 c-666">刘德华</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">上海师范大学法学院副教授、清华大学法学博士。自2004年至今已有9年的司法考试培训经验。长期从事司法考试辅导，深知命题规律，了解解题技巧。内容把握准确，授课重点明确，层次分明，调理清晰，将法条法理与案例有机融合，强调综合，深入浅出。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">上海师范大学法学院副教授</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="周润发" target="_blank">
                    <img src="~/assets/photo/teacher/1442297935589.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="周润发" target="_blank" class="fsize18 c-666">周润发</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">法学博士，北京师范大学马克思主义学院副教授，专攻毛泽东思想概论、邓小平理论，长期从事考研辅导。出版著作两部，发表学术论文30余篇，主持国家社会科学基金项目和教育部重大课题子课题各一项，参与中央实施马克思主义理论研究和建设工程项目。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">考研政治辅导实战派专家，全国考研政治命题研究组核心成员。</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="钟汉良" target="_blank">
                    <img src="~/assets/photo/teacher/1442298121626.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="钟汉良" target="_blank" class="fsize18 c-666">钟汉良</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span class="fsize14 c-999">具备深厚的数学思维功底、丰富的小学教育经验，授课风格生动活泼，擅长用形象生动的比喻帮助理解、简单易懂的语言讲解难题，深受学生喜欢</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">毕业于师范大学数学系，热爱教育事业，执教数学思维6年有余</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="唐嫣" target="_blank">
                    <img src="~/assets/photo/teacher/1442297957332.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="唐嫣" target="_blank" class="fsize18 c-666">唐嫣</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">中国科学院数学与系统科学研究院应用数学专业博士，研究方向为数字图像处理，中国工业与应用数学学会会员。参与全国教育科学“十五”规划重点课题“信息化进程中的教育技术发展研究”的子课题“基与课程改革的资源开发与应用”，以及全国“十五”科研规划全国重点项目“掌上型信息技术产品在教学中的运用和开发研究”的子课题“用技术学数学”。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">中国人民大学附属中学数学一级教师</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="周杰伦" target="_blank">
                    <img src="~/assets/photo/teacher/1442297969808.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="周杰伦" target="_blank" class="fsize18 c-666">周杰伦</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span class="fsize14 c-999">中教一级职称。讲课极具亲和力。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">毕业于北京大学数学系</p>
                </div>
              </section>
            </li>
            <li>
              <section class="i-teach-wrap">
                <div class="i-teach-pic">
                  <a href="/teacher/1" title="陈伟霆" target="_blank">
                    <img src="~/assets/photo/teacher/1442297977255.jpg" alt>
                  </a>
                </div>
                <div class="mt10 hLh30 txtOf tac">
                  <a href="/teacher/1" title="陈伟霆" target="_blank" class="fsize18 c-666">陈伟霆</a>
                </div>
                <div class="hLh30 txtOf tac">
                  <span
                    class="fsize14 c-999">政治学博士、管理学博士后，北京师范大学马克思主义学院副教授。多年来总结出了一套行之有效的应试技巧与答题方法，针对性和实用性极强，能帮助考生在轻松中应考，在激励的竞争中取得高分，脱颖而出。</span>
                </div>
                <div class="mt15 i-q-txt">
                  <p class="c-999 f-fA">长期从事考研政治课讲授和考研命题趋势与应试对策研究。考研辅导新锐派的代表。</p>
                </div>
              </section>
            </li>
          </ul>
        </article>
      </section>
    </div>
  </div>
</template>

<script>
import banner from '@/api/banner'
// import index from '@api/index'
export default {
  data() {
    return {
      swiperOption: {
        //配置分页
        pagination: {
          el: '.swiper-pagination'//分页的dom节点
        },
        autoplay: {
          delay: 2000,
          speed: 800,
        },
        //配置导航
        navigation: {
          nextEl: '.swiper-button-next',//下一页dom节点
          prevEl: '.swiper-button-prev'//前一页dom节点
        }
      },
      //banner数组
      bannerList: [],
      // eduList:[],
      // teacherList:[]
    }
  },
  created() {
    //调用查询banner的方法
    this.getBannerList()

  },
  methods: {
    //查询热门课程和名师
    // getHotCourseTeacher() {
    //   index.getIndexData()
    //     .then(response => {
    //       this.eduList = response.data.data.eduList
    //       this.teacherList = response.data.data.teacherlist
    //     }
    //     )
    // },

    //查询banner数据
    getBannerList() {
      banner.getListBanner()
        .then(response => {
          this.bannerList = response.data.data.list
        }

        )
    }

  }
}

</script>


<style scoped>
* {
  /* 內减模式 */
  box-sizing: border-box;
}

li {
  list-style: none;
}

a {
  text-decoration: none;
}

.clearfix:before,
.clearfix:after {
  content: "";
  display: table;
}

.clearfix:after {
  clear: both;
}

body {
  background-color: #f3f5f7;
}


/* 版心 */

.wrapper {
  width: 1200px;
  margin: 0 auto;
}

.navtop {
  height: 60px;
  background-color: #ffffff;
}

.header {
  height: 60px;
  background-color: #ffffff;
  padding: 30px auto;
}

h1 {
  float: left;
}

.nav {
  float: left;
  margin-left: 70px;
  height: 60px;
}

.nav li {
  float: left;
  margin-right: 26px;
}

.Personal-Center,
.nav li a {
  display: block;
  padding: 0 9px;
  height: 60px;
  line-height: 60px;
  font-size: 16px;
  color: #050505;
}

.Personal-Center:hover,
.nav li a:hover {
  border-bottom: 2px solid #00a4ff;
}


/* 搜索 */

.search {
  float: left;
  margin-left: 59px;
  margin-top: 10px;
  /* border-radius: 20px; */
  width: 310px;
  height: 40px;
  border: 1px solid #00a4ff;
}

.search input {
  float: left;
  padding-left: 10px;
  /* 左右加一起的尺寸要小于等于410 */
  width: 258px;
  height: 38px;
  border: 0;
}


/* 控制placeholder的样式 */

.search input::placeholder {
  font-size: 14px;
  color: #bfbfbf;
}

.search button {
  float: left;
  width: 50px;
  height: 39px;
  background-image: url(~/assets/img/btn.png);
  border: 0;
  cursor: pointer;

}


/* 个人中心 */

.Personal-Center {
  float: left;
  margin-left: 80px;
}

.user {
  float: right;
  margin-right: 55px;
  height: 60px;
  line-height: 60px;
}

.circleImg {
  border-radius: 20px;
  width: 40px;
  height: 40px;
  margin: 0 auto;
}

.user img {
  /* 调节图片垂直对齐方式, middle:居中 */
  vertical-align: middle;
}


/* 轮播图banner */

.page {
  width: 1200px;
  margin: 0 auto;
}

.banner {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  width: 1200px;
  margin: 20px 0;
  margin-bottom: 12px;
  position: relative;
}


/* banner-left */

.banner-left {
  box-sizing: border-box;
  display: flex;
  flex-flow: column nowrap;
  width: 200px;
  height: 360px;
  padding: 10px 0;
  border-radius: 8px;
  background-color: rgb(255, 255, 255);
  position: absolute;
  transition: all 0.2s;
  left: 0;
  z-index: 9;
}

.banner-left .banner-left-course {
  box-sizing: border-box;
  width: 200px;
  height: 34px;
  padding: 0 12px;
  line-height: 34px;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow: hidden;
  color: rgb(153, 153, 153);
}

.banner-left .banner-left-course:hover {
  background-color: skyblue;
  color: #27ff9c;
}

.banner-left .banner-left-course .banner-left-course-tpye {
  margin-right: 8px;
  font-size: 14px;
  font-weight: 500;
  color: rgb(51, 51, 51);
}

.banner-left a {
  color: inherit;
  transition: all 0.2s;
}

.banner-left .banner-left-course .subject {
  line-height: 17px;
  font-size: 12px;
  font-weight: 400;
}


/* banner-middle */

.banner-middle {
  position: relative;
  margin: 0px;
  width: 776px;
  height: 360px;
  border-radius: 8px;
  left: 212px;
  background-color: rgb(255, 255, 255);
  /* background-image: url(~/assets/img/banner.png); */
}


/* banner-right */

.banner-right {
  box-sizing: border-box;
  position: relative;
  display: flex;
  flex-flow: column nowrap;
  -ms-flex-align: center;
  align-items: center;
  width: 200px;
  height: 360px;
  border-radius: 8px;
  background-color: rgb(255, 255, 255);
}

.pad,
.MyCourses {
  margin: 20px;
}

.circleImg1 {
  border-radius: 30px;
  width: 60px;
  height: 60px;
  margin: 0 auto;
}

.user1 {
  font-size: 12px;
}

.Collect-courses {
  margin-top: 20px;
  line-height: 100px;
  height: 100px;
}

.courses {
  line-height: 30px;
  height: 30px;
  font-size: 14px;
  color: #888888;
}

.Collect-courses .courses:hover {
  color: #00CC7E;
}

.banner-right .MyCourses .MyCourses1 {
  width: 168px;
  height: 32px;
  border-radius: 18px;
  line-height: 32px;
  font-size: 14px;
  text-align: center;
  color: rgb(255, 255, 255);
  background-color: #00CC7E;
  outline: none;
  cursor: pointer;
  transition: 0.1s all;
}
</style>