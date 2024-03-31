
Notes & Potentially incorrect things with my explanation:

the sticky-header has an overflow issue 
between 1026px - 1126px, and I can't set overflow: scroll or overflow: hidden for a couple of reasons:

1. I hate that on google chrome, having an element with overflow: scroll, shows the scrollbar regardless. 

2. Since I'm using checkbox:checked toggle in place of js, setting overflow can cause the toggle functionality to not perform. 

For the mobile menu, when toggles, typically takes the full-height of the screen. Since I'm using toggle, I can't have the menu blocking the toggle checkbox. Hence, why the different modals are beneath the checkbox. That is all. 

Toggle functionalities:
1. Header Artists dropdown menu 
2. Header Mobile Menu sliding 
3. Footer currency toggle 
4. Cart Menu Toggle
5. popular work sort by toggle 

3rd Party JS libraries:

1. swiper.js


Cool things I've learned:

for autoplay to work, it should have muted attribute followed autoplay. 

Shocking things I've learned:

The mobile's menu toggles uses a negative left value,and when untoggled -- does not cause horizontal overflow. If the menu has a negative right value, it will cause horizontal overflow?! The solution if i want to have negative right value is to use position: fixed instead of position: absolute. Thats crazy. 

When using sticky header, and I have an element that is position absolute, and i also have an element that sits on top of the header and disappears when I start scrolling, the absolute element will shift down.... 
Thats quite fascinating and I never figured out why the absolute element shifts down until now.... 
