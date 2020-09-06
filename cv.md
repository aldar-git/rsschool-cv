# Aldar Amteev

* Telegram: [Aldar Amteev(@folkrit)](https://t.me/folkrit)

## Summary

My goal is to improve my programming skills

## Skills

* C#
* MS SQL
* HTML/CSS
* PHP
* JS

## Code examples

File transfer and getting the result via Ajax
```javascript
function plagiat(){
	$("#loadImg").show();
	var datafile = new FormData();
	datafile.append('userfile', $('#userfile').prop('files')[0])
	if ($('#userfile').prop('files')[0]==null)
	{
		alert("Необходимо выбрать файл");
		$("#loadImg").hide();
	}
	else
	{
		$.ajax({
			type: 'POST',
			url: "../js/ajax/antiplagiat.php",
			data: datafile,
			dataType: 'text',
			cache: false,
			contentType: false,
			processData: false,
			success: function(result){
				$("#resultTab").html(result);
				his();
				$("#loadImg").hide();
			},
			error:  function(xhr, str){
				alert('Возникла ошибка: ' + xhr.responseCode);
				$("#loadImg").hide();
			}
		});
	}
}
```

## Experience 

* Graduation work
* Kalmyk State University, lead developer, department of information
* Pension Fund of the Russian Federation, specialist, information technology department