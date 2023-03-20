<script>
    import { element } from "svelte/internal";



const elements =[
	{
		name:"H",
		id:1
	}
	,
	null,
	null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,
	{
		name:"He",
		id:2
	},
	{
		name:"Li",
		id:3
	}
	,
	{
		name:"Be",
		id:4
	},null,null,null,null,null,null,null,null,null,null,
	{
		name:"B",
		id:5
	},

	{
		name:"C",
		id:1
	},
	{
		name:"N",
		id:1
	},
	{
		name:"O",
		id:1
	},
	{
		name:"F",
		id:6
	},
	{
		name:"Ne",
		id:2
	},
	{
		name:"Na",
		id:3
	},
	{
		name:"Mg",
		id:4
	},null,null,null,null,null,null,null,null,null,null,
	{
		name:"Al",
		id:7
	},
	{
		name:"Si",
		id:5
	},
	{
		name:"P",
		id:1
	},
	{
		name:"S",
		id:1
	},
	{
		name:"Cl",
		id:6
	},
	{
		name:"Ar",
		id:2
	},
	{
		name:"K",
		id:3
	},
	{
		name:"Ca",
		id:4
	},
	{
		name:"Sc"
		
	},
	{
		name:"Ti"
		
	},
	{
		name:"V"
	
	},
	{
		name:"Cr"
		
	},
	{
		name:"Mn"
		
	},
	{
		name:"Fe"
		
	},
	{
		name:"Co"
		
	},
	{
		name:"Ni"
		
	}
	,
	{
		name:"Cu"
		
	},
	{
		name:"Zn",
		
	},
	{
		name:"Ga",
		id:7
	},
	{
		name:"Ge",
		id:5
	},
	{
		name:"As",
		id:5
	},
	{
		name:"Se",
		id:1
	},
	{
		name:"Br",
		id:6
	},
	{
		name:"Kr",
		id:2
	},
	{
		name:"Rb",
		id:3
	},
	{	name:"Sr",
		id:4
	},
	{
		name :"Y"
	},
	{
		name: "Zr"
	},
	{
		name:"Nb"
	},
	{
		name:"Mo"
	},
	{
		name:"Tc"
	},
	{
		name:"Ru"
	},
	{
		name:"Rh"
	},
	{
		name:"Pd"
	},
	{
		name:"Ag"
	},
	{
		name:"Cd"
	},
	{
		name:"In",
		id:7
	},
	{
		name:"Sn",
		id:7
	},
	{
		name:"Sb",
		id:5
	},
	{
		name:"Te",
		id:5
	},
	{
		name:"I",
		id:6
	},
	{
		name:"Xe",
		id:2
	},
	{
		name:"Cs",
		id:3
	},
	{
		name:"Ba",
		id:4
	},
	{
		name:"La"
	},
	{
		name:"Hf"
	},
	{
		name:"Ta"
	},
	{
		name:"W"
	},
	{
		name:"Re"
	},
	{
		name:"Os"
	},
	{
		name:"Ir"
	},
	{
		name:"Pt"
	},
	{
		name:"Au"
	},
	{
		name:"Hg"
	},
	{
		name:"Ti",
		id:7
	},
	{
		name:"Pb",
		id:7
	},
	{
		name:"Bi",
		id:7
	},
	{
		name:"Po",
		id:5
	},
	{
		name:"At",
		id:6
	},
	{
		name:"Rn",
		id:2
	},
	{
		name:"Fr",
		id:3
	},
	{
		name:"Ra",
		id:4
	},
	{
		name:"+Ac"
	},
	{
		name:"Rf"
	},
	{
		name:"Ha"
	},
	{
		name:"Sg"
	},
	{
		name:"Ns"
	},
	{
		name:"Hs"
	},
	{
		name:"Mt"
	},
	{
		name:"110"
	},
	{
		name:"111"
	},
	{
		name:"112"
	},
	{
		name:"113",
		id:7
	}


]
</script>


<div class="container">
	{#each elements as element }
		{#if !element}
			<div></div>
			{:else if element.id==1}
				<div class="green">{element.name}</div>
			{:else if element.id==2}
				<div class="orangered">{element.name}</div>
			{:else if element.id==3}
				<div class="orange">{element.name}</div>
			{:else if element.id==4}
				<div class="blue">{element.name}</div>
			{:else if element.id==5}
				<div class="purple">{element.name}</div>
			{:else if element.id==6}
				<div class="yellow">{element.name}</div>
			{:else if element.id==7}
				<div class="turq">{element.name}</div>
			{:else}
				
			<div class="kutu1">{element.name}</div>
		{/if}
		
	{/each}
</div>




<style>
	*{
    margin:0px;
    padding : 0px;
    box-sizing: border-box;
	}
	.container{
		width: 500px;
		height: auto;
		margin: 0px auto;	
		display: grid;
		grid-template-columns: repeat(18, 50px);
		grid-auto-rows: 50px;
		gap:5px;
		 
	}

	.kutu1{
		background: rgb(83, 83, 237);
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}
	.yellow{
		background: rgb(222, 222, 16);
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}

	.turq{
		background: turquoise;
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}
	
	.green{
		background: rgb(53, 184, 53);
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}
	.orange{
		background: orange;
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}
	.blue{
		background: rgb(49, 49, 170);
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}
	.purple{
		background: purple;
		width: 50px;
		display: grid;
		align-items: center;
		justify-items: center;
	}


	.orangered{
		width: 50px;
		background: orangered;
		display: grid;
		align-items: center;
		justify-items: center;
	}
</style>