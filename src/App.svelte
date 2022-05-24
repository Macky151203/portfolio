<script>
	import Modal from './Home.svelte'
	import About from './About.svelte'
	import Mywork from './Mywork.svelte'
	let showmodal = false;
	let showabout = false;
	let showwork = false;
	const show = ()=>{
		showmodal=!showmodal;
	}
	const about = ()=>{
		showabout=!showabout;
	}
	const work = ()=>{
		showwork=!showwork;
	}
	

</script>
<Modal {showmodal} on:click={show} />
<About {showabout} on:click={about}  />
<Mywork {showwork} on:click={work} />
<main>
	<div class="navbar">
		
		<div class="item"><button on:click={show}>HOME</button></div>
		<div class="item"><button on:click={about}>ABOUT</button></div>
		<div class="item"><button on:click={work}>MY WORKS</button></div>
		

	</div>
	<div class="pc">
	<div class="partition">

	</div>

</div>
	<div class="body">

		
		<div class="namecont">
			<div class="name">
			</div>
		</div>
		<body>
			<div class="wrapper">
				<div class="static-text">I em</div>
				<div class="dynamic-text">
					<div class="li"><span>a frontend developer...</span></div>
					<div class="li"><span>Subro...</span></div>
					<div class="li"><span>a lazzyyy guy...</span></div>
					
				</div>
					
					
					

			</div>
	
		</body>
		<div class="bar">
			<div class="fitem"><a href="https://www.instagram.com/" target="_blank"><img src="data:image/jpeg;base64,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" alt="sry"></a></div>
			<div class="fitem"><a href="https://github.com/Macky151203" target="_blank"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQLy_HmTFeQfyzTIVXY2VdnwNep4Bgvtxl9jZd2Inz3Sw&s" alt="sry"></a></div>
			<div class="fitem"><a href="https://www.linkedin.com/feed/" target="_blank"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOEAAADhCAMAAAAJbSJIAAAAllBMVEUMZMX///8AYcQAWcFDf8nL3PIAWrzQ3vMAYcI0eclZjtAucslAgsz6/v3x9/sgbclOhM8AX8QAYsAAX70AV70AWMLm7vgAXb4sdsw5fsoRbsVmltK6z+iUt+AMZcGDrN3c6fNvnddiltWqwuPA0+r0+vyOrt+lweR9pduuyueUst9Lh81pldd1mtYdbcunxOXO4u7Z4fGRyVlRAAAEKUlEQVR4nO3ce1faMBzG8SblEpSCiUUuQrkMhsCc+v7f3Ko4KjW/yLY0WXOez9mf4Ml3vSW1NYoAAAAAAAAAAAAAAAAAAAAAAAAAAADgYiriIsqU72FURcapGnXHk5aMue+xVCCT6n56x960Z2OpMt8jsozz+Xve0Xqc+h6SXbKzYOeSfex7UBap+J591lThHI3awPxw5KGcVFUj0RayaRrI6UaUj8GTpfA9NivknApkvTC2YdwjC9lc+h6dBWpFB7JFCIXx1FDIRr6HZ0Fq2EkZewjgXNMnLhVH34a+x/fPeMdYOK3/gchvTIFsXf/ZKR+bC+u/DcW1cS/d1f84jFobU+H3ANYXadNU2PU9PAvkd0Ngz/forMgMhU/1P5Xm4h0ZmHQCOAzz68WEPNdsg9iE+ZH4QATeBTApPYqf9PvoKIh99E2qOxQ3jVvf47JHDT5fMl5GAQW+3tNvnF/4N3shwrhJc8Ljw/Q0Q13MJ4GcRc8IORjP99vZfpWlQe2gH3EZx7Gs/4IJAADqQ3DJX/+FM38vqHyKlA5Hhx+Pj49X43468P34CheEiz9Z+pTMlrvFaQ6YbNrblRpKf6vNbHRNKX2yT/kwSVd5XluzGGs//Ew9NfIGS/RYs3X2yUGzp7dpnMYu+zPql1mbp46f+XxeSCkVxrpt8+bmWJgJOTPeYP7m5QkWi4Wye0d94t3m3sNmtFao5OyLvle7zPnRaKlQCb6+IDBfXvddJ1oq5BH5WE7JXd/xwWilUKnJpYGM9a7dPk5mpfCWP18cmO+okdOtaKVwYHxm5ZP1wOWNPBuFneUfBTK2dHkzyEbhwfirco3NxOF+aqPw8rPMbzuHV34bhX+h4e6q6KnQ4ZM6ngrZyNlG9FXo7hfMvgp7zt7o8FXIDq52U2+FznbTKgovmgAsalq4mB0mQqjJYfvler98o6sWhevuYPh2C5jz4WD1ReMPR4soi4W91dmtXy7MK469o7mpvcLn8nRaSWPi9PzH/++FCXvW3LuXpoXxi6MllK1tqHtGLBMd0zccLYNtFR60W8T0wkqv7yTQVuGTfpfLuvRXkms3sxo7hQlx/yy7NayOO3Uq3MXExY148PFY6OZyYafwihqsXNJfGteoMCGXQoYfzxo1KmxSO2kkJvTLcXUq3BreraFnp3UqNLwT3aJPpnUqPNBjTV+CKDScFVv0t+pUaLiytegXq1BoCQoLKNRDYfVQWEChHgqrh8ICCvVQWD0UFlCoh8LqobCAQj0UVg+FBRTqobB6KCygUA+F1UNhAYV6KKweCgso1ENh9VBYQKEeCquHwkKAhe1SIf2UoaFwSP+/dB29FtTvUsbnH+Q3VxTDmxOq+zffskqJiOtFpZda+OV/M6uQKepLof0NWAAAAAAAAAAAAAAAAAAAAAAAAAAAgAr8Aj5RWY0PDbn2AAAAAElFTkSuQmCC" alt="sry"></a></div>
		</div>
	
			
		
	</div>
	
