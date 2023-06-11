<svelte:head>
	<title>WebSkimmers</title>
	<meta name="description" content="information about webskimmers" />
</svelte:head>

<div class="container">
	<div class="divider">
		<h1> Types / Examples <h1>
	</div>
</div>


<div class = "examples">
	<ul class="imgList">
		<li> 		
			<img src="https://picsum.photos/200/300/?grayscale" alt="img">
			<h2> What are WebSkimmers?</h2>
			<p>Web skimmers are a type of malware that operates by adding a small piece of code onto a legitimate website to exfiltrate private information, including credit card information and social security numbers, to an attacker's server, while continuing to submit the details to the legitimate site. Because of the way they are made, web skimmers are impossible to detect just by looking at the web page since they operate entirely in the background and have no obvious indicators. (Bower)</p>
		</li>

		<li> 		
			<img src="https://picsum.photos/200/300/?grayscale" alt="img">
			<h2>Origins?</h2>
			<p>Web skimmer attacks are also called form jacking, JS-sniffers, JavaScript skimmer, or Magecart attacks, owing to the fact that they were first widely identified in use on sites running the Magento software.</p>

			<p>Web skimmers take their name from ATM skimmers, where a criminal will place counterfeit hardware onto real cash machines to steal credit card information, similar to the injected code of a web skimmer sending sensitive consumer information to an attacker's server. (Bower)</p>

			<p>Web skimmers started to enter the public eye in 2018 after a series of high-profile attacks on major retailers became known. Subjects of these attacks included British Airways, Newegg, and Ticketmaster. TheBritish Airways attack alone had an estimate of up to 380,000 consumers that had their private information stolen.  (Bower)</p>
		</li>
	</ul>
</div>



<div class="BottomSection">
  <div class="content">
    <h1>How do they work ?</h1>
    <hr>
    <div class="BottomInfo">
      <p class="BottomInfoText">
				A web skimmer is a form of confidentiality attack that utilizes a piece of malicious code embedded in a legitimate website to secretly send personal information to an adversary. (Bower)
      </p>
			<p class="BottomInfoText">
			
			Injection Method

			<br>
			For a skimming attack to occur, code has to be injected into a target website. There are multiple methods that culprits use that all depend on how the target website is designed, is architectured, and what underlying software it uses. Some methods are a rogue employee from within the organization may insert skimmer code directly onto the target website's server, or an e-commerce platform may be attacked using a cross-site scripting (XSS) vulnerability. In what is referred to as a supply-chain attack, skimmers could also be added to a website by taking advantage of a third-party resource. For instance, if a JavaScript library hosted on a CDN was compromised by having a skimmer inserted into its code, any website that imported the resource would be vulnerable to a skimming attack. (Bower)

			</p>
      <p class="BottomInfoText">
				Attack Families
				<br>
					There are multiple forms of skimming script, some are inspired by others, but some are wholly original. Because of this, it is challenging to classify the various assault families into a clear taxonomy. RiskIQ, a California-based cyber security company, claims that there are at least seven different types of JavaScript skimming attacks, with an additional five variants not yet public. These attacks differ not only in their technical implementation but also in the sites they target. On the other side, Group-IB, a Russian cyber-defense company, claims to have discovered up to 38 distinct skimmer families.
			<p class="BottomInfoText">

			</p>
      <p class="BottomInfoText">
				Obfuscation Techniques
				<br>
				Skimmers are built in client-side JavaScript, as opposed to other forms of malware that  operate server side, and as a result, anyone visiting a website that is infected can view its source code. Due to this, skimmer software is made to obfuscate their code as  much is possible. Otherwise, purposefully alter and modify the source code such that it keeps the desired behavior but is challenging for humans to read and understand what the code actually does.

				Although, there are legitimate reasons for authors to obfuscate their code, such as attempts to hide the functionality of proprietary software or to hide email addresses from web crawlers.  Despite the fact that many malicious scripts are obfuscated by their authors, the presence of obfuscation does not automatically mean a script is malicious.

				Attackers frequently use methods like string splitting to evade signature-based detection systems, which scan files for specific strings that could indicate the presence of malicious scripts. The string "Hello world," for instance, might be broken up into a number of smaller strings and then concatenated together, looking like "Hel" + "lo w" + "orld." Using escape sequences to type text in a different way is another typical method. To circumvent signature-based detection, the string "x68x65x6cx6cx6f," which employs hexadecimal representations of ASCII letters, decodes to "Hello." As an example of a more sophisticated technique, tokenizing an entire file and replacing each token with smaller, equivalent base 62 values for compression and readability is demonstrated. To further confuse anyone attempting to understand the code, some scripts may even purposefully include dead code blocks (blocks of code that the program cannot access).
      </p>
			<p class="BottomInfoText">
			</p>
    </div>
  </div>
</div>

<div>

</div>

<style>
	.container{
		display: flex; 
		justify-content:center; 
		align-items:center;
		height: 200px; 
	}
	
	.divider{
		position: relative; 
		text-align: center; 
		padding:2rem;
	}

	.divider:before,
	.divider:after{
		content:"";
		position: absolute; 
		top: 50% ;
		width:180%; 
		height:1px; 
		background-color:#000;
	}
	.divider:before {
	
	left:0;
  margin-left: 100%; /* Adjust the position of the left bar */
}

	.divider:after {
		right:0;
		margin-right: 100%; /* Adjust the position of the right bar */
	}

	.examples{
		display:flex; 
		justify-content:center; 
	}

 .imgList{
		list-style:none; 
		display: flex; 
	}
	
	.imgList h2{

		padding-left:1.5rm;
	}
	.imgList li {
		margin-right:10px; 
		padding-left:4rem;
		padding-right:4rem;
	}
	.imgList img{
		width:15rem;
		display:block;
		border-radius:50%;
	}
	.BottomSection {
		display: flex;
	}

	.content {
		flex: 1;
		padding-right: 20px;
	}

	h1 {
		margin-bottom: 10px;
	}

	hr {
		width: 100%;
	}

	.BottomInfoText {
		margin-bottom: 20px;
	}

	.image-container {
		display: flex;
		justify-content: flex-end;
		align-items: flex-start;
	}


</style>
