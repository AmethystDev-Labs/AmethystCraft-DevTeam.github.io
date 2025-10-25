---
layout: page
---
<script setup>
import {
  VPTeamPage,
  VPTeamPageTitle,
  VPTeamMembers
} from 'vitepress/theme'

// 团队成立时间（可以设定你实际的成立日期）
const establishedDate = new Date('2024-08-22'); // 设定成立日期为 2023-01-01

// 获取当前时间 
const currentDate = new Date(); 

// 计算日期差（以天为单位）
const timeDiff = currentDate - establishedDate;
const daysDiff = Math.floor(timeDiff / (1000 * 60 * 60 * 24));

// 生成显示的文本
const durationText = daysDiff === 0 ? '今天成立' : `已经成立了 ${daysDiff} 天`;

const members = [
  {
    avatar: 'https://www.github.com/Starry-Sky-World.png',
    name: 'Starry-Sky-World',
    title: '创始人/机器人开发',
    links: [
      { icon: 'github', link: 'https://github.com/Starry-Sky-World' }
    ]
  },
  {
    avatar: 'http://q.qlogo.cn/headimg_dl?dst_uin=3773898834&spec=640&img_type=jpg',
    name: 'Color111111',
    title: '联合创始人/插件or机器人测试',
    links: []
  },
  {
    avatar: 'https://p.qlogo.cn/gh/952518546/952518546/640/',
    name: 'Github团队',
    title: 'Github团队',
    links: [
      { icon: 'github', link: 'https://github.com/AmethystCraft-DevTeam' }
    ]
  },
]
</script>

<VPTeamPage>
  <VPTeamPageTitle>
    <template #title>
      AmethystCraft团队
    </template>
    <template #lead>
      {{ durationText }}，感谢每个人的付出！
    </template>
  </VPTeamPageTitle>
  <VPTeamMembers
    :members="members"
  />
</VPTeamPage>
