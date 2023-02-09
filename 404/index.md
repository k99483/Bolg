---
title: "404 - 真巧，竟然在這裡遇到你！"
date: 2023-02-09 21:02:31
comments: false
permalink: /404.html
---

<!-- markdownlint-disable MD039 MD033 -->

## 這是一個不存在的頁面

很抱歉，你目前存取的頁面並不存在。

預計將在約 <span id="timeout">5</span> 秒後返回首頁。

如果你很急著想看文章，你可以 **[點這裡](https://cooperwu.com/)** 返回首頁。

<script>
let countTime = 5000;

function count() {
  
  document.getElementById('timeout').textContent = countTime;
  countTime -= 1;
  if(countTime === 0){
    location.href = 'https://cooperwu.com';
  }
  setTimeout(() => {
    count();
  }, 1000);
}

count();
</script>
