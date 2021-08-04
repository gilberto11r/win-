html>
  <body>
    <script src="https://cdn.jsdelivr.net/npm/hls.js@latest"></script>
    <video id="video" controls></video>
    <script>
    if(Hls.isSupported())
    {
        var video = document.getElementById('video');
        var hls = new Hls();
        hls.loadSource('https://1rowsports.com/online/2/68.php?');
        hls.attachMedia(video);
        hls.on(Hls.Events.MANIFEST_PARSED,function()
        {
            video.play();
        });
    }
    else if (video.canPlayType('application/vnd.Apple.mpegurl'))
    {
        video.src = 'https://1rowsports.com/online/2/68.php?';
        video.addEventListener('canplay',function()
        {
            video.play();
        });
    }
    </script>
  </body>
</html>