</main>

<style>
	main {
		text-align: center;
		max-width: 100vw;
		background-color: black;
		margin: 0 auto;
	}
	.navbar{
		display: grid;
		grid-template-columns: repeat(3,1fr);
		max-width: 100vw;
		height: 70px;
		background-color: black;
		font-weight:1000;
		display: flex;
		justify-content: center;
		align-items: center;
		column-gap: 30px;
		
	}
	.body{
		background-color: black;
		max-width: 100vw;
		min-height: 92vh;
		
	}
	.name{
		color: greenyellow;
		font-size: 30px;
		
		
	}
	.namecont{
		width: 100vw;
		height: 30vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.partition{
		width: 70vw;
		height: 1px;
		background-color: grey;
	}
	.pc{
		display: flex;
		justify-content: center;
	}
	body{
		display: flex;
		align-items: center;
		justify-content: center;
		max-height: 40vh;
	}
	.wrapper{
		display: inline-flex;
	}
	.wrapper .static-text{
		color: white;
		font-size: 60px;
		font-weight: 400;
		font-family: fantasy;

	}
	.wrapper .dynamic-text{
		margin-left: 10px;
		overflow: hidden;
		line-height: 90px;
		height: 90px;
	}
	.dynamic-text .li{
		font-family: fantasy;
		list-style: none;
		font-size: 50px;
		font-weight: 500;
		color: green;
		position: relative;
		top: 0px;
		/* left: 0px; */
		text-align: left;
		animation: slide 6s steps(3) infinite;
		z-index: 1;
		
	}
	@keyframes slide{
		100%{
			top: -270px;
		}

	}
	.dynamic-text .li span{
		position: relative;
		

	}
	.dynamic-text .li span::after{
		content:"";
		position: absolute;
		top: 0px;
		left: 0;
		height: 100%;
		width: 100%;
		border-left: 2px solid green;
		animation: typing 2s steps(30) infinite ;
		background: black;
		z-index: 1;
	}
	@keyframes typing{
		100%{
			left: 100%;
			margin: 0 -35 0 35px;
		}
		
	}
	.bar{
		/* height: 400px;
		width: 60px;
		
		float: right; */
		margin-top: 60px;
		height: 100px;
		max-width: 100vw;
		display: grid;
		grid-template-columns: repeat(3,1fr);
		display: flex;
		justify-content: center;
		align-items: center;
		column-gap: 70px;

	}
	img{
		max-height: 50px;
		border-radius: 10px;
	}
	button{
		color: rgb(47, 133, 209);
		background-color: black;
		border: none;
	}
	@media screen and (max-width:540px){

		.static-text{
			
			
			
			position: absolute;
			left: 40px;
			
			
		}
		.dynamic-text{
			position: absolute;
			top: 385px;
			left: 20px;
		}
		.bar{
			position: absolute;
			top: 500px;
			left: 40px;
		}
		
		
	}

	
</style>
