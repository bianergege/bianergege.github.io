---
layout:     post
title:      "新生代的粤语力量"
subtitle:   "80后歌手的情怀"
date:       2016-05-02 11:38:00
author:     "Fish"
header-img: "img/post-bg-markdown.jpg"
catalog:    true
tags:
    - 粤语
    - 新生代
    - 80后
    - 音乐
---

> 我只是一个听众，长期不定时更新

### **张敬轩**

或许很多人和我一样，听轩仔的第一首应该是《断点》，但真正让我入迷的，是他的粤语歌。

*《不吐不快》*

<script src="/js/jquery-1.7.2.min.js"></script>
<div id="player" style="display:none"></div>
<ul id="playlist"></ul>
<script type="text/javascript"> 
    (function($){
	// Settings
	var continous = true,
		autoplay = true,
		playlist = [
			{
				title: '不吐不快',
				mp3: '/music/butubukuai.mp3',
				content:'如果有人能在ktv唱出这首歌，那一定拥有不可小觑的唱功。开头那几个长句，真的好似不吐不快那般，要一下子将所有都倾吐，难得的是，张敬轩将这几句要么断气要么憋死的歌词唱的一气呵成，气息处理的井然有序，不负夕爷的词。',
				ogg: ''
			},
			{
				title: '悲剧人物',
				mp3: '/music/beijurenwu.mp3',
				content:'456',
				ogg: ''
			},
			{
				title: '城寨英雄',
				mp3: '/music/walls.mp3',
				content:'456',
				ogg: ''
			},
			{
				title: 'kimi',
				mp3: '/music/kimi.mp3',
				content:'456',
				ogg: ''
			},
			];

	// Load playlist
	for (var i=0; i<playlist.length; i++){
		var item = playlist[i];
		$('#playlist').append('<li>'+item.title+'</li>');
		$('#playlist').append(item.content);
	}

	var time = new Date(),
		currentTrack = 0,
		trigger = false,
		audio, isPlaying, playCounts;

	var play = function(){
		audio.play();
		isPlaying = true;
	}

	var pause = function(){
		audio.pause();
		isPlaying = false;
	}


	// Switch track
	var switchTrack = function(i){
		if (i < 0){
			track = currentTrack = playlist.length - 1;
		} else if (i >= playlist.length){
			track = currentTrack = 0;
		} else {
			track = i;
		}

		$('audio').remove();
		loadMusic(track);
		if (isPlaying == true) play();
	}

	// Fire when track ended
	var ended = function(){
		pause();
		audio.currentTime = 0;
		playCounts++;
		if (continous == true) isPlaying = true;
	}

	var beforeLoad = function(){
	var endVal = this.seekable && this.seekable.length ? this.seekable.end(0) : 0;
	$('.progress .loaded').css('width', (100 / (this.duration || 1) * endVal) +'%');
	}

	// Fire when track loaded completely
	var afterLoad = function(){
		if (autoplay == true) play();
	}

	// Load track
	var loadMusic = function(i){
		var item = playlist[i],
			newaudio = $('<audio>').html('<source src="'+item.mp3+'"><source src="'+item.ogg+'">').appendTo('#player');
		$('#playlist li').removeClass('playing').eq(i).addClass('playing');
		audio = newaudio[0];
		audio.addEventListener('progress', beforeLoad, false);
		audio.addEventListener('durationchange', beforeLoad, false);
		audio.addEventListener('canplay', afterLoad, false);
		audio.addEventListener('ended', ended, false);
	}

	loadMusic(currentTrack);
	$('#playlist li').each(function(i){
		var _i = i;
		$(this).on('click', function(){
			switchTrack(_i);
		});
	});

})(jQuery);
</script>

如果有人能在ktv唱出这首歌，那一定拥有不可小觑的唱功。开头那几个长句，真的好似不吐不快那般，要一下子将所有都倾吐，难得的是，张敬轩将这几句要么断气要么憋死的歌词唱的一气呵成，气息处理的井然有序，不负夕爷的词。

*《悲剧人物》*

*《春秋》*

*《青春常驻》*

*《酷爱》*

*《樱花树下》*

*《绯荔榭•少年》*

*《悔过诗》*

### **周柏豪**

*《够钟》*

*《宏愿》*

*《一事无成》*

*《无力挽回》*

### **洪卓立**

*《弥顿道》*

*《少年游记》*

*《请你别要说下去》*

### **许廷铿**

*《遗物》*

*《青春颂》*

*《面具》*

*《真相》*

### **陈柏宇**

*《你瞒我瞒》*

*《I Will Be Loving You》*

### **胡鸿钧**

*《明白了》*

*《化蝶》*

*《真相》*

*《棋逢对手》*

*《一生一心》*

### **C Allstar**

*《天梯》*

你可能不认识C Allstar，但你不能没听过《天梯》。这首由“爱情天梯”衍生出来的歌曲，先后由张智霖、twins、李克勤翻唱，但我想，最深入人心的，应该是C Allstar的原唱。相信听过我们的胡士托红馆演唱会的全场大合唱的人，没有办法不为之流泪，不仅仅是因为钊峰的哽咽，更是因为这首歌所赋予的不顾一切，为爱痴狂。

*《家书》*

*《无惧》*

### **林奕匡**

*《高山低谷》*

### **卫兰**

*《回电我》*

*《长痛短痛》*

### **吴若希**

*《爱我请留言》*

*《越难越爱》*

*《休止符》*

### **钟舒漫**

*《给自己的信》*

### **连诗雅**

*《水星逆行》*

*《说一句》*

### **方力申**

*《好心好报》*

*《ABC君》*

*《好好恋爱》*

*《无双谱》*

*《同屋住》*

*《在你遥远的附近》*

### **麦浚龙**

*《耿耿于怀》*

*《念念不忘》*

*《罗生门》*

*《弱水三千》*

### **吴雨霏**

*《吴哥窟》*

*《我本人》*

*《生命树》*

*《人非草木》*

*《杀她死》*

### **郑欣宜**

*《上心》*

*《直觉》*

*《忘记的理由》*

