---
title: "Message Board"
---

## Message Board

Good communication is the beginning of learning and progress, welcome to contact me!

<div id="disqus_thread"></div>
<script>
    var disqus_config = function () {
        this.page.url = '{{ .Permalink }}';
        this.page.identifier = '{{ .Path }}';
    };
    (function() {
        var d = document, s = d.createElement('script');
        s.src = 'https://yi-zhou.disqus.com/embed.js';
        s.setAttribute('data-timestamp', +new Date());
        (d.head || d.body).appendChild(s);
    })();
</script>
