# remove-disqus-ads
like the name


<script>	
//let attemps=0;
const clearDsq = setInterval(() => {
	//console.log(attemps++)
	document.querySelectorAll('iframe[name^=dsq]').forEach(element => 	{
		if (element.getAttribute('src') == null) { 
			element.remove(); 
			clearInterval(clearDsq);
		}	
	})
}, 400);

</script>	
