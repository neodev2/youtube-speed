# youtube-speed

```javascript

var video = document.querySelectorAll('.html5-main-video')[0];

var speed = document.createElement('input');
speed.setAttribute('class','speed');
speed.setAttribute('type','range');
speed.setAttribute('min','0.5');
speed.setAttribute('max','4');
speed.setAttribute('step','0.01');
speed.setAttribute('value','1');
speed.setAttribute('style','position: absolute; z-index: 99999999999; top: 140px; left: 20px; display: block; width: 150px;');
speed.value = video.playbackRate;
document.body.appendChild(speed);

speed.oninput = function(){
    video.playbackRate = this.value;
}

```
