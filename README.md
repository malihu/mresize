# mresize
Event based jQuery element resize 

The plugin does not use any kind of timer(s) to detect size changes. It uses the resize event on (invincible) iframe(s) which makes it perform much better than other solutions which use timers to poll element size. The script detects size changes made from JS, CSS, animations etc. and it works on any element able to contain other elements (e.g. div, p, li etc.). To use it on other inline elements (e.g. images) you need to add a wrapper and call the event on it. 

#### Usage 

`
$(selector).on("mresize",function(){
	console.log($(this));
});
` 
